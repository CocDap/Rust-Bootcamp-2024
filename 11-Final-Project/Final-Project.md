### Final Project

## Final project sẽ gồm các kiến thức sau: 
+ Kiểu dữ liệu
+ Struct
+ Trait ( trait bound, associated type, )
+ Generic Type 
+ Viết unit tests (cách sử dụng `assert_eq!` để so sánh kết quả thực tế và kết quả mong muốn) (Phần này mặc dù ko có trong chương trình nhưng mọi người có thể hiểu đơn giản là viết các trường hợp test cho logic của mình có đúng hay không)
+ Cấu trúc file cơ bản : `lib.rs`, các module khác ví dụ như `energy.rs`
+ Macro trong Rust (Phần thảo luận)


Ví dụ :
+ Định nghĩa viết test case 
```rust
// định nghĩa viết test case 
#[cfg(test)]
mod tests {
    // unit test 
    #[test]
	fn one_greater_than_zero() {
        assert!(1>0, "1 lớn hơn 0");
    }
    #[test]
	fn one_equal_one() {
        assert_eq!(1, 1);
    }
}
```

+ Chạy test bằng `cargo test`

## Implementation
+ Đọc hiểu nội dung của logic 
+ Hoàn thành `todo!()`


## Run test

```bash
cargo test 
```
