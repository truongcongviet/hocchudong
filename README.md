# hocchudong
note everything I learned
# Các khái niệm căn bản:
## lớp là dùng để định nghĩa một thực thể theo thuộc tính và hành động chung.
## Đối tượng là một trường hợp của một lớp
## Trong mỗi 1 đối tượng các khía cạnh sau đây cần được đinh rõ:
### Tình trạng (state)
### Thái độ (behavior)
### chân tính (indentity)
## Thuộc tính là một đặt tính để mô tả đói tượng
## Phương thức là một sự xác định về cách thức hoạt đọng được thực thi
## Hàm thiết lập ("`Contructor)"` là một phương thức đặt biệt phải được gọi trước khi sử dụng bất kỳ PT nào tronng một lớp. Hàm thiết
## lập khởi tạo các thuộc tính và cấp phát bộ nhớ.
# 1. Biến
## Biến cung cấp một tên vùng nhớ để chương trình có thể thao tác, mỗi biến trong java có mỗi kiểu khái báo cụ thể
## 1.1 kiểu biến chính trong java
- Biến Cục bộ ( local variable)
- Biến thuộc thực (instance variable )
- Biến Stactic ( Biến của lớp) 
# __ cách khai báo cơ bản của các biến__
## data type variable [ = value][, variable [ = value] ...] ;\
## 1.1.1 Biến cục bộ
### - Vị trí khai báo là trong các phương thức, contructor hoặc block
### - Các biến cục bộ chỉ có thể nhìn thấy trong phương thức khai báo, constructor hoặc block
## 1.1.2 Biến thực thể ( instance)
### - Các biến thực thể được khai báo bên trong class nhưng bên ngoài phương thức, contructor
### - vd: public __String__ _name_;
## 1.1.3 Biến Static
### - được khia báo bên trong lớp nhưng bên ngoài các phương thức, contructoer or block
### - Các biến tĩnh thường được dùng khi muốn khai báo hằng số
### - vd: private static __double__ _salary_;
## Bài WRAPPER (19/03/2020):
## Đây là link bài học [Wrapperinjava](https://viettuts.vn/java/lop-wrapper-trong-java)
### Ý nghĩa : wrapper trong java là cung cấp cơ chế chuyển đổi kiểu dữ liệu nguyên thủy thành kiểu dữ liệu đối tượng.
### Các Wrapper class cung cấp cho chúng ta nhiều method để thao tác với kiểu dữ liệu nguyên thuỷ tương ứng
### Wrapper class cung cấp cho chúng ta nhiều cơ giúp thao tác nhanh gọn thế nhưng không phải lúc nào cũng sử dụng chúng. Vì Wrapper class sẽ phải khởi object và tốn bộ nhớ hơn. Chúng ta cần phân tích kỹ trước khi sử dụng.
