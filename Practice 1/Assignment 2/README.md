# Phân tích và xây dựng Web

## 1. Phân tích bố cục tổng thể

### Cấu trúc layout

Trang web có bố cục dạng **Grid** gồm:

- 1 tiêu đề chính: _KHÓA HỌC SẮP KHAI GIẢNG_
- Danh sách các khóa học hiển thị theo **3 cột × 2 hàng**

Sơ đồ bố cục:

```
---------------------------------
| KHÓA HỌC SẮP KHAI GIẢNG         |
---------------------------------
| Card | Card | Card             |
|------|------|------            |
| Card | Card | Card             |
---------------------------------
```

---

## 2. Nhận diện các thành phần giao diện

### 2.1. Container chính

- Chứa toàn bộ nội dung khóa học
- Sử dụng thẻ `<section>` hoặc `<div>`

### 2.2. Card khóa học

Mỗi khóa học được biểu diễn bằng **một card**, gồm các phần:

1. Ảnh minh họa khóa học
2. Tên khóa học
3. Mô tả ngắn
4. Danh sách thông tin chi tiết có icon

### 2.3. Các phần tử HTML sử dụng

| Thành phần | Thẻ HTML                       |
| ---------- | ------------------------------ |
| Ảnh        | `<img>`                        |
| Tiêu đề    | `<h3>`                         |
| Mô tả      | `<p>`                          |
| Danh sách  | `<ul><li>`                     |
| Icon       | Font Awesome / Bootstrap Icons |

---

## 3. Phân tích chi tiết một Card khóa học

Ví dụ: **LẬP TRÌNH WEB FULLSTACK**

### Nội dung card:

- Ảnh đại diện khóa học
- Tên khóa học
- Mô tả tổng quan
- Thông tin chi tiết:
  - Ưu đãi học phí
  - Thời gian khai giảng
  - Thời lượng khóa học

Mỗi dòng thông tin cần thêm **Icon + Text**.
