

I.	CSS Table
1.	Căn chỉnh văn bản
-	Căn chỉnh theo chiều ngang: Thuộc text-aligntính đặt căn chỉnh theo chiều ngang (như trái, phải hoặc giữa) của nội dung trong <th> hoặc <td>
Vd: td {
  text-align: center;
}
-	Căn dọc: Thuộc vertical-aligntính đặt căn chỉnh theo chiều dọc (như trên, dưới hoặc giữa) của nội dung trong <th> hoặc <td>
Vd: td {
  height: 50px;
  vertical-align: bottom;
}
2.	Kiểu bản CSS
-	Bộ chia ngang: hêm border-bottomthuộc tính vào <th> và <td> cho dải phân cách ngang
Vd: th, td {
  border-bottom: 1px solid #ddd;
}
-	Bảng di chuột: Sử dụng :hoverbộ chọn trên <tr> để đánh dấu các hàng trong bảng khi di chuột qua
Vd: tr:hover {background-color: coral;}
3.	Bảng đáp ứng: Thêm phần tử vùng chứa (như <div>) xung overflow-x:autoquanh phần tử <table> để làm cho phần tử này phản hồi
Vd: <style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {background-color: #f2f2f2;}
</style>
</head>
<body>

<h2>Responsive Table</h2>
<p>A responsive table will display a horizontal scroll bar if the screen is too 
small to display the full content. Resize the browser window to see the effect:</p>
<p>To create a responsive table, add a container element (like div) with <strong>overflow-x:auto</strong> around the table element:</p>

<div style="overflow-x: auto;">
  <table>
    <tr>
      <th>First Name</th>
      <th>Last Name</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
    </tr>
    <tr>
      <td>Jill</td>
      <td>Smith</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
    </tr>
    <tr>
      <td>Eve</td>
      <td>Jackson</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
    </tr>
    <tr>
      <td>Adam</td>
      <td>Johnson</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
    </tr>
  </table>
</div>
II.	Hiển thị CSS
-	Thuộc tính hiển thị: Thuộc displaytính được sử dụng để chỉ định cách hiển thị một phần tử trên trang web
-	Các phần tử cấp khối: 
Vd1: span {
  display: block;
}
Vd2: a {
  display: block;
}
-	Ẩn một phàn tử - hiển thị
Vd: <!DOCTYPE html>
<html>
<head>
<style>
h1.hidden {
  display: none;
}
</style>
</head>
<body>

<h1>This is a visible heading</h1>
<h1 class="hidden">This is a hidden heading</h1>
<p>Notice that the h1 element with display: none; does not take up any space.</p>

</body>
</html>
III.	Thuộc tính vị trí
1.	Vị trí tài sản
-	Thuộc positiontính chỉ định loại phương pháp định vị được sử dụng cho một phần tử
2.	Vị trí tĩnh
-	Một phần tử position: static;không được định vị theo bất kỳ cách đặc biệt nào; nó luôn được định vị theo luồng thông thường của trang
Vd: div.static {
  position: static;
  border: 3px solid #73AD21;
}
3.	Vị trí tương đối
-	Một phần tử with position: relative;được định vị so với vị trí bình thường của nó
Vd: div.relative {
  position: relative;
  left: 30px;
  border: 3px solid #73AD21;
}
4.	Vị trí cố định:
-	Một phần tử position: fixed;được định vị tương ứng với khung nhìn, có nghĩa là nó luôn ở cùng một vị trí ngay cả khi trang được cuộn
Vd: div.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 300px;
  border: 3px solid #73AD21;
}
5.	Vị trí tuyệt đối
-	Một phần tử position: absolute;được định vị tương đối so với tổ tiên được định vị gần nhất (thay vì được định vị tương đối với khung nhìn, như cố định)
Vd: div.relative {
  position: relative;
  width: 400px;
  height: 200px;
  border: 3px solid #73AD21;
}

div.absolute {
  position: absolute;
  top: 80px;
  right: 0;
  width: 200px;
  height: 100px;
  border: 3px solid #73AD21;
}
6.	Vị trí dính
-	Một phần tử position: sticky;được định vị dựa trên vị trí cuộn của người dùng
-	Phần tử cố định chuyển đổi giữa relativevà fixed, tùy thuộc vào vị trí cuộn.
Vd: div.sticky {
  position: -webkit-sticky; /* Safari */
  position: sticky;
  top: 0;
  background-color: green;
  border: 2px solid #4CAF50;
}
IV.	Độ mờ / Độ trong suốt của CSS
1.	Hình ảnh trong suốt
-	Thuộc opacitytính có thể nhận giá trị từ 0,0 - 1,0
Vd: img {
  opacity: 0.5;
}
2.	Hiệu ứng di chuyển chột trong suốt
-	Thuộc tính này opacitythường được sử dụng cùng với :hover bộ chọn để thay đổi độ mờ khi di chuột qua
Thuộc tính này opacitythường được sử dụng cùng với :hover bộ chọn để thay đổi độ mờ khi di chuột qua
Vd: img {
  opacity: 0.5;
}

img:hover {
  opacity: 1.0;
}
3.	Độ trong suốt bằng RGBA
Vd: div {
  background: rgba(76, 175, 80, 0.3) /* Green background with 30% opacity */
}
4.	Văn bản trong hộp trong suốt
Vd: <html>
<head>
<style>
div.background {
  background: url(klematis.jpg) repeat;
  border: 2px solid black;
}

div.transbox {
  margin: 30px;
  background-color: #ffffff;
  border: 1px solid black;
  opacity: 0.6;
}

div.transbox p {
  margin: 5%;
  font-weight: bold;
  color: #000000;
}
</style>
</head>
<body>

<div class="background">
  <div class="transbox">
    <p>This is some text that is placed in the transparent box.</p>
  </div>
</div>

</body>
</html>
V.	Thanh điều hướng CSS
-	Thanh điều hướng = Danh sách liên kết
Vd: <!DOCTYPE html>
<html>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<p>Note: We use href="#" for test links. In a real web site this would be URLs.</p>

</body>
</html>
-	Thanh điều hướng dọc: 
Vd1: li a {
  display: block;
  width: 60px;
}
Vd2: ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #f1f1f1;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

/* Change the link color on hover */
li a:hover {
  background-color: #555;
  color: white;
}
-	Liên kết điều hướng hiện tại/đang hoạt động: 
Vd: ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #f1f1f1;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

/* Change the link color on hover */
li a:hover {
  background-color: #555;
  color: white;
}
-	Liên kết trung tâm và thêm đường viền: 
•	Thêm text-align:centervào <li> hoặc <a> để căn giữa các liên kết
•	Thêm borderthuộc tính để <ul> thêm đường viền xung quanh thanh điều hướng
•	thêm a border-bottomvào tất cả các phần tử <li>, ngoại trừ phần tử cuối cùng
Vd: <!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #f1f1f1;
  border: 1px solid #555;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

li {
  text-align: center;
  border-bottom: 1px solid #555;
}

li:last-child {
  border-bottom: none;
}

li a.active {
  background-color: #04AA6D;
  color: white;
}

li a:hover:not(.active) {
  background-color: #555;
  color: white;
}
</style>
</head>
<body>

<h2>Vertical Navigation Bar</h2>
<p>In this example, we center the navigation links and add a border to the navigation bar.</p>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
-	Thanh điều hướng dọc cố định có chiều cao đầy đủ: 
Vd: <!DOCTYPE html>
<html>
<head>
<style>
body {
  margin: 0;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 25%;
  background-color: #f1f1f1;
  position: fixed;
  height: 100%;
  overflow: auto;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

li a.active {
  background-color: #04AA6D;
  color: white;
}

li a:hover:not(.active) {
  background-color: #555;
  color: white;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<div style="margin-left:25%;padding:1px 16px;height:1000px;">
  <h2>Fixed Full-height Side Nav</h2>
  <h3>Try to scroll this area, and see how the sidenav sticks to the page</h3>
  <p>Notice that this div element has a left margin of 25%. This is because the side navigation is set to 25% width. If you remove the margin, the sidenav will overlay/sit on top of this div.</p>
  <p>Also notice that we have set overflow:auto to sidenav. This will add a scrollbar when the sidenav is too long (for example if it has over 50 links inside of it).</p>
  <p>Some text..</p>
  <p>Some text..</p>
  <p>Some text..</p>
  <p>Some text..</p>
  <p>Some text..</p>
  <p>Some text..</p>
  <p>Some text..</p>
</div>

</body>
</html>
-	Thanh điều hướng ngang – Danh sách nổi:
Vd: <!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
}

li {
  float: left;
}

li a {
  display: block;
  padding: 8px;
  background-color: #dddddd;
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

<p><b>Note:</b> If a !DOCTYPE is not specified, floating items can produce unexpected results.</p>
<p>A background color is added to the links to show the link area. The whole link area is clickable, not just the text.</p>
<p><b>Note:</b> overflow:hidden is added to the ul element to prevent li elements from going outside of the list.</p>

</body>
</html>
-	Vd về thanh điều hướng ngang:
Vd: <!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
-	Liên kết ngang hướng hiện tại/đang hoạt động
Vd: <!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #111;
}

.active {
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
-	Liên kết căn phải: 
<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #111;
}

.active {
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li style="float:right"><a class="active" href="#about">About</a></li>
</ul>

</body>
</html>
-	Dải phân cách biên giới: Thêm thuộc border-righttính vào <li> để tạo bộ chia liên kết
Vd: <!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
  border-right:1px solid #bbb;
}

li:last-child {
  border-right: none;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #111;
}

.active {
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li style="float:right"><a href="#about">About</a></li>
</ul>

</body>
</html>
-	Thanh điều hướng cố định: 
Vd: # Cố định hàng đầu
ul {
  position: fixed;
  top: 0;
  width: 100%;
}
		Vd: # Đáy cố định
ul {
  position: fixed;
  bottom: 0;
  width: 100%;
}
-	Thanh điều hướng ngang màu xám: 
Vd: <!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  border: 1px solid #e7e7e7;
  background-color: #f3f3f3;
}

li {
  float: left;
}

li a {
  display: block;
  color: #666;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #ddd;
}

li a.active {
  color: white;
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
-	Thanh điều hướng dính: Thêm position: sticky;vào <ul> để tạo thanh điều hướng cố định
Vd: ul {
  position: -webkit-sticky; /* Safari */
  position: sticky;
  top: 0;
}
-	Thanh điều hướng thả xuống:
Vd: <!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color:white;
}
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #38444d;
}

li {
  float: left;
}

li a, .dropbtn {
  display: inline-block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover, .dropdown:hover .dropbtn {
  background-color: red;
}

li.dropdown {
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {background-color: #f1f1f1;}

.dropdown:hover .dropdown-content {
  display: block;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li class="dropdown">
    <a href="javascript:void(0)" class="dropbtn">Dropdown</a>
    <div class="dropdown-content">
      <a href="#">Link 1</a>
      <a href="#">Link 2</a>
      <a href="#">Link 3</a>
    </div>
  </li>
</ul>

<h3>Dropdown Menu inside a Navigation Bar</h3>
<p>Hover over the "Dropdown" link to see the dropdown menu.</p>

</body>
</html>
-	Thanh thả xuống cơ bản:
Vd: <style>
.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  padding: 12px 16px;
  z-index: 1;
}

.dropdown:hover .dropdown-content {
  display: block;
}
</style>

<div class="dropdown">
  <span>Mouse over me</span>
  <div class="dropdown-content">
    <p>Hello World!</p>
  </div>
</div>
-	Trình thả xuống đơn: 
Vd: <style>
/* Style The Dropdown Button */
.dropbtn {
  background-color: #4CAF50;
  color: white;
  padding: 16px;
  font-size: 16px;
  border: none;
  cursor: pointer;
}

/* The container <div> - needed to position the dropdown content */
.dropdown {
  position: relative;
  display: inline-block;
}

/* Dropdown Content (Hidden by Default) */
.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

/* Links inside the dropdown */
.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

/* Change color of dropdown links on hover */
.dropdown-content a:hover {background-color: #f1f1f1}

/* Show the dropdown menu on hover */
.dropdown:hover .dropdown-content {
  display: block;
}

/* Change the background color of the dropdown button when the dropdown content is shown */
.dropdown:hover .dropbtn {
  background-color: #3e8e41;
}
</style>

<div class="dropdown">
  <button class="dropbtn">Dropdown</button>
  <div class="dropdown-content">
    <a href="#">Link 1</a>
    <a href="#">Link 2</a>
    <a href="#">Link 3</a>
  </div>
</div>
-	Nội dung thả xuống được căn phải:
Vd: .dropdown-content {
  right: 0;
}




















