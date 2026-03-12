Câu 1: Selector nào có độ ưu tiên cao nhất trong CSS?
Inline Style

Câu 2 : Nếu một phần tử HTML có cả h1, .title, và #main cùng set color — selector nào thắng? Tại sao?
#main vì ID = 100 điểm Class = 10 điểm tag = 1 điểm nên 100 > 10 > 1 màu của ID sẽ được áp dụng

Câu 3: Nếu bạn thêm style="color: pink" trực tiếp vào phần tử ở Câu 2, kết quả thay đổi như thế nào?
Phần tử sẽ chuyển sang màu pink. Inline style có điểm ưu tiên là 1000, cao hơn cả ID, nên nó sẽ ghi đè lên màu của #main

Câu 4: Tại sao theme.css có thể override style từ base.css? Điều kiện để override thành công là gì?
Hai cái này bằng nhau điều kiện là ai viết sau thì người đó sẽ thắng theme.css phải được khai báo nằm dưới base.css nên theme.css thắng

Câu 5: Trong project, có hai phần tử đều dùng class .title nhưng hiển thị màu khác nhau. Giải thích tại sao.
Do ID đè Class: Một phần tử dùng cả .title và #main (hoặc #special), khi đó ID sẽ thắng và áp dụng màu của ID.
Do Inline Style: Một phần tử có .title nhưng lại có thêm style="color: ..." ngay tại thẻ, dẫn đến màu inline thắng.

Câu 6: Phần tử nào trong project có CSS phức tạp nhất? Liệt kê các selector tác động và giải thích selector thắng cuối cùng.
Phần tử phức tạp nhất là thẻ h1 ở trang Dashboard
selector tác động:

Tag selector h1 (từ base.css).

Class selector .title (từ base.css và theme.css).

ID selector #special (từ base.css và theme.css).

Inline style style="color: HotPink".

Internal CSS trong thẻ <style>.

Vô địch Inline style (1000 điểm)
