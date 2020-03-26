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
### - Ý nghĩa : wrapper trong java là cung cấp cơ chế chuyển đổi kiểu dữ liệu nguyên thủy thành kiểu dữ liệu đối tượng.
### - Các Wrapper class cung cấp cho chúng ta nhiều method để thao tác với kiểu dữ liệu nguyên thuỷ tương ứng
### - Wrapper class cung cấp cho chúng ta nhiều cơ giúp thao tác nhanh gọn thế nhưng không phải lúc nào cũng sử dụng chúng. Vì Wrapper class sẽ phải khởi object và tốn bộ nhớ hơn. Chúng ta cần phân tích kỹ trước khi sử dụng.
## MẢNG TRONG JAVA:
### 1. ưu điểm:
#### Tối ưu code: Gom các phần tử liên quan vào chung một với nhau giúp code gọn gàng hơn. Có thể truy cập ngấu nhiên: Do các vị trí ô lưu trữ liên tiếp ta có thể truy cập ngấu nhiên bằng chỉ số phần tử dễ dàng và nhanh chóng.
### 2. Nhược điểm
#### - Giới hạn kích thước: Khi sử dụng mảng ta phải khai báo kích thước lưu trữ của mảng và không thể thay đổi kích thước trong lúc chạy. Vùng lưu trữ phải liên tiếp: Đây cũng là vừa ưu vừa nhược điểm. Vì yêu cầu các ô nhớ liên tiếp nên phải tốn không gian bộ nhớ, hoặc đủ ô nhớ nhớ nhưng các ô nhớ không tiếp nên không thể khai báo được.
### ** Cách khai báo:
### <kiểu dữ liệu> [] <tên mảng> = new <kiểu dữ liệu>[kích cỡ mảng];
# Vòng lặp (loop):
## Đây là link bài học [Loopinjava](https://www.javatpoint.com/java-for-loop)
## ![alt text](https://www.javatpoint.com/java-for-loop/java-loops.png)
## 1_ For Loop
### - Vòng for là cấu trúc hỗ trợ việc viết các vòng lặp mà số lần lặp được kiểm soát bằng biến đếm
### - Sử dụng khi biết rõ về số lần lặp, cú pháp vòng lặp __for__ là:
### for(init; condition; incr/decr){
### // code to be executed 
### }
## Trong đó: 
- __init__ :  biểu thức thi hành một lần khi bắt đầu vòng lặp 

- __condition__: mỗi lần kiểm tra điều kiện này là true thì khối lệnh thi hành, nếu false sẽ thoát khỏi vòng lặp.

- __Decrement__  thi hành mỗi lần đến cuỗi vòng lặp
## 2_ WHILE loop:

### - Vòng while lặp đi lặp lại chuỗi hành động, gọi là thân vòng lặp, nếu như điều kiện lặp vẫn còn được thỏa mãn

### - Vòng lặp __while__ thi hành khối lệnh khi mà điều kiện kiểm tra vẫn là __true__ , Cú pháp thực thi câu lệnh:

### while(điều kiện lặp){  
### //Nội dụng cần lặp
### }
## 3_ DO WHILE LOOP:

### - Tương tự vòng lặp while nhưng khối lệnh thi hành trước rồi mới kiểm tra điều kiện, nếu điều kiện đúng thì lặp lại. Có nghĩa là do ... while khối lệnh luôn có ít nhất một lần được thi hành

### do{  
### // thân vòng lặp 
### while(điều kiện lặp); 

# Switch Case: 
## - Đây là link bài học [Switch](https://www.javatpoint.com/java-switch)

### - Lệnh switch rẽ nhánh, nó kiểm tra biến với một danh sách giá trị. Một giá trị gọi là một trường hợp case, và khối lệnh thi hành từ đó nếu điều kiện kiểm tra trên là đúng.

### - Vấn đề đặc biệt của cấu trúc switch là các lệnh break. Nếu ta không tự gắn một lệnh break vào cuối chuỗi lệnh cần thực hiện cho mỗi trường hợp, chương trình sẽ chạy tiếp chuỗi lệnh của trường hợp sau chứ không tự động nhảy tới cuối cấu trúc switch

### - NOTE: Kể từ Java SE 7, ta có thể dùng các đối tượng String làm nhãn cho các lệnh case

### - Nếu expression không bằng giá trị nào trong các case thì có hai trường hợp xảy ra: Nếu có khối default: thì sẽ chạy code từ đây, nếu không có default: khi không có code nào trong khối switch thi hành.
# 22/03/2020
## Lệnh Break trong java
## Link (https://www.javatpoint.com/java-break)
### - Từ khóa break được sử dụng để dừng toàn bộ vòng lặp. __Từ khóa break phải được sử dụng bên trong bất kỳ vòng lặp nào hoặc một lệnh switch.__ 
### - Lệnh break khi được thực thi bên trong một cấu trúc lặp hay một cấu trúc switch có tác dụng lập tức chấm dứt cấu trúc đó, chương trình sẽ chạy tiếp ở lệnh nằm tiếp sau cấu trúc đó. Lệnh break thường được dùng để kết thúc sớm vòng lặp (thay vì đợi đến lượt kiểm tra điều kiện lặp) hoặc để bỏ qua phần còn lại của cấu trúc switch.

### - Từ khóa break sẽ dừng sự thực thi của vòng lặp trong cùng và bắt đầu thực thi dòng code tiếp theo sau khối đó.
### *Cú pháp của lệnh break trong Java như sau: __break;__
## Lệnh continue trong java;
# link (https://www.javatpoint.com/java-continue);
### - Từ khóa continue có thể được sử dụng trong bất kỳ cấu trúc điều khiển vòng lặp nào. Nó làm cho vòng lặp ngay lập tức tiếp tục tiến trình lặp tiếp theo của vòng lặp.
## Comment trong java:
# link (https://www.javatpoint.com/java-comments)
### $-__mục đích__: Các đoạn comment này dùng để giải thích về ý nghĩa, công dụng của các biến, phương thức, các Class hoặc bất kỳ những dòng lệnh khác để cho chương trình của chúng ta dễ hiểu và dễ bảo trì hơn
### - Trong Java, chúng ta có 3 cách comment code như sau
### *
 * Comment nhiều dòng
 * Dòng 1
 * Dòng 2
 * ...
 * Dòng n
 
 */
 
// Comment 1 dòng
 
/**
 * Comment đặc biệt dùng để tạo Java code documentation ở định dạng HTML (Java Document)
 
*/
# 23/03/2020
## 1.Các ký tự ngắt văn bản trong Java:
|Ký tự ngắt | Miêu tả|
|----------:|:-------:|
|/t|	Chèn một tab vào văn bản tại điểm này|
|/b|	Chèn một backspace vào văn bản tại điểm này|
|/n|	Chèn một dòng mới vào văn bản tại điểm này|
|/r|	Chèn một carriage return  vào văn bản tại điểm này|
|/f|	Chèn một form feed vào văn bản tại điểm này|
## 2.1Biến Static trong java:
### - Biến static có thể được sử dụng để tham chiếu thuộc tính chung của tất cả đối tượng (mà không là duy nhất cho mỗi đối tượng),
### - Biến static giúp bộ nhớ chương trình của bạn được sử dụng hiệu quả hơn
# 25/03/2020
## Hàm Nhập xuất dữ liệu Scanner
### - Để sử dụng từ khóa Scanner cần phải Import gói java.untill.Scanner
### - Để sử dụng phương thức Scanner thì cần tạo đối tượng Scanner trong Java như sau: Scanner input = new Scanner (System.in);
### - Các phương thức thường được sử dụng của lớp Scanner trong java:
|Phương thức| Mô tả|
|-----------:|:-----:|
|public String text()|Trả về kết quả nội dụng trước khoảng trắng|
|public String textLine()|Trả về kết quả nội dụng của một chuỗi nhập vào (String)|
|public String nextInt()|Trả về kết quả kiểu Interger|
## Các phép toán trong java:
## 1- Toán tử số học trong Java:
|toan tử| Miêu Tả|
|------:|:-------:|
| + | Phép Cộng|
| - | phép trừ: trừ toán hạng trái cho toán hạn phải|
| * | Phép nhân|
| / | phép Chia: Chia toán hạng trái cho toán hạng phải|
| % | Phép chia lấy phần dư: Lấy phần dư của phép chia toán hạng trái cho toán hạng phải|
| ++ | Phép lượng gia: lượng gia giá trị toán hạng thêm 1|
| -- | Phép lượng giảm: lượng giảm giá trị toán hạng đi 1| 

## 2 - Toán tử quan hệ trong java:
| toán tử | Miêu tả| 
|--------:|:------:|
| == | Kiểm tra nếu giá trị của hai toán hạng có cân bằng hay không, nếu có thì điều kiện là true.|
| != | Kiểm tra nếu giá trị hai toán hạng là cân bằng hay không, nếu không cân bằng, thì điều kiện là true|
| > | Kiểm tra nếu toán hạng trái có lớn hơn toán hạng phải hay không, nếu có thì điều kiện là true|
| < | Kiểm tra nếu toán hạng phải có lớn hơn toán hạng trái hay không, nếu có thì điều kiện là true|
| <= | Kiểm tra nếu toán hạng trái có lớn hơn hoặc bằng toán hạng phải hay không, nếu có thì điều kiện là true|
| >= | Kiểm tra nếu toán hạng phải có lớn hơn hoặc bằng toán hạng trái hay không, nếu có thì điều kiện là true|

## 3- Toán tử logic trong java
 
| Toán tử | Miêu tả|
|--------:|:-------:|
| && | Toán tử Và logic. Nếu cả hai toán hạng cùng 1 điều kiện , thì khi đó điều kiện là true|
| // | Toán tử Và logic. Nếu 1 trong 2 toán hạng cùng đúng điều kiện , thì khi đó điều kiện là true |
| ! | Toán tử Phủ định logic. Sử dụng để đảo ngược lại trạng thái logic của toán hạng đó. Nếu điều kiện toán hạng là true thì phủ định nó sẽ là false|
# 26/03/2020
## 1- Object trong java:
### - Đối tượng là 1 thực thể có trạng thái và hành vi dùng để thể hiện kết quả của 1 lớp.
### - Ta phải phân biệt rõ giữa biến tham chiếu đối tượng và đối tượng trong java
### - Có 4 cách để khởi tạo đối tượng trong java;
#### + Sử dụng từ khóa new
#### + Sử dụng phương thức newInstance()
#### + Sử dụng phương thức clone()
#### + Sử dụng phương thức factory,...
### - Khi ta dùng lệnh new để khởi tạo 1 đối tượng thì Java sẽ thực hiện 1 phương thức đăc biệt được gọi là Hàm Khởi Tạo (Contructor)

