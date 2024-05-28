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
    