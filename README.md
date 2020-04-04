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
## ![image](https://media.geeksforgeeks.org/wp-content/uploads/Loop1.png)
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
## ![Loop](https://kynangso.net/courses/bai-7-vong-lap-trong-java-loop-in-java.html/Bài-7-Vòng-lặp-trong-Java-Loops-in-Java-type.png)

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
## Link :(https://www.javatpoint.com/object-and-class-in-java)
### - Lớp là  khuôn mẫu để từ đó tạo ra có đối tượng, khi thiết kế một lớp ta cần nghĩ đến những đối tượng sẽ được tạo ra từ lớp đó.
### - Có 2 thông tin quan trọng trong mỗi đối tượng:
* Những thông tin mà đối tượng đó __biết__
* Những việc mà đối tượng đó __làm__
### - Đối tượng là 1 thực thể có trạng thái và hành vi dùng để thể hiện kết quả của 1 lớp.
### - Ta phải phân biệt rõ giữa biến tham chiếu đối tượng và đối tượng trong java
### - Có 4 cách để khởi tạo đối tượng trong java;
#### + Sử dụng từ khóa new
#### + Sử dụng phương thức newInstance()
#### + Sử dụng phương thức clone()
#### + Sử dụng phương thức factory,...
### - Khi ta dùng lệnh new để khởi tạo 1 đối tượng thì Java sẽ thực hiện 1 phương thức đăc biệt được gọi là Hàm Khởi Tạo (Contructor)
## Những đặc điểm quan trọng của Object in Java:
1.  Một đối tượng có thẻ tự lo cho bản thân , ta không phải cần biết hay quan tâm một đối tượng làm việc đó ntn.
2.  một đói tượng __biết__ về một số thứ và có thể __làm__ một số việc.
3.  Những gì đối tượng biết về chính nó được gọi là các __biến thực thể (thuộc tính )__ của nó. chúng đại diện cho trạng thái của đối tượng.
4.  Những gì một đối tượng có thể __làm__ đgl __*phương thức*__. Chúng đại diện cho hành vi của đối tượng.
5.  __Tại thời gian chương trình chạy, một đối tượng java chính là 1 nhóm các đối tượng đang "nói chuyện" với nhau.__  
_*(nói chuyện) là các phương thức đang gọi lẫn nhau*_
## Tạo và sử dụng đối tượng:
### Để tạo và sử dụng một đối tượng, ta cần đến hai lớp:
#### 1. Một lớp dành cho kiểu đối tượng mà ta muốn tạo.
#### 2. Một lớp khác để thử nghiệm lớp đó.
* Lớp thử nghiệm là chương trình nơi ta đặt phương thức __*main*__ , và tại phương thức main đó ta tạo và sử dụng một đối tượng thuộc lớp vừa xây dựng. Lớp thử nhiệm chỉ có một nhiệm vụ duy nhát: chạy thử các biến và phương thức của lướp đối tượng mới.
## 1.Trạng Thái của đối tượng:
### Trạng thái của đối tượng nói lên tính đặc thù hay đặc trưng của đối tượng đó.
## 2.Hành Vi của đối tượng:
### - là hành động mà đối tượng có trách nhiệm phải thực hiện.

## Hàm Contructor trong Java:
## link: (https://www.javatpoint.com/java-constructor)
### - Contructor là 1 phương thức đặt biệt được sủ dụng để khởi tạo một đối tượng.
### Đặc điểm của 1 hàm Contructor:
* Một Contructor trong java phỉa có kiểu trả về rõ ràng.
* Nõ có thể là abtract, final, static.
* trên của __contructor__ phải giống với tên class của nó.
### Trong Java có 2 kiểu Contructor
### 1 Default Contructor (hàm khởi tạo)
<class_name>(){};
### 2 Parametezited Contructor ( Hàm khởi tạo có đối số)
* tên của contructor phải trùng tên của lớp để phân biệt với phương thức bình thường.
* Một lớp có thể có nhiều contructor, nhưng tham số truyền vào phải khác nhau.
* Với 1 lớp có nhiều contructor ta có thể gọi từ Contructor này đến Contructor khác. __*sử dụng từ khóa THIS*__
* Một Contructor chỉ được thực thi 1 lần khi từ khóa New được gọi
### 3 hàm khởi tạo có tham số
## Thư Viện sử lý sô liệu
### 1- Decimalformat
* DecimalFormat __dcf__ = new DecimaFormat("#.##");
+ Ví dụ: 3.33333 => 3.34
### 2- DecimalFormatSymbol
* DecimalFormatSymbols __dfs__ = new DeciamlFormatSymbol(Locale.getDault);
+ ví dụ : 1234567 ==> 1,234,567
## Thư Viện Xử Lý ngày tháng trong java:
### 1- Calendar:
* __Lấy ngày tháng năm hiện tại__: Calendar cal = Calendar._*getInstance*-();
* __Lấy từng tiêu Chí__: + cal.get(Calendar.__YEAR__);
                     + cal.get(Calendar.__MONTH__);
                     + cal.get(Calendar.__DAY_OF_MONTH__);
* __Thay đổi tiêu Chí__: cal.set(Calendar.YEAR,1990);
* __Lấy ngày tháng__: Date t = cal.getTime();

###  2 - SimpleDateFormat:
### SimPleDateFormat sdf = new SimPleDateFormat("DD/MM/YYYY");
## Thư Viện Xử Lý Toán Học:
|Tên Phương Thức| Mô Tả|
|--------------:|:-----:|
|PI| Trả về giá trị PI|
|abs(a)| trả về trị tuyệt đối của a|
|max(a,b)|Trả về giá trị lớn nhắt giữa a và b|
|min(a,b)| Trả về giá trị nhỏ  nhất giữa a và b|
|sqrt(a)| Trả về căn bậc 2 của a|
|Pow(x,y)| Trả về tính giá trị lũy thừa X^y|
|sin(radian)| Tính sin, radian =Math.PI*goc/180.|

### Hàm Random (Số nguyên):
* Random rd = __new__ Random();
- Ví dụ: int x = rd.nextInt(n);
+ Trả về ngẫu nhiên từ [0...n-1]
# 03/04/2020
## Thư viện xử lý chuỗi
### StringBuilder:
* Lớp StringBuilder
- StringBuilder __sb__ = new StringBuilder();
+ sb.apppend (); ==> nhập 1 chuỗi String
+ sb.Insert(int offset, String ); ==> thêm vào 1 chuỗi từ 1 vị trí thứ Offset;
+ sb.delete(int StartIndex, int endIndex); ==> xóa 1 chuỗi từ ví trí bắt đầu đến vị trí kết thúc
## Hàm  tìm chuỗi trong String
### Indexof("String s"); ==> kiểu trả về INT
* Trả về vị trí ký tự đầu tiên
### lastIndexof("String s"); ==> kiểu trả về INT
* Trả về vị trí ký tự cuối cùng
## Hàm đổi chuỗi trong String
### Replace("String s","String S2"); 
* Đổi chuỗi s thì chuỗi S2
### ReplaceFirst("String s","String S2");
* Đổi chuỗi s ở vị trí xuất hiện đầu tien thành S2
