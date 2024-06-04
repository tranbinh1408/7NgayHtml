# Báo cáo môn lập trình ngôn ngữ javascript – ngày 3
I.	HTML TABLES
1.	HTML tables
-	Ô bảng: <td>
-	Hàng bản: <tr>
-	Tiêu đề bảng: <th>
2. Đường viền bảng HTML
-	Cách thêm đường viền bảng: border
Vd: table, th, td {
  border: 1px solid black;
}
-	Đường viền bảng được thu gọn: border – collapse
Vd: table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
-	Biên giới bàn tròn: border – radius
Vd: table, th, td {
  border: 1px solid black;
  border-radius: 10px;
}
-	Đường viền bảng: border – style ( dotted, dashed, solid, double, groove, ridge, inset, none, hidden)
Vd:  th, td {
  border-style: dotted;
}
-	Màu viền: border – color
Vd:  th, td {
  border-color: #96D4D4;
}
3. Tiêu đề bảng
-	Tiêu đề cho nhiều cột: colspan
Vd: <table>
  <tr>
    <th colspan="2">Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table>
-	Bảng chú thích: caption
Vd: <table style="width:100%">
    <caption>Monthly savings</caption>
    <tr>
        <th>Month</th>
        <th>Savings</th>
    </tr>
    <tr>
        <td>January</td>
        <td>$100</td>
    </tr>
    <tr>
        <td>February</td>
        <td>$50</td>
    </tr>
    </table>
4. Khoảng đệm và khoảng cách bảng HTML
- Bảng HTMl – Đệm ô: padding-top, padding-bottom, padding-left, padding-right
- Khoảng cách ô: border-spacing
5. Bảng HTML colspan & Rowspan
-	Bảng HTMl – Colspan: Để tạo một ô trải dài trên nhiều cột, sử dụng colspan
Vd: <table>
  <tr>
    <th colspan="2">Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>43</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>57</td>
  </tr>
</table>
-	Rowspan: Để tạo một ô trải dài trên nhiều hàng
Vd: <table>
  <tr>
    <th>Name</th>
    <td>Jill</td>
  </tr>
  <tr>
    <th rowspan="2">Phone</th>
    <td>555-1234</td>
  </tr>
  <tr>
    <td>555-8745</td>
</tr>
</table>
6.	Tạo kiểu bảng HTML
-	Sọc ngựa vắn: Để tạo kiểu cho mọi thành phần hàng khác của bảng, hãy sử dụng :nth-child(even)
Để tạo kiểu cho mọi thành phần hàng khác của bảng, hãy sử dụng :nth-child(even)
Vd: tr:nth-child(even) {
  background-color: #D6EEEE;
}
-	Sọc vằn dọc: :nth-child(even)
Vd: td:nth-child(even), th:nth-child(even) {
  background-color: #D6EEEE;
}
-	Kết hợp sọc ngựa vằn dọc và ngang: Sử dụng rgba()màu để chỉ định độ trong suốt của màu
Vd: tr:nth-child(even) {
  background-color: rgba(150, 212, 212, 0.4);
}

th:nth-child(even),td:nth-child(even) {
  background-color: rgba(150, 212, 212, 0.4);
}
-	Bộ chia ngang: border – bottom
Vd: tr {
  border-bottom: 1px solid #ddd;
}
-	Bảng di chuột: Sử dụng :hover bộ chọn bật trđể đánh dấu các hàng trong bảng khi di chuột qua
Vd: tr:hover {background-color: #D6EEEE;}
7.	Nhóm bảng HTML
-	Nhóm bảng HtML: 
•	Phần tử này <colgroup>nên được sử dụng làm nơi chứa các thông số kỹ thuật của cột
•	Mỗi nhóm được chỉ định bằng một <col>phần tử
•	Thuộc spantính chỉ định số lượng cột có kiểu
•	Thuộc styletính chỉ định kiểu cho các cột
Vd: <table>
  <colgroup>
    <col span="2" style="background-color: #D6EEEE">
  </colgroup>
  <tr>
    <th>MON</th>
    <th>TUE</th>
    <th>WED</th>
    <th>THU</th>
...
-	Thuộc tính CSS hợp pháp: Chỉ có một lựa chọn rất hạn chế về thuộc tính CSS được phép sử dụng trong nhóm colgroup
•	Width
•	Visibility
•	Background
•	Border
-	Ẩn cột: visibility: collapse
Vd: <table>
  <colgroup>
    <col span="2">
    <col span="3" style="visibility: collapse">
  </colgroup>
  <tr>
    <th>MON</th>
    <th>TUE</th>
    <th>WED</th>
    <th>THU</th>
...
II.	Danh sách HTML
1.	Danh sách HTML
-	 Danh sách không có thứ tự:
•	Danh sách không có thứ tự bắt đầu bằng <ul>thẻ. Mỗi mục danh sách bắt đầu bằng <li>thẻ
•	Thuộc tính CSS list-style-typeđược sử dụng để xác định kiểu của điểm đánh dấu mục danh sách (disc, circle, square, none)
Vd1: <ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
Vd2: <ul style="list-style-type:disc;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
Vd3: # Danh sách lồng vào nhau
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
-	Danh sách HTMl được đặt hàng: 
•	Một danh sách có thứ tự bắt đầu bằng <ol>thẻ. Mỗi mục danh sách bắt đầu bằng <li>thẻ
•	Thuộc tính loại: type="1", type="A", type="a", type="I", type="i"
•	Danh sách kiểm soát: start
Vd1: <ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
Vd2: # Danh sách kiểm soát
<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol type="I" start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
-	Danh sách mô tả HTML: Thẻ <dl>xác định danh sách mô tả, <dt>thẻ xác định thuật ngữ (tên) và <dd> thẻ mô tả từng thuật ngữ
Vd: <dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
-	Danh sách ngang: 
Vd: <!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111111;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>
</body>
</html>
-	Danh sách mô tả HTML: Thẻ <dl>xác định danh sách mô tả, thẻ xác định thuật ngữ (tên) và thẻ mô tả từng thuật ngữ: <dt> <dd>
Vd: <dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
III.	HTML Div
-	Phần tử <div>: Theo mặc định, phần tử này <div>là phần tử khối, nghĩa là nó chiếm toàn bộ chiều rộng có sẵn và đi kèm với các ngắt dòng trước và sau
Vd: Lorem Ipsum <div>I am a div</div> dolor sit amet.
Kq: Lorem Ipsum
I am a div 
dolor sit amet.
-	Làm vùng chứa: Phần tử này <div>thường được sử dụng để nhóm các phần của trang web lại với nhau
Vd: <div>
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>London has over 13 million inhabitants.</p>
</div>
-	<div> cạnh nhau: float
Vd: <!DOCTYPE html>
<html>
<style>
div.mycontainer {
  width:100%;
  overflow:auto;
}
div.mycontainer div {
  width:33%;  
  float:left;
}
</style>
<body>

<div class="mycontainer">

  <div style="background-color:#FFF4A3;">
    <h2>London</h2>
    <p>London is the capital city of England.</p>
    <p>London has over 13 million inhabitants.</p>
  </div>
  
  <div style="background-color:#FFC0C7;">
    <h2>Oslo</h2>
    <p>Oslo is the capital city of Norway.</p>
    <p>Oslo has over 600.000 inhabitants.</p>
  </div>
  
  <div style="background-color:#D9EEE1;">
    <h2>Rome</h2>
    <p>Rome is the capital city of Italy.</p>
    <p>Rome has almost 3 million inhabitants.</p>
  </div>

</div>

</body>
</html>
-	Chặn nội tuyến: Nếu bạn thay đổi thuộc tính <div>của phần tử displaytừ blockthành inline-block, các <div>phần tử sẽ không còn thêm dấu ngắt dòng trước và sau nữa và sẽ được hiển thị cạnh nhau thay vì chồng lên nhau
Vd: <!DOCTYPE html>
<html>
<style>
div {
  width:30%;  
  display:inline-block;
}
</style>
<body>

<div style="background-color:#FFF4A3;">
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>London has over 13 million inhabitants.</p>
</div>

<div style="background-color:#FFC0C7;">
  <h2>Oslo</h2>
  <p>Oslo is the capital city of Norway.</p>
  <p>Oslo has over 600.000 inhabitants.</p>
</div>

<div style="background-color:#D9EEE1;">
  <h2>Rome</h2>
  <p>Rome is the capital city of Italy.</p>
  <p>Rome has almost 3 million inhabitants.</p>
</div>

</body>
</html>
-	Uốn cong: 
•	Mô-đun bố cục CSS Flexbox được giới thiệu để giúp thiết kế cấu trúc bố cục đáp ứng linh hoạt mà không cần sử dụng float hoặc định vị dễ dàng hơn
•	Để làm cho phương thức CSS flex hoạt động, hãy bao quanh các <div>phần tử bằng một <div>phần tử khác và đặt cho nó trạng thái là một thùng chứa flex
Vd: <style>
.mycontainer {
  display: flex;
}
.mycontainer > div {
  width:33%;
}
</style>
-	Lưới: 
•	Mô-đun bố cục lưới CSS cung cấp một hệ thống bố cục dựa trên lưới, với các hàng và cột, giúp thiết kế trang web dễ dàng hơn mà không cần phải sử dụng các float và định vị
•	Nghe gần giống như flex nhưng có khả năng xác định nhiều hàng và định vị từng hàng riêng lẻ
•	Phương pháp lưới CSS yêu cầu bạn bao quanh các <div>phần tử bằng một <div>phần tử khác và đưa ra trạng thái dưới dạng vùng chứa lưới, đồng thời bạn phải chỉ định độ rộng của mỗi cột
Vd: <style>
.grid-container {
  display: grid;
  grid-template-columns: 33% 33% 33%;
}
</style>
IV.	HTML Responsive
-	Cài đặt khung nhìn: Để tạo một trang web phản hồi, hãy thêm thẻ sau <meta> vào tất cả các trang web của bạn
Vd: <meta name="viewport" content="width=device-width, initial-scale=1.0">
-	Hiển thị hình ảnh khác nhau tùy thuộc vào chiều rộng trình duyệt: Phần tử HTML <picture>cho phép bạn xác định các hình ảnh khác nhau cho các kích thước cửa sổ trình duyệt khác nhau
Vd: <picture>
  <source srcset="img_smallflower.jpg" media="(max-width: 600px)">
  <source srcset="img_flowers.jpg" media="(max-width: 1500px)">
  <source srcset="flowers.jpg">
  <img src="img_smallflower.jpg" alt="Flowers">
</picture>
-	Truy vấn phương tiện truyền thông: Với truy vấn phương tiện, bạn có thể xác định các kiểu hoàn toàn khác nhau cho các kích thước trình duyệt khác nhau
Vd: <style>
.left, .right {
  float: left;
  width: 20%; /* The width is 20%, by default */
}

.main {
  float: left;
  width: 60%; /* The width is 60%, by default */
}

/* Use a media query to add a breakpoint at 800px: */
@media screen and (max-width: 800px) {
  .left, .main, .right {
    width: 100%; /* The width is 100%, when the viewport is 800px or smaller */
  }
}
</style>
-	Trang web đáp ứng: Trang web phản hồi sẽ trông đẹp mắt trên màn hình máy tính để bàn lớn và trên điện thoại di động nhỏ
V.	HTML Forms
-	Biểu mẫu HTML
Vd: <!DOCTYPE html>
<html>
<body>

<h2>HTML Forms</h2>

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 

<p>If you click the "Submit" button, the form-data will be sent to a page called "/action_page.php".</p>

</body>
</html>
-	Phần tử <form>: Được sử dụng để tạo biểu mẫu HTML cho người dùng nhập
Vd: <form>
.
form elements
.
</form>
-	Phần tử <input>: <input type="text">, <input type="radio">, <input type="checkbox">, <input type="submit">, <input type="button">
-	Trường văn bản: <input type="text">
Vd: <form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
-	Thuộc tính <action>:  xác định hành động sẽ được thực hiện khi biểu mẫu được gửi
Vd: <form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
-	Thuộc tính mục tiêu <target>:  chỉ định nơi hiển thị phản hồi nhận được sau khi gửi biểu mẫu (_blank, _self, _parent, _top, framename)
-	Thuộc tính phương thức <method>:Dữ liệu biểu mẫu có thể được gửi dưới dạng biến URL (với method="get") hoặc dưới dạng giao dịch bài đăng HTTP (với method="post")
Vd1: <form action="/action_page.php" method="get">
Vd2: <form action="/action_page.php" method="post">
-	Thuộc tính hoàn thành <autocomplete>: Khi bật tính năng tự động hoàn thành, trình duyệt sẽ tự động hoàn thành các giá trị dựa trên các giá trị mà người dùng đã nhập trước đó
Vd: <form action="/action_page.php" autocomplete="on">
-	Thuộc tính novalidate: Khi xuất hiện, nó chỉ định rằng dữ liệu biểu mẫu (đầu vào) sẽ không được xác thực khi gử
Vd: <form action="/action_page.php" novalidate>
-	Phàn tử <input>: 
Vd: <label for="fname">First name:</label>
<input type="text" id="fname" name="fname">
-	Phần tử <seclect>: Xác định danh sách thả xuống
Vd: <label for="cars">Choose a car:</label>
<select id="cars" name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
-	Phần tử <option>: Xác định một tùy chọn có thể được chọn
Vd: <option value="fiat" selected>Fiat</option>
-	Phần tử <size>: Để chỉ định số lượng giá trị hiển thị
Vd: <label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="3">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
-	Phần tử <multiple>: Để cho phép người dùng chọn nhiều giá trị
Vd: <label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="4" multiple>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
-	Phần tử <textarea>: Xác định trường nhập nhiều dòng (vùng văn bản)
Vd: <textarea name="message" rows="10" cols="30">
The cat was playing in the garden.
</textarea>
-	Phần tử <button>: Xác định một nút có thể nhấp
Vd: <button type="button" onclick="alert('Hello World!')">Click Me!</button>
-	Các phần tử <fieldset> và <legend>:
•	Phần <fieldset>tử được sử dụng để nhóm dữ liệu liên quan trong một biểu mẫu
•	Phần <legend>tử xác định chú thích cho <fieldset> phần tử
Vd: <form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>
-	Phần tử <datalist>: Chỉ định danh sách các tùy chọn được xác định trước cho một <input>phần tử
Vd: <form action="/action_page.php">
  <input list="browsers">
  <datalist id="browsers">
    <option value="Edge">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
</form>
-	Phần tử <ouput>:biểu thị kết quả của một phép tính (giống như kết quả được thực hiện bởi một tập lệnh)
Vd: <form action="/action_page.php"
  oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  0
  <input type="range"  id="a" name="a" value="50">
  100 +
  <input type="number" id="b" name="b" value="50">
  =
  <output name="x" for="a b"></output>
  <br><br>
  <input type="submit">
</form>
-	Các kiểu nhập HTML: <input type="button">
•	<input type="checkbox">
•	<input type="color">
•	<input type="date">
•	<input type="datetime-local">
•	<input type="email">
•	<input type="file">
•	<input type="hidden">
•	<input type="image">
•	<input type="month">
•	<input type="number">
•	<input type="password">
•	<input type="radio">
•	<input type="range">
•	<input type="reset">
•	<input type="search">
•	<input type="submit">
•	<input type="tel">
•	<input type="text">
•	<input type="time">
•	<input type="url">
•	<input type="week">
-	Loại văn bản đầu vào: <input type="text">xác định trường nhập văn bản một dòng
Vd: <form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
-	Mật khẩu đầu vào: <input type="password">xác định trường mật khẩu
Vd: <form>
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="username"><br>
  <label for="pwd">Password:</label><br>
  <input type="password" id="pwd" name="pwd">
</form>
-	Loại đầu vào gửi: <input type="submit">xác định nút để gửi dữ liệu biểu mẫu tới trình xử lý biểu mẫu
Vd: <form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
-	Đặt lại loại đầu vào: <input type="reset">xác định nút đặt lại sẽ đặt lại tất cả các giá trị của biểu mẫu về giá trị mặc định của chúng
Vd: <form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
  <input type="reset" value="Reset">
</form>
-	Phần tử <radio>: Nút radio cho phép người dùng CHỈ chọn MỘT trong số các lựa chọn giới hạn
Vd: <p>Choose your favorite Web language:</p>

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
-	Hộp kiểm tra loại đầu vào: <input type="checkbox">xác định một hộp kiểm, các hộp kiểm cho phép người dùng chọn các tùy chọn KHÔNG hoặc NHIỀU tùy chọn trong một số lựa chọn giới hạn
Vd: <form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form>
-	Nút loại đầu vào: <input type="button">
Vd: <input type="button" onclick="alert('Hello World!')" value="Click Me!">
-	Màu loại đầu vào: <input type="color">
Vd: <form>
  <label for="favcolor">Select your favorite color:</label>
  <input type="color" id="favcolor" name="favcolor">
</form>
-	Loại đầu vào ngày: <input type="date">
Vd1: <form>
  <label for="birthday">Birthday:</label>
  <input type="date" id="birthday" name="birthday">
</form>
Vd2: # Sử dụng  thuộc tính minvà maxđể thêm các hạn chế về ngày tháng
<form>
  <label for="datemax">Enter a date before 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>
  <label for="datemin">Enter a date after 2000-01-01:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02">
</form>
-	Loại đầu vào ngày giờ - cục bộ: <input type="datetime-local">chỉ định trường nhập ngày và giờ, không có múi giờ
Vd: <form>
  <label for="birthdaytime">Birthday (date and time):</label>
  <input type="datetime-local" id="birthdaytime" name="birthdaytime">
</form>
-	Loại đầu vào email: <input type="email">sử dụng cho các trường đầu vào phải chứa địa chỉ email
Vd: <form>
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email">
</form>
-	Loại đầu vào hình ảnh: <input type="image"> xác định một hình ảnh là một nút gửi.
Vd: <form>
<input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
</form>
-	Loại đầu vào tệp: <input type="file"> định trường chọn tệp và nút "Browse" để tải tệp lên
Vd: <form>
  <label for="myfile">Select a file:</label>
  <input type="file" id="myfile" name="myfile">
</form>
-	Loại đầu vào ẩn: <input type="hidden"> xác định trường đầu vào ẩn (không hiển thị cho người dùng)
Vd: <form>
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="hidden" id="custId" name="custId" value="3487">
  <input type="submit" value="Submit">
</form>
-	Loại đầu vào tháng: <input type="month">cho phép người dùng chọn một tháng và năm
Vd: <form>
  <label for="bdaymonth">Birthday (month and year):</label>
  <input type="month" id="bdaymonth" name="bdaymonth">
</form>
-	 Số loại đầu vào: <input type="number">xác định một trường đầu vào số 
Vd: <form>
  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5">
</form>
-	Hạn chế đầu vào: checked, disabled, max, maxlength, min, pattern, readonly, required, size, step, value
Vd: <form>
  <label for="quantity">Quantity:</label>
  <input type="number" id="quantity" name="quantity" min="0" max="100" step="10" value="30">
</form>
-	Phạm vi đầu vào: <input type="range"> một điều khiển để nhập một số có giá trị chính xác không quan trọng (như điều khiển thanh trượt) . Phạm vi mặc định là từ 0 đến 100. Tuy nhiên, bạn có thể đặt giới hạn về số nào được chấp nhận bằng các thuộc tính min, max, và step
Vd: <form>
  <label for="vol">Volume (between 0 and 50):</label>
  <input type="range" id="vol" name="vol" min="0" max="50">
</form>
-	Tìm kiếm loại đầu vào: <input type="search">sử dụng cho các trường tìm kiếm (trường tìm kiếm hoạt động giống như trường văn bản thông thường)
Vd: <form>
  <label for="gsearch">Search Google:</label>
  <input type="search" id="gsearch" name="gsearch">
</form>
-	Loại đầu vào ĐT: <input type="tel">sử dụng cho các trường đầu vào phải chứa số điện thoại
Vd: <form>
  <label for="phone">Enter your phone number:</label>
  <input type="tel" id="phone" name="phone" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
</form>
-	Loại đầu vào thời gian: <input type="time">cho phép người dùng chọn thời gian (không có múi giờ)
Vd: <form>
  <label for="appt">Select a time:</label>
  <input type="time" id="appt" name="appt">
</form>
-	Url loại đầu vào: <input type="url">sử dụng cho các trường đầu vào phải chứa địa chỉ URL
Vd: <form>
  <label for="homepage">Add your homepage:</label>
  <input type="url" id="homepage" name="homepage">
</form>
-	Loại đầu vào tuần: <input type="week">cho phép người dùng chọn một tuần và năm
Vd: <form>
  <label for="week">Select a week:</label>
  <input type="week" id="week" name="week">
</form>
-	Thuộc tính giá trị: <value> chỉ định giá trị ban đầu cho trường đầu vào
Vd: <form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
-	Thuộc tính chỉ đọc: huộc tính đầu vào readonly chỉ định rằng trường đầu vào là chỉ đọc
Vd: <form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John" readonly><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
-	Thuộc tính bị vô hiệu hóa: Thuộc tính đầu vào disabledchỉ định rằng trường đầu vào sẽ bị tắt
Vd: <form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John" disabled><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
-	Thuộc tính đầu vào size chỉ định chiều rộng hiển thị, tính bằng ký tự, của trường đầu vào
Vd: <form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" size="4">
</form>
-	Thuộc tính maxlength: Thuộc tính đầu vào maxlengthchỉ định số lượng ký tự tối đa được phép trong trường đầu vào   
Vd: <form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" maxlength="4" size="4">
</form>
-	Thuộc tính tối thiểu và tối đa: Các thuộc tính minvà maxhoạt động với các loại đầu vào sau: số, phạm vi, ngày, ngày giờ địa phương, tháng, thời gian và tuần
Vd: <form>
  <label for="datemax">Enter a date before 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

  <label for="datemin">Enter a date after 2000-01-01:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>

  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5">
</form>
-	Nhiều thuộc tính:
•	Thuộc tính đầu vào multiplechỉ định rằng người dùng được phép nhập nhiều giá trị vào trường đầu vào
•	Thuộc tính này multiplehoạt động với các loại đầu vào sau: email và tệp
Vd: <form>
  <label for="files">Select files:</label>
  <input type="file" id="files" name="files" multiple>
</form>
-	Thuộc tính mẫu: 
•	Thuộc tính đầu vào pattern chỉ định một biểu thức chính quy mà giá trị của trường đầu vào được kiểm tra khi biểu mẫu được gửi
•	Thuộc tính này pattern hoạt động với các loại đầu vào sau: văn bản, ngày tháng, tìm kiếm, url, số điện thoại, email và mật khẩu
Vd:   <form>
  <label for="country_code">Country code:</label>
  <input type="text" id="country_code" name="country_code"
  pattern="[A-Za-z]{3}" title="Three letter country code">
</form>
-	Thuộc tính giữ chỗ: 
•	Thuộc tính đầu vào placeholder chỉ định một gợi ý ngắn mô tả giá trị mong đợi của trường đầu vào (giá trị mẫu hoặc mô tả ngắn gọn về định dạng dự kiến)
•	Thuộc tính này placeholder hoạt động với các loại đầu vào sau: văn bản, tìm kiếm, url, số, điện thoại, email và mật khẩu
Vd: <form>
  <label for="phone">Enter a phone number:</label>
  <input type="tel" id="phone" name="phone"
  placeholder="123-45-678"
  pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
</form>
-	Thuộc tính bắt buộc: 
•	Thuộc tính đầu vào required chỉ định rằng trường đầu vào phải được điền trước khi gửi biểu mẫu
•	Thuộc tính này required hoạt động với các loại đầu vào sau: văn bản, tìm kiếm, url, số điện thoại, email, mật khẩu, bộ chọn ngày, số, hộp kiểm, radio và tệp
Vd: <form>
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" required>
</form>
-	Thuộc tính bước: Thuộc tính đầu vào stepchỉ định các khoảng số hợp lệ cho trường đầu vào
Vd: <form>
  <label for="points">Points:</label>
  <input type="number" id="points" name="points" step="3">
</form>
-	Thuộc tính tự động lấy nét: Thuộc tính đầu vào autofocuschỉ định rằng trường đầu vào sẽ tự động lấy tiêu điểm khi tải trang
Vd: <form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" autofocus><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
-	Thuộc tính danh sách: Thuộc tính đầu vào listđề cập đến một <datalist>phần tử chứa các tùy chọn được xác định trước cho phần tử <input>
Vd: <form>
  <input list="browsers">
  <datalist id="browsers">
    <option value="Edge">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
</form>
-	Thuộc tính tự động hoàn thành: 
•	Thuộc tính đầu vào autocompletechỉ định xem một biểu mẫu hoặc trường đầu vào có nên bật hay tắt tính năng tự động hoàn thành hay không
•	Thuộc tính này autocompletehoạt động với <form>các loại sau <input>: văn bản, tìm kiếm, url, số điện thoại, email, mật khẩu, bộ chọn ngày, phạm vi và màu sắc
Vd: <form action="/action_page.php" autocomplete="on">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" autocomplete="off"><br><br>
  <input type="submit" value="Submit">
</form>
-	Thuộc tính hình thành: 
•	Thuộc tính đầu vào formaction chỉ định URL của tệp sẽ xử lý đầu vào khi biểu mẫu được gửi
•	Thuộc tính này formactionhoạt động với các loại đầu vào sau: gửi và hình ảnh
Vd: <form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formaction="/action_page2.php" value="Submit as Admin">
</form>
-	Thuộc tính formenctype: 
•	Thuộc tính đầu vào formenctype chỉ định cách mã hóa dữ liệu biểu mẫu khi được gửi (chỉ dành cho các biểu mẫu có phương thức = "post")
•	Thuộc tính này formenctypehoạt động với các loại đầu vào sau: gửi và hình ảnh
Vd: <form action="/action_page_binary.asp" method="post">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formenctype="multipart/form-data"
  value="Submit as Multipart/form-data">
</form>
-	Thuộc tính phương thức biểu mẫu: 
•	Thuộc tính đầu vào formmethod xác định phương thức HTTP để gửi dữ liệu biểu mẫu tới URL hành động
•	Thuộc tính này formmethodhoạt động với các loại đầu vào sau: gửi và hình ảnh
Vd: <form action="/action_page.php" method="get">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit using GET">
  <input type="submit" formmethod="post" value="Submit using POST">
</form>
-	Thuộc tính formtarget: 
•	Thuộc tính đầu vào formtargetchỉ định tên hoặc từ khóa cho biết nơi hiển thị phản hồi nhận được sau khi gửi biểu mẫu
•	Thuộc tính này formtargethoạt động với các loại đầu vào sau: gửi và hình ảnh
Vd: <form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formtarget="_blank" value="Submit to a new window/tab">
</form>
-	Thuộc tính formnovalidate: 
•	Thuộc tính đầu vào formnovalidatechỉ định rằng phần tử <input> không được xác thực khi gử
•	Thuộc tính này formnovalidatehoạt động với các loại đầu vào sau: gửi
Vd: <form action="/action_page.php">
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formnovalidate="formnovalidate"
  value="Submit without validation">
</form>
-	Thuộc tính novalidate: 
Vd: <form action="/action_page.php" novalidate>
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email"><br><br>
  <input type="submit" value="Submit">
</form>
