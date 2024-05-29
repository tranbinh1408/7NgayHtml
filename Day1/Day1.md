# Báo cáo dự án cuối kỳ môn lập trình script

## I. HTML BASIC

### 1. HTML DOCUMENTS
- Tất cả các tài liệu HTML phải bắt đầu bằng một khai báo loại tài liệu: `<!DOCTYPE html>`
- Khai báo `<!DOCTYPE>` đại diện cho loại tài liệu, giúp trình duyệt hiển thị các trang web đúng cách
- Khai báo `<!DOCTYPE>` cho HTML5 là: `<!DOCTYPE html>`

### 2. HTML HEADINGS
- Tiêu đề được xác định bằng thẻ `<h1>` đến `<h6>`
- Thẻ `<h1>` chứa nội dung quan trọng nhất, thẻ `<h6>` chứa nội dung ít quan trọng hơn

### 3. HTML PARAGRAPHS
- Ghi nội dung của các đoạn HTML bằng thẻ `<p>ghi nội dung</p>`

### 4. HTML LINKS
- Links được ghi bằng thẻ `<a href="gán link">ghi nội dung link</a>`

### 5. HTML IMAGES
- `<img src="link ảnh" alt="văn bản thay thế ảnh" width="chiều ngang ảnh" height="chiều cao ảnh">`

### 6. HOW TO VIEW HTML SOURCE
- Xem nguồn trang: Ctrl + U, chuột phải chọn "Xem nguồn trang"
- Kiểm tra: Chuột phải chọn "Kiểm tra", F12

## II. HTML ELEMENTS
- Thuộc tính "lang": Dùng để khai báo ngôn ngữ của trang web
  - Ví dụ: 
    ```html
    <!DOCTYPE html>
    <html lang="en-US">
    <body>
    ...
    </body>
    </html>
    ```
  - Hai kí tự đầu "en" là ngôn ngữ, hai kí tự cuối "US" là quốc gia.

- Thay đổi phong cách:
  - Ví dụ:
    ```html
    <p style="color:red;">This is a red paragraph.</p>
    ```

- Thuộc tính tiêu đề:
  - Ví dụ:
    ```html
    <p title="I'm a tooltip">This is a paragraph.</p>
    ```
    - Khi bạn di chuyển chuột qua phần tử, giá trị của thuộc tính tiêu đề sẽ được hiển thị dưới dạng chú giải công cụ.

## III. HTML PARAGRAPHS
- Thẻ `<hr>` xác định điểm ngắt theo chủ đề trong trang HTML và thường được hiển thị dưới dạng quy tắc ngang
- Thẻ `<br>` xác định ngắt dòng
- Thẻ `<pre>` dùng để giữ nguyên đoạn văn nhập vào

## IV. HTML STYLES
- Màu nền: `background-color`
- Màu văn bản: `color`
- Phông chữ: `font-family`
- Cỡ chữ: `font-size` 
- Căn chỉnh văn bản: `text-align`
 