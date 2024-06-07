Báo cáo lập trình môn javascript – ngày 4
I.	Khung nội tuyến HTML
-	Cú pháp: Thẻ HTML <iframe> chỉ định khung nội tuyến
Vd: <iframe src="url" title="description"></iframe>
-	Iframe – Đặt chiều cao và chiều rộng: Sử dụng các thuộc tính height và width để chỉ định kích thước của iframe
Vd: <iframe src="demo_iframe.htm" height="200" width="300" title="Iframe Example"></iframe
-	Xóa đường viền: border
Vd: <iframe src="demo_iframe.htm" style="border:none;" title="Iframe Example"></iframe>
-	Mục tiêu cho liên kết: Vd:<iframe src="demo_iframe.htm" name="iframe_a" title="Iframe Example"></iframe>

<p><a href="https://www.w3schools.com" target="iframe_a">W3Schools.com</a></p>
II.	HTML JavaScript
III.	Color
1.	Màu RGB
-	Thông số: rgb(red, green, blue)
Vd: <h2 style="background-color:rgb(255, 0, 0);">rgb(255, 0, 0)</h2>
<h2 style="background-color:rgb(0, 0, 255);">rgb(0, 0, 255)</h2>
<h2 style="background-color:rgb(60, 179, 113);">rgb(60, 179, 113)</h2>
<h2 style="background-color:rgb(238, 130, 238);">rgb(238, 130, 238)</h2>
<h2 style="background-color:rgb(255, 165, 0);">rgb(255, 165, 0)</h2>
<h2 style="background-color:rgb(106, 90, 205);">rgb(106, 90, 205)</h2>
2.	Màu RGBA
-	Thông số: rgba(red, green, blue, alpha)
3.	Màu HEX:
-	#rrggbb: Trong đó rr (đỏ), gg (xanh lục) và bb (xanh lam) là các giá trị thập lục phân từ 00 đến ff (giống như số thập phân 0-255)
Vd: <h2 style="background-color:#ff0000;">#ff0000</h2>
<h2 style="background-color:#0000ff;">#0000ff</h2>
<h2 style="background-color:#3cb371;">#3cb371</h2>
<h2 style="background-color:#ee82ee;">#ee82ee</h2>
<h2 style="background-color:#ffa500;">#ffa500</h2>
<h2 style="background-color:#6a5acd;">#6a5acd</h2>
-	Giá trị HEX 3 chữ số: # rgb Trong đó r, g và b đại diện cho các thành phần màu đỏ, xanh lục và xanh lam có giá trị từ 0 đến f
4.	Màu HSL
-	Màu HSL: hsl(hue, saturation, lightness)
•	Hue là một độ trên bánh xe màu từ 0 đến 360. 0 là đỏ, 120 là xanh lục và 240 là xanh lam
•	Saturation:  0% có nghĩa là màu xám và 100% là màu đầy đủ
•	Lightness: 0% là màu đen, 50% không sáng cũng không tối, 100% là màu trắng
-	Màu HSLA: Là phần mở rộng của giá trị màu HSL với kênh alpha - kênh này chỉ định độ mờ cho màu
IV.	Nền CSS
1.	Độ mờ/ Độ trong suốt
-	Thuộc opacitytính chỉ định độ mờ/độ trong suốt của một phần tử. Nó có thể nhận giá trị từ 0,0 - 1,0
Vd: div {
  background-color: green;
  opacity: 0.3;
}
-	Độ trong suốt bằng RGBA:  rgba(red, green, blue, alpha )
Vd: div {
  background: rgba(0, 128, 0, 0.3) /* Green background with 30% opacity */
}
2.	Hình nền CSS
-	background-image: chỉ định một hình ảnh để sử dụng làm nền của một phần tử
Vd: body {
  background-image: url("paper.gif");
}
-	Lặp lại nền CSS theo chiều ngang: background-repeat: repeat-x;
Vd: body {
  background-image: url("gradient_bg.png");
  background-repeat: repeat-x;
}
-	Không lặp lại: Chỉ hiển thị hình nền một lần cũng được chỉ định bởi background-repeat thuộc tính
Vd: body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
}
-	Vị trí nền CSS: background-position được sử dụng để xác định vị trí của hình nền
Vd: body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}
3.	Tệp đính kèm nền CSS
-	Đính kèm nền CSS: background-attachment chỉ định xem hình nền sẽ cuộn hay được cố định 
Vd: body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: fixed;
}
4.	Viết tắt nền CSS
-	Nền CSS – Thuộc tính viết tắt: Để rút ngắn mã, cũng có thể chỉ định tất cả các thuộc tính nền trong một thuộc tính duy nhất
Vd: body {
  background: #ffffff url("img_tree.png") no-repeat right top;
}
V.	Đường viền CSS 
1.	Thuộc border-styletính chỉ định loại đường viền sẽ hiển thị:
-	dotted- Xác định đường viền chấm
-	dashed- Xác định đường viền nét đứt
-	solid- Xác định một đường viền vững chắc
-	double- Xác định đường viền kép
-	groove- Xác định đường viền có rãnh 3D. Hiệu ứng phụ thuộc vào giá trị màu đường viền
-	ridge- Xác định đường viền có gờ 3D. Hiệu ứng phụ thuộc vào giá trị màu đường viền
-	inset- Xác định đường viền chèn 3D. Hiệu ứng phụ thuộc vào giá trị màu đường viền
-	outset- Xác định đường viền đầu 3D. Hiệu ứng phụ thuộc vào giá trị màu đường viền
-	none- Xác định không có đường viền
-	hidden- Xác định đường viền ẩn
Vd: p.dotted {border-style: dotted;}
p.dashed {border-style: dashed;}
p.solid {border-style: solid;}
p.double {border-style: double;}
p.groove {border-style: groove;}
p.ridge {border-style: ridge;}
p.inset {border-style: inset;}
p.outset {border-style: outset;}
p.none {border-style: none;}
p.hidden {border-style: hidden;}
p.mix {border-style: dotted dashed solid double;}
2.	Chiều rộng đường viền CSS
-	Chiều rộng đường viền:  chỉ định chiều rộng của bốn đường viền
Vd: p.one {
  border-style: solid;
  border-width: 5px;
}

p.two {
  border-style: solid;
  border-width: medium;
}

p.three {
  border-style: dotted;
  border-width: 2px;
}

p.four {
  border-style: dotted;
  border-width: thick;
}
-	Các mặt riêng lẻ
Vd: p {
  border-top-style: dotted;
  border-right-style: solid;
  border-bottom-style: dotted;
  border-left-style: solid;
}
3.	Thuộc tính đường viền viết tắt CSS
-	Thuộc tính viết tắt:
Vd: p {
  border: 5px solid red;
}
p {
  border-left: 6px solid red;
}
p {
  border-bottom: 6px solid red;
}
4.	Đường viền tròn CSS
-	border-radius:  sử dụng để thêm đường viền tròn cho một phần tử
Vd: p {
  border: 2px solid red;
  border-radius: 5px;
}
VI.	Lề
-	Các mặt riêng lẻ:
•	margin-top
•	margin-right
•	margin-bottom
•	margin-left
Vd: p {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}
-	Thuộc tính viết tắt:
Vd1: p {
  margin: 25px 50px 75px 100px;
}
# Lề: 25px 50px 75px 100px;
o	lề trên là 25px
o	lề phải là 50px
o	lề dưới là 75px
o	lề trái là 100px
Vd2: p {
  margin: 25px 50px 75px;
}
# Lề: 25px 50px 75px;
o	lề trên là 25px
o	lề phải và trái là 50px
o	lề dưới là 75px
Vd3: p {
  margin: 25px 50px;
}
# lề: 25px 50px;
o	lề trên và dưới là 25px
o	lề phải và trái là 50px
Vd4: p {
  margin: 25px;
}
# lề: 25px;
o	tất cả bốn lề đều là 25px
-	Giá trị tự động: auto
Vd: div {
  width: 300px;
  margin: auto;
  border: 1px solid red;
}
-	Giá trị thừa kế: 
Vd: div {
  border: 1px solid red;
  margin-left: 100px;
}

p.ex1 {
  margin-left: inherit;
}
-	Thu gọn lề: 
Vd: h1 {
  margin: 0 0 50px 0;
}

h2 {
  margin: 20px 0 0 0;
}
VII.	Tóm tắt CSS
1.	Kiểu phác thảo CSS
-	dotted- Xác định một đường viền chấm
-	dashed- Xác định đường viền nét đứt
-	solid- Xác định một phác thảo vững chắc
-	double- Xác định một phác thảo kép
-	groove- Xác định đường viền có rãnh 3D
-	ridge- Xác định đường viền có gờ 3D
-	inset- Xác định một phác thảo nội dung 3D
-	outset- Xác định một phác thảo đầu 3D
-	none- Xác định không có phác thảo
-	hidden- Xác định một phác thảo ẩn
Vd: p.dotted {outline-style: dotted;}
p.dashed {outline-style: dashed;}
p.solid {outline-style: solid;}
p.double {outline-style: double;}
p.groove {outline-style: groove;}
p.ridge {outline-style: ridge;}
p.inset {outline-style: inset;}
p.outset {outline-style: outset;}
2.	Chiều rộng phác thảo CSS
Vd: p.ex1 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: thin;
}

p.ex2 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: medium;
}

p.ex3 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: thick;
}

p.ex4 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: 4px;
}
3.	Màu đường viền CSS
-	Màu đường viền CSS
Vd: p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: red;
}

p.ex2 {
  border: 2px solid black;
  outline-style: dotted;
  outline-color: blue;
}

p.ex3 {
  border: 2px solid black;
  outline-style: outset;
  outline-color: grey;
}
-	Giá trị HEX: 
Vd:p.ex1 {
  outline-style: solid;
  outline-color: #ff0000; /* red */
}
-	Giá trị RGB:
Vd: p.ex1 {
  outline-style: solid;
  outline-color: rgb(255, 0, 0); /* red */
}
-	Giá trị HSL:
Vd: p.ex1 {
  outline-style: solid;
  outline-color: hsl(0, 100%, 50%); /* red */
}
-	Tóm tắt CSS
Vd: <!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {outline: dashed;}
p.ex2 {outline: dotted red;}
p.ex3 {outline: 5px solid yellow;}
p.ex4 {outline: thick ridge pink;}
</style>
</head>
<body>

<h2>The outline Property</h2>

<p class="ex1">A dashed outline.</p>
<p class="ex2">A dotted red outline.</p>
<p class="ex3">A 5px solid yellow outline.</p>
<p class="ex4">A thick ridge pink outline.</p>

</body>
</html>
-	Phần bù phác thảo CSS: Thuộc outline-offsettính thêm khoảng trống giữa đường viền và cạnh/viền của một phần tử. Khoảng cách giữa một phần tử và đường viền của nó là trong suốt
Vd: p {
  margin: 30px;
  border: 1px solid black;
  outline: 1px solid red;
  outline-offset: 15px;
}
4.	Văn bản
-	Căn chỉnh văn bản: Thuộc text-aligntính được sử dụng để thiết lập căn chỉnh theo chiều ngang của văn bản
Vd: h1 {
  text-align: center;
}

h2 {
  text-align: left;
}

h3 {
  text-align: right;
}
-	Căn bản văn bản cuối cùng: Thuộc text-align-lasttính chỉ định cách căn chỉnh dòng cuối cùng của văn bản
Vd: p.a {
  text-align-last: right;
}

p.b {
  text-align-last: center;
}

p.c {
  text-align-last: justify;
}
-	Văn bản chỉ đạo: Các thuộc tính directionvà unicode-bidicó thể được sử dụng để thay đổi hướng văn bản của một phần tử
Vd: p {
  direction: rtl;
  unicode-bidi: bidi-override;
}
-	Căn dọc: Thuộc vertical-aligntính thiết lập căn chỉnh theo chiều dọc của một phần tử
Vd: img.a {
  vertical-align: baseline;
}

img.b {
  vertical-align: text-top;
}

img.c {
  vertical-align: text-bottom;
}

img.d {
  vertical-align: sub;
}

img.e {
  vertical-align: super;
}
-	Thêm dòng trang trí vào văn bản: Thuộc text-decoration-linetính được sử dụng để thêm dòng trang trí vào văn bản
Vd: h1 {
  text-decoration-line: overline;
}

h2 {
  text-decoration-line: line-through;
}

h3 {
  text-decoration-line: underline;
}

p {
  text-decoration-line: overline underline;
}
-	Chỉ định màu cho đường trang trí: Thuộc tính này text-decoration-colorđược sử dụng để thiết lập màu của đường trang trí
Vd: h1 {
  text-decoration-line: overline;
  text-decoration-color: red;
}

h2 {
  text-decoration-line: line-through;
  text-decoration-color: blue;
}

h3 {
  text-decoration-line: underline;
  text-decoration-color: green;
}

p {
  text-decoration-line: overline underline;
  text-decoration-color: purple;
}
-	Chỉ định kiểu cho đường trang trí: Thuộc tính này text-decoration-styleđược sử dụng để thiết lập kiểu dáng của đường trang trí
Vd: 	h1 {
  text-decoration-line: underline;
  text-decoration-style: solid;
}

h2 {
  text-decoration-line: underline;
  text-decoration-style: double;
}

h3 {
  text-decoration-line: underline;
  text-decoration-style: dotted;
}

p.ex1 {
  text-decoration-line: underline;
  text-decoration-style: dashed;
}

p.ex2 {
  text-decoration-line: underline;
  text-decoration-style: wavy;
}

p.ex3 {
  text-decoration-line: underline;
  text-decoration-color: red;
  text-decoration-style: wavy;
}
-	Chỉ định độ dày cho đường trang trí: Thuộc text-decoration-thicknesstính được sử dụng để thiết lập độ dày của đường trang trí
Vd: h1 {
  text-decoration-line: underline;
  text-decoration-thickness: auto;
}

h2 {
  text-decoration-line: underline;
  text-decoration-thickness: 5px;
}

h3 {
  text-decoration-line: underline;
  text-decoration-thickness: 25%;
}

p {
  text-decoration-line: underline;
  text-decoration-color: red;
  text-decoration-style: double;
  text-decoration-thickness: 5px;
}
-	Thuộc tính viết tắt:Thuộc text-decorationtính là một thuộc tính viết tắt 
•	text-decoration-line(yêu cầu)
•	text-decoration-color(không bắt buộc)
•	text-decoration-style(không bắt buộc)
•	text-decoration-thickness(không bắt buộc)
Vd: h1 {
  text-decoration: underline;
}

h2 {
  text-decoration: underline red;
}

h3 {
  text-decoration: underline red double;
}

p {
  text-decoration: underline red double 5px;
}
-	Mẹo nhỏ: text-decoration: none sử dụng để xóa phần gạch chân khỏi các liên kết, như thế này
Vd: a {
  text-decoration: none;
}
-	Chuyển đổi văn bản: Thuộc text-transformtính được sử dụng để chỉ định chữ hoa và chữ thường trong văn bản
Vd: p.uppercase {
  text-transform: uppercase;
}

p.lowercase {
  text-transform: lowercase;
}

p.capitalize {
  text-transform: capitalize;
}
-	Khoảng cách văn bản: 
•	text-indent
•	letter-spacing
•	line-height
•	word-spacing
•	white-space
-	Thụt lề văn bản: Thuộc text-indenttính được sử dụng để xác định mức thụt dòng của dòng đầu tiên trong văn bản
Vd: p {
  text-indent: 50px;
}
-	Khoảng cáh chữ: Thuộc letter-spacingtính được sử dụng để chỉ định khoảng cách giữa các ký tự trong văn bản
Vd: h1 {
  letter-spacing: 5px;
}

h2 {
  letter-spacing: -2px;
}
-	Chiều cao giữa các dòng: Thuộc line-heighttính được sử dụng để chỉ định khoảng cách giữa các dòng
Vd: p.small {
  line-height: 0.8;
}

p.big {
  line-height: 1.8;
}
-	Khoảng cách từ: Thuộc word-spacingtính được sử dụng để chỉ định khoảng cách giữa các từ trong văn bản
Vd: p.one {
  word-spacing: 10px;
}

p.two {
  word-spacing: -2px;
}
-	Khoảng trắng: Thuộc white-spacetính chỉ định cách xử lý khoảng trắng bên trong một phần tử
Vd: p {
  white-space: nowrap;
}
-	Bóng văn bản: Thuộc text-shadow tính thêm bóng vào văn bản
Vd: h1 {
  text-shadow: 2px 2px;
}
# Tiếp theo, thêm màu (đỏ) cho bóng
h1 {
  text-shadow: 2px 2px red;
}
# Sau đó, thêm hiệu ứng làm mờ (5px) cho bóng
h1 {
  text-shadow: 2px 2px 5px red;
}
5.	Phông chữ CSS
-	Họ phông chữ chung
•	Serif: có một nét nhỏ ở rìa mỗi chữ cái. Chúng tạo cảm giác trang trọng và sang trọng
•	Sans-serif: có đường nét rõ ràng (không có nét nhỏ kèm theo). Chúng tạo ra một cái nhìn hiện đại và tối giản.
•	Monospace: ở đây tất cả các chữ cái đều có cùng chiều rộng cố định. Họ tạo ra một cái nhìn máy móc.
•	Cursive: bắt chước chữ viết tay của con người.
•	Fantasy:  là phông chữ trang trí/vui tươi.
-	Thuộc tính họ phông chữ CSS: Trong CSS, chúng ta sử dụng font-familythuộc tính để chỉ định phông chữ của văn bản
Vd: .p1 {
  font-family: "Times New Roman", Times, serif;
}

.p2 {
  font-family: Arial, Helvetica, sans-serif;
}

.p3 {
  font-family: "Lucida Console", "Courier New", monospace;
}
-	Phông chữ dự phòng: 
Vd: p {
font-family: Tahoma, Verdana, sans-serif;
}
# Ở đây, có ba loại phông chữ: Tahoma, Verdana và sans-serif. Phông chữ thứ hai và thứ ba là bản sao lưu, trong trường hợp không tìm thấy phông chữ đầu tiên.
-	Phông chữ an toàn trên web tốt nhất cho HTML và CSS: 
•	Arial (sans-serif)
•	Verdana (sans-serif)
•	Tahoma (sans-serif)
•	Trebuchet MS (sans-serif)
•	Times New Roman (có chân)
•	Georgia (chân)
•	Garamond (chân)
•	Chuyển phát nhanh mới (monospace)
•	Brush Script MT (chữ thảo)
-	Kiểu phông chữ: font-style (normal, italic, oblique)
Vd: p.normal {
  font-style: normal;
}

p.italic {
  font-style: italic;
}

p.oblique {
  font-style: oblique;
}
-	Trọng lượng phông chữ: Thuộc font-weighttính chỉ định trọng lượng của phông chữ
Vd: p.normal {
  font-weight: normal;
}

p.thick {
  font-weight: bold;
}
-	Biến thể phông chữ: Thuộc font-varianttính chỉ định liệu văn bản có được hiển thị bằng phông chữ viết hoa nhỏ hay không
Vd: p.normal {
  font-variant: normal;
}

p.small {
  font-variant: small-caps;
}
-	Cỡ chữ: Thuộc font-sizetính thiết lập kích thước của văn bản
-	Đặt cỡ chữ bằng pixel: Đặt kích thước văn bản bằng pixel cho phép bạn kiểm soát hoàn toàn kích thước văn bản
Vd: h1 {
  font-size: 40px;
}

h2 {
  font-size: 30px;
}

p {
  font-size: 14px;
}
-	Đặt cỡ chữ bằng Em: ích thước mặc định của 1em là 16px
Vd: h1 {
  font-size: 2.5em; /* 40px/16=2.5em */
}

h2 {
  font-size: 1.875em; /* 30px/16=1.875em */
}

p {
  font-size: 0.875em; /* 14px/16=0.875em */
}
-	Kích thước phông chữ đáp ứng:  Kích thước văn bản có thể được đặt bằng một vwđơn vị, có nghĩa là "chiều rộng khung nhìn"
Vd: <h1 style="font-size:10vw">Hello World</h1>
-	Cách sử dụng phông chữ của Google: Chỉ cần thêm một liên kết biểu định kiểu đặc biệt vào phần <head> rồi tham khảo phông chữ trong CSS
Vd: Ở đây, chúng tôi muốn sử dụng phông chữ có tên "Sofia" từ Google Fonts:
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<style>
body {
  font-family: "Sofia", sans-serif;
}
</style>
</head>
Ở đây, chúng tôi muốn sử dụng phông chữ có tên "Trirong"từ Google Fonts:
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Trirong">
<style>
body {
  font-family: "Trirong", serif;
}
</style>
</head>
Ở đây, chúng tôi muốn sử dụng phông chữ có tên "Audiowide" từ Google Fonts:
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide">
<style>
body {
  font-family: "Audiowide", sans-serif;
}
</style>
</head>
-	Sử dụng nhiều phông chữ của Google: Để sử dụng nhiều phông chữ của Google, chỉ cần phân tách tên phông chữ bằng ký tự ống dẫn ( |), như thế này
Vd: <head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide|Sofia|Trirong">
<style>
h1.a {font-family: "Audiowide", sans-serif;}
h1.b {font-family: "Sofia", sans-serif;}
h1.c {font-family: "Trirong", serif;}
</style>
</head>
-	Tạo kiểu cho phông chữ Google: 
Vd: Tạo kiểu cho phông chữ "Sofia":
	<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<style>
body {
  font-family: "Sofia", sans-serif;
  font-size: 30px;
  text-shadow: 3px 3px 3px #ababab;
}
</style>
</head>
-	Kích hoạt hiệu ứng phông chữ: 
Vd:# Thêm hiệu ứng lửa vào phông chữ "Sofia"
	<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=fire">
<style>
body {
  font-family: "Sofia", sans-serif;
  font-size: 30px;
}
</style>
</head>
<body>

<h1 class="font-effect-fire">Sofia on Fire</h1>

</body>
	# Thêm nhiều hiệu ứng cho phông chữ "Sofia":
	<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=neon|outline|emboss|shadow-multiple">
<style>
body {
  font-family: "Sofia", sans-serif;
  font-size: 30px;
}
</style>
</head>
<body>

<h1 class="font-effect-neon">Neon Effect</h1>
<h1 class="font-effect-outline">Outline Effect</h1>
<h1 class="font-effect-emboss">Emboss Effect</h1>
<h1 class="font-effect-shadow-multiple">Multiple Shadow Effect</h1>

</body>
6.	Biểu tượng CSS
-	Cách thêm biểu tượng: 
•	Cách đơn giản nhất để thêm biểu tượng vào trang HTML của bạn là sử dụng thư viện biểu tượng, chẳng hạn như Font Awesome
•	Thêm tên của lớp biểu tượng được chỉ định vào bất kỳ phần tử HTML nội tuyến nào (như <i>hoặc <span>)
-	Phông chữ biểu tượng tuyệt vời:Để sử dụng các biểu tượng Font Awesome, hãy truy cập fontawgie.com , đăng nhập và nhận mã để thêm vào <head>phần trang HTML  <script src="https://kit.fontawesome.com/yourcode.js"crossorigin="anonymous"></script>
Vd: <!DOCTYPE html>
<html>
<head>
<script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
</head>
<body>

<i class="fas fa-cloud"></i>
<i class="fas fa-heart"></i>
<i class="fas fa-car"></i>
<i class="fas fa-file"></i>
<i class="fas fa-bars"></i>
</body>
</html>
-	Biểu tượng Bootstrap: Để sử dụng glyphicons Bootstrap, hãy thêm dòng sau vào bên trong <head>phần trang HTML <link rel="stylesheet"href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
Vd: <!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
</head>
<body>

<i class="glyphicon glyphicon-cloud"></i>
<i class="glyphicon glyphicon-remove"></i>
<i class="glyphicon glyphicon-user"></i>
<i class="glyphicon glyphicon-envelope"></i>
<i class="glyphicon glyphicon-thumbs-up"></i>

</body>
</html>
-	Biểu tượng google: Để sử dụng các biểu tượng Google, hãy thêm dòng sau vào bên trong <head>phần trang HTML  <link rel="stylesheet"href="https://fonts.googleapis.com/icon?family=Material+Icons">
Vd: <!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
</head>
<body>

<i class="material-icons">cloud</i>
<i class="material-icons">favorite</i>
<i class="material-icons">attachment</i>
<i class="material-icons">computer</i>
<i class="material-icons">traffic</i>

</body>
</html>
-	Liên kết CSS: 
•	a:link- một liên kết bình thường, chưa được truy cập
•	a:visited- một liên kết người dùng đã truy cập
•	a:hover- một liên kết khi người dùng di chuột qua nó
•	a:active- một liên kết ngay khi nó được nhấp vào
Vd: 
<!DOCTYPE html>
<html>
<head>
<style>
/* unvisited link */
a:link {
  color: red;
}

/* visited link */
a:visited {
  color: green;
}

/* mouse over link */
a:hover {
  color: hotpink;
}

/* selected link */
a:active {
  color: blue;
}
</style>
</head>
<body>

<h2>Styling a link depending on state</h2>

<p><b><a href="default.asp" target="_blank">This is a link</a></b></p>
<p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be effective.</p>
<p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>
</body>
</html>
-	Trang trí văn bản: Thuộc tính này text-decoration chủ yếu được sử dụng để xóa phần gạch chân khỏi các liên kết
Vd: a:link {
  text-decoration: none;
}

a:visited {
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

a:active {
  text-decoration: underline;
}
-	Màu nền: Thuộc background-color tính có thể được sử dụng để chỉ định màu nền cho các liên kết
Vd: a:link {
  background-color: yellow;
}

a:visited {
  background-color: cyan;
}

a:hover {
  background-color: lightgreen;
}

a:active {
  background-color: hotpink;
} 
-	Nút liên kết:  Liên kết dưới dạng hộp/nút
Vd: a:link, a:visited {
  background-color: #f44336;
  color: white;
  padding: 14px 25px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a:hover, a:active {
  background-color: red;
}
7.	Danh sách
-	Các điểm đánh dấu mục danh sách khác nhau: Thuộc list-style-type tính chỉ định loại điểm đánh dấu mục danh sách
Vd: ul.a {
  list-style-type: circle;
}

ul.b {
  list-style-type: square;
}

ol.c {
  list-style-type: upper-roman;
}

ol.d {
  list-style-type: lower-alpha;
}
-	Hình ảnh: Thuộc list-style-imagetính chỉ định một hình ảnh làm điểm đánh dấu mục danh sách
Vd: ul {
  list-style-image: url('sqpurple.gif');
}
-	Định vị các điểm đánh dấu mục danh sách: Thuộc list-style-positiontính chỉ định vị trí của các điểm đánh dấu mục danh sách (dấu đầu dòng)
Vd: ul.b {
  list-style-position: inside;
}
</style>
</head>
<body>

<h1>The list-style-position Property</h1>

<h2>list-style-position: outside (default):</h2>
<ul class="a">
  <li>Coffee - A brewed drink prepared from roasted coffee beans, which are the seeds of berries from the Coffea plant</li>
  <li>Tea - An aromatic beverage commonly prepared by pouring hot or boiling water over cured leaves of the Camellia sinensis, an evergreen shrub (bush) native to Asia</li>
  <li>Coca Cola - A carbonated soft drink produced by The Coca-Cola Company. The drink's name refers to two of its original ingredients, which were kola nuts (a source of caffeine) and coca leaves</li>
</ul>

<h2>list-style-position: inside:</h2>
<ul class="b">
  <li>Coffee - A brewed drink prepared from roasted coffee beans, which are the seeds of berries from the Coffea plant</li>
  <li>Tea - An aromatic beverage commonly prepared by pouring hot or boiling water over cured leaves of the Camellia sinensis, an evergreen shrub (bush) native to Asia</li>
  <li>Coca Cola - A carbonated soft drink produced by The Coca-Cola Company. The drink's name refers to two of its original ingredients, which were kola nuts (a source of caffeine) and coca leaves</li>
</ul>
</body>
</html>
-	Xóa cài đặt mặc định: Thuộc tính này list-style-type:nonecũng có thể được sử dụng để xóa điểm đánh dấu/dấu đầu dòng. Lưu ý rằng danh sách cũng có lề và phần đệm mặc định. Để loại bỏ phần này, hãy thêm margin:0và padding:0vào <ul> hoặc <ol>
Vd: ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}
-	Thuộc tính viết tắt: 
•	Thuộc list-style tính là một thuộc tính viết tắt
•	list-style-type(nếu chỉ định list-style-image, giá trị của thuộc tính này sẽ được hiển thị nếu hình ảnh vì lý do nào đó không thể hiển thị)
•	list-style-position(chỉ định xem các điểm đánh dấu mục danh sách sẽ xuất hiện bên trong hay bên ngoài luồng nội dung)
•	list-style-image(chỉ định một hình ảnh làm điểm đánh dấu mục danh sách)
Vd: ul {
  list-style: square inside url("sqpurple.gif");
}
-	kiểu danh sách với màu sắc: 
Vd: ol {
  background: #ff9999;
  padding: 20px;
}

ul {
  background: #3399ff;
  padding: 20px;
}

ol li {
  background: #ffe5e5;
  color: darkred;
  padding: 5px;
  margin-left: 35px;
}

ul li {
  background: #cce5ff;
  color: darkblue;
  margin: 5px;
}


		




	










	




















