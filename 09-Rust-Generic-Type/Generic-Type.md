## Generic Type 

### Định nghĩa 
+ Generic type là kiểu dữ liệu chung (placeholder) có thể thay thế cho các kiểu dữ liệu Rust

+ Sử dụng kí tự in hoa 

Ví dụ 1:

+ Định nghĩa generic type là T -> T có thể là các kiểu dữ liệu primitive, array, tuple, ...

```rust
pub enum Option<T> {
    None,
    Some(T),
}
```

Ví dụ 2:
+ Định nghĩa 2 generic type là `T` và `E`
+ `T` là `placeholder` -> đại diện cho giá trị trả về 
+ `E` -> đại diện cho lỗi trả về  

```rust
enum Result<T, E> {
   Ok(T),
   Err(E),
}
```


### Generic Struct in Rust
+ Định nghĩa 1 generic type `T` đối với Struct 

```rust
struct Point<T> {
    x: T,
    y: T,
}
```

+ Định nghĩa 2 generic type `T` và `U` đối với Struct 

```rust
struct Point<T,U> {
    x: T,
    y: U,
}
```

### Generic Function in Rust
+ Generic Type như là 1 đầu vào của hàm 


```rust
    fn min<T: PartialOrd>(a: T, b: T) -> T {
        if a < b {
            return a;
        } else {
            return b;
        }
    }
```

### Khi nào sử dụng Generic type 
+ Viết code linh hoạt và làm việc với nhiều kiểu dữ liệu khác nhau 

### Hiệu suất code khi mà sử dụng Generic Type
+ Không ảnh hưởng gì đến quá trình chạy runtime (thực thi code) so với sử dụng kiểu dữ liệu cụ thể 
+ Trong quá trình biên dịch code liên quan tới generic thì Bộ biên dịch Rust sẽ thực hiện `monomorphization`
+ Tốn thời gian biên dịch lâu ( vì tạo ra nhiều phiên bản khác nhau mà chương trình có thể sử dụng)
Ví dụ:

```rust
enum Option_i32 {
    Some(i32),
    None,
}

enum Option_f64 {
    Some(f64),
    None,
}

fn main() {
    let integer = Option_i32::Some(5);
    let float = Option_f64::Some(5.0);
}

```




