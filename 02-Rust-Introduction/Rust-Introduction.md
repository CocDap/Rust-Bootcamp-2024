## Cách ghi chú 

+  `//` : ghi chú một dòng 
+ `/* ... */`: ghi chú nhiều dòng 
+ Ghi chú không ảnh hưởng tới việc thực thi code 

Ví dụ: 

```rust
// Xin chào mọi người
/*
    Tôi tên là Dụng
    Hiện tại tôi là Blockchain Engineer
*/
```

## Hiển thị kết quả đầu ra 

+ `println!` -> hiển thị kết quả ra màn hình console

Ví dụ: 

```rust
println!("Xin chào Rust Bootcamp 2024!");
```

## Biến 
+ Biến là đại diện cho giá trị 
+ Biến mặc định là bất biến (immutable)
+ Để tạo biến có thể thay đổi -> sử dụng từ khoá `mut`

```rust
let x = 5;
let mut y = 10; 
```

## Kiểu dữ liệu 
Có 2 kiểu dữ liệu:
+ Scalar: lưu trữ đơn giá trị như integer, float, char, boolean, string 
+ Compound: lưu trữ đa giá trị như Array, Tuple

Ví dụ:
```rust
   let bootcamp = "Rust Bootcamp"; 
   let year = 2024;           
   let free = true; 
```

## Ép kiểu dữ liệu 
+ Chuyển đổi kiểu dữ liệu này sang kiểu dữ liệu khác 
+ Dùng từ khoá `as`

Ví dụ:
```rust
let x = 42;
let y = x as f64;
```

## Toán tử 
+ Hỗ trợ toán tử cơ bản như `+`, `-`, `*`, `/`,... cho các phép toán số học 
+ Các toán tử so sánh như `==`, `!=`, `>`, `<`, ...
+ Các toán tử logic như `&&`, `||`, `!`
+ Ngoài ra còn có nhiều toán tử khác 

Tài liệu tham khảo: https://doc.rust-lang.org/book/appendix-02-operators.html#operators








