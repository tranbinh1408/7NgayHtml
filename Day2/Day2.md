# I. Định dạng văn bản HTML
## 1. Các phần tử HTML '<b>' và '<strong>'
- Phần tử HTML '<b>' xác định văn bản in đậm mà không có bất kỳ tầm quan trọng nào thêm.
Vd: '''
        <p><b>This text is bold.</b></p>
    '''
- Phần tử HTML '<strong>' xác định văn bản có tầm quan trọng cao. Nội dung bên trong thường được hiển thị in đậm.
Vd: '''
        <p><strong>This text important!</strong></p>
    '''
## 2. Phần tử HTML '<i>' và '<em>'
- Phần tử HTML '<i>' xác định một phần văn bản bằng giọng nói hoặc tâm trạng thay thế. Nội dung bên trong thường được hiển thị bằng chữ nghiêng. 
Vd: '''
        <p><i>This text is italic.</i></p>
    '''
- Phần tử HTML '<em>' xác định văn bản được nhấn mạnh. Nội dung bên trong thường được hiển thị bằng chữ nghiêng.
Vd: '''
        <p><i>This text is italic.</i></p>
    '''
## 3. Phần tử HTML '<small>'
- Phần tử HTML <small>xác định văn bản nhỏ hơn.
Vd: '''
        <p><small>This is some smaller text.</small></p>
    '''
## 4. Phần tử HTML '<mark>'
- Phần tử HTML '<mark>' xác định văn bản cần được đánh dấu hoặc đánh dấu.
Vd: '''
        <p>Do not forget to buy <mark>milk</mark> today.</p>
    '''
## 5. Phần tử HTML '<del>'
- Phần tử HTML '<del>' xác định văn bản đã bị xóa khỏi tài liệu. Các trình duyệt thường sẽ gạch một dòng qua văn bản đã xóa.
Vd: '''
        <p>My favorite color is <del>blue</del> red.</p>
    '''
## 6. Phần tử HTML '<ins>'
- Phần tử HTML '<ins>' xác định một văn bản đã được chèn vào tài liệu. Các trình duyệt thường sẽ gạch dưới văn bản được chèn.
Vd: '''
        <p>My favorite color is <del>blue</del> <ins>red</ins>.</p>
    '''
## 7. Phần tử HTML '<sub>' và '<sup>'
- Phần tử HTML '<sub>' xác định văn bản chỉ số dưới. Văn bản chỉ số dưới xuất hiện nửa ký tự bên dưới dòng bình thường và đôi khi được hiển thị bằng phông chữ nhỏ hơn.
Vd: '''
        <p>This is <sub>subscripted</sub> text.</p>
    '''
- Phần tử HTML '<sup>' xác định văn bản chỉ số trên. Văn bản chỉ số trên xuất hiện nửa ký tự phía trên dòng bình thường và đôi khi được hiển thị bằng phông chữ nhỏ hơn. 
Vd: '''
        <p>This is <sup>superscripted</sup> text.</p>
    '''
# II. Các phần tử trích dẫn và trích dẫn HTML
## 1. HTML '<blockquote>' cho Báo giá
- Phần tử HTML <blockquote>xác định một phần được trích dẫn từ một nguồn khác.
- Trình duyệt thường thụt lề <blockquote>các phần tử.
Vd: '''
        <p>Here is a quote from WWF's website:</p>
    <blockquote cite="http://www.worldwildlife.org/who/index.html">
    For 60 years, WWF has worked to help people and nature thrive. As the world's leading conservation organization, WWF works in nearly 100 countries. At every level, we collaborate with people around the world to develop and deliver innovative solutions that protect communities, wildlife, and the places in which they live.
    </blockquote>
    '''
## 2. HTML <q> cho các trích dẫn ngắn
- Thẻ HTML <q>xác định một trích dẫn ngắn.
Vd: '''
        <p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
        # Câu trong thẻ <p> được để trong dấu ngoặc kép.
    '''
## 3. HTML <abbr> cho từ viết tắt
- Thẻ HTML <abbr>xác định từ viết tắt hoặc từ viết tắt, như "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM".
Vd: '''
        <p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
        # Sử dụng thuộc tính tiêu đề chung để hiển thị mô tả cho từ viết tắt/viết tắt khi bạn di chuột qua phần tử. 
    '''
## 4. HTML <địa chỉ> cho thông tin liên hệ
- Thẻ HTML <address>xác định thông tin liên hệ của tác giả/chủ sở hữu tài liệu hoặc bài viết.
- Thông tin liên hệ có thể là địa chỉ email, URL, địa chỉ thực, số điện thoại, địa chỉ mạng xã hội.
- Văn bản trong phần <address>tử thường hiển thị ở dạng in nghiêng và trình duyệt sẽ luôn thêm dấu ngắt dòng trước và sau phần <address>tử.
Vd: '''
        <address>
        Written by John Doe.<br> 
        Visit us at:<br>
        Example.com<br>
        Box 564, Disneyland<br>
        USA
        </address>
    '''
## 5. HTML '<cite>' cho Tiêu đề công việc 
- Thẻ HTML '<cite>' xác định tiêu đề của một tác phẩm sáng tạo (ví dụ: một cuốn sách, một bài thơ, một bài hát, một bộ phim, một bức tranh, một tác phẩm điêu khắc, v.v.). 
Vd: '''
        <p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
    '''
## 6. HTML '<bdo>' để ghi đè hai chiều
- BDO là viết tắt của Ghi đè hai chiều.
- Thẻ HTML '<bdo>' được sử dụng để ghi đè hướng văn bản hiện tại.
Vd: '''
        <bdo dir="rtl">This line will be written from right to left</bdo>
    '''
## 7. Thẻ nhận xét HTML
- Với nhận xét, bạn có thể đặt thông báo và lời nhắc trong mã HTML của mình
Vd: '''
        <!-- This is a comment -->
        <p>This is a paragraph.</p>
        <!-- Remember to add more information here -->
    '''
- Bình luận có thể được sử dụng để ẩn nội dung.
Vd1: '''
        <p>This is a paragraph.</p>
        <!-- <p>This is another paragraph </p> -->
        <p>This is a paragraph too.</p>
    '''
Vd2:
    '''
        <p>This <!-- great text --> is a paragraph.</p>
    '''
# III. CSS
## 1. Đường viền CSS
- Thuộc tính CSS borderxác định đường viền xung quanh phần tử HTML.
## 2. Phần đệm CSS
- Thuộc tính CSS paddingxác định khoảng đệm (khoảng trắng) giữa văn bản và đường viền.
## 3. Ký quỹ CSS
- Thuộc tính CSS marginxác định lề (khoảng trắng) bên ngoài đường viền.
## 4. Liên kết tới CSS bên ngoài
- Ví dụ này sử dụng một URL đầy đủ để liên kết đến một biểu định kiểu:
    '''
        <link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
    '''
- Ví dụ này liên kết đến một biểu định kiểu nằm trong thư mục html trên trang web hiện tại: 
    '''
        <link rel="stylesheet" href="/html/styles.css">
    '''
- Ví dụ này liên kết đến một biểu định kiểu nằm trong cùng thư mục với trang hiện tại:
    '''
        <link rel="stylesheet" href="styles.css">
    '''
# IV. Liên kết HTML
## 1. Liên kết HTML - Thuộc tính đích
- Thuộc targettính có thể có một trong các giá trị sau:

    - _self- Mặc định. Mở tài liệu trong cùng cửa sổ/tab khi tài liệu được nhấp vào
    - _blank- Mở tài liệu trong cửa sổ hoặc tab mới
    - _parent- Mở tài liệu trong khung cha
    - _top- Mở tài liệu ở chế độ toàn màn hình
Vd: '''
        <a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
    '''
## 2. URL tuyệt đối so với URL tương đối
-  URL tuyệt đối (địa chỉ web đầy đủ) trong hrefthuộc tính
- Liên kết cục bộ (liên kết đến một trang trong cùng một trang web) được chỉ định bằng URL tương đối (không có phần "https://www")
## 3. Liên kết đến một địa chỉ email
- Sử dụng mailto:bên trong hrefthuộc tính để tạo liên kết mở chương trình email của người dùng (để cho phép họ gửi email mới)
Vd: '''
        <a href="mailto:someone@example.com">Send email</a>
    '''
## 4. Nút dưới dạng liên kết
Vd: '''
        <button onclick="document.location='default.asp'">HTML Tutorial</button>
    '''
## 5. Tiêu đề liên kết
- Thuộc title tính chỉ định thông tin bổ sung về một phần tử. Thông tin thường được hiển thị dưới dạng văn bản chú giải công cụ khi chuột di chuyển qua phần tử.
Vd: '''
        <a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our HTML Tutorial</a>
    '''
## 6. Liên kết và tạo dấu trang
- Đầu tiên, sử dụng idthuộc tính để tạo dấu trang
- Sau đó, thêm liên kết vào dấu trang ("Chuyển tới Chương 4"), từ trong cùng một trang: '''<a href="#C4">Jump to Chapter 4</a>'''
# V. Hình ảnh
## 1. Hình ảnh nối
- Sử dụng thuộc tính CSS float
Vd: '''
        style="float:right;width:42px;height:42px;">
    '''
## 2. Nền
- Nếu bạn muốn hình nền bao phủ toàn bộ phần tử, bạn có thể đặt thuộc background-sizetính thành cover.
- Ngoài ra, để đảm bảo toàn bộ phần tử luôn được che phủ, hãy đặt background-attachmentthuộc tính thànhfixed.
- Để tránh hình nền lặp lại, hãy đặt background-repeatthuộc tính thành no-repeat.
- Nếu bạn muốn hình nền co giãn để vừa với toàn bộ phần tử, bạn có thể đặt thuộc background-sizetính thành 100% 100%.
## 3. Phần tử <picture> HTML
- Phần tử HTML <picture> giúp các nhà phát triển web linh hoạt hơn trong việc chỉ định tài nguyên hình ảnh.
- Phần <picture> tử chứa một hoặc nhiều <source> phần tử, mỗi phần tử đề cập đến các hình ảnh khác nhau thông qua srcset thuộc tính. Bằng cách này, trình duyệt có thể chọn hình ảnh phù hợp nhất với chế độ xem và/hoặc thiết bị hiện tại.
- Mỗi <source>phần tử có một mediathuộc tính xác định thời điểm hình ảnh phù hợp nhất.