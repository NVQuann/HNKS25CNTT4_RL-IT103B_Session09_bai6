## 1. Khái niệm & Khởi tạo

- Cấu trúc lưu trữ theo cặp Key-Value
- Khởi tạo nhanh bằng Object Literal `{ }`
- Thuộc nhóm kiểu dữ liệu tham chiếu (Reference type)

## 2. Cú pháp truy cập thuộc tính

- Dot Notation (`obj.prop`)
  - Dùng cho key tĩnh, tên biến hợp lệ
- Bracket Notation chuỗi (`obj['prop']`)
  - Bắt buộc khi key chứa ký tự đặc biệt, khoảng trắng, gạch ngang
- Bracket Notation biến động (`obj[var]`)
  - Bắt buộc dùng cho dynamic key (biến chứa tên thuộc tính)

## 3. Thao tác CRUD trên Object

- Create: Thêm key mới (`obj.newKey = value`)
- Read: Đọc giá trị (`obj.key` hoặc `obj['key']`)
- Update: Ghi đè giá trị (`obj.key = newValue`)
- Delete: Xóa hoàn toàn key bằng toán tử `delete obj.key`

## 4. Mảng các Đối tượng (Array of Objects)

- Đại diện cho mô hình bảng dữ liệu (Table/Collection)
- Quản lý danh sách thực tế (VD: Danh sách phòng Grand Hotel)
- Thao tác bằng vòng lặp `for` để duyệt mảng
- Tìm kiếm/Lọc dữ liệu dựa trên thuộc tính định danh (VD: `roomId`)

## 5. Cạm bẫy & Sai sót thường gặp

- Lỗi `for...in`: Lấy giá trị sai vì dùng `obj.key` thay vì `obj[key]`
- Xóa ảo: Gán `key = undefined` khiến key vẫn tồn tại (phải dùng `delete`)
- Lỗi tham chiếu: Gán `=` trực tiếp 2 object chỉ sao chép địa chỉ bộ nhớ
- Hậu quả tham chiếu: Sửa object này vô tình làm thay đổi object kia
