# AI LOG – BUỔI 7, TIẾT 3

> Điền vào `[ ... ]`, tích `[x]` vào lựa chọn phù hợp. Ghi đúng việc đã làm; chưa kiểm tra thì ghi “Chưa kiểm tra”. Không cần chép toàn bộ cuộc trò chuyện AI.

## Thông tin sinh viên

- Họ và tên: [Ma Tráng Pao]
- Mã sinh viên – Lớp: [2071020150-lớp 20-02]
- Ngày thực hiện: [30 ]
- Link repository: [ https://github.com/matrangpao14-sudo/bai-tap-A2-A2.git ]
- URL website: [ https://github.com/matrangpao14-sudo/bai-tap-A2-A2.git ]
- Tình huống: [ sai đường link css] Website của tôi  [ https://github.com/matrangpao14-sudo/bai-tap-A2-A2.git ] Repo luyện của giảng viên

## 1. Nhận định của tôi trước khi hỏi AI

- Trang/thao tác gặp lỗi: [link css]
- Mong muốn và hiện tượng thực tế: [ Tôi muốn trang portfolio hiển thị đúng giao diện đã thiết kế bằng CSS. Tuy nhiên, đường dẫn CSS trong mã HTML đang trỏ đến một đường dẫn trên máy tính cá nhân nên khi đưa mã nguồn lên GitHub hoặc mở trên máy khác, trình duyệt có thể không tìm thấy tệp CSS. ]
- Dữ kiện đã kiểm tra (cấu trúc tệp, Request URL, Status…): [ Repository có tệp index.html ở thư mục gốc và có thư mục css. Trong index.html, dòng liên kết CSS đang ghi D:\CNTT20-04\portfolio\css\style.css. Request URL và Status trong thẻ Network: Chưa kiểm tra. Tên tệp CSS cụ thể bên trong thư mục css: cần mở thư mục để xác nhận. ]
- Tôi nghi nguyên nhân là: [Đường dẫn CSS đang dùng đường dẫn tuyệt đối của máy tính Windows thay vì đường dẫn tương đối trong dự án. ]
- Vì sao tôi nhận định như vậy: [ Đường dẫn D:\CNTT20-04\portfolio\css\style.css chỉ phù hợp với vị trí thư mục trên máy tính đã tạo ra nó. Khi website chạy từ GitHub hoặc môi trường khác, đường dẫn này không còn đúng.]

## 2. Tôi hỏi AI và nhận được gợi ý

- Nguồn: [x ] Công cụ AI: [ ChatGPT ]  [ ] Phản hồi mẫu của giảng viên
- Câu hỏi/prompt tôi đã gửi (hoặc tình huống của phản hồi mẫu):

  [ Tôi có repository GitHub portfolio gồm tệp index.html ở thư mục gốc và thư mục css. Trong index.html, đường dẫn CSS đang là D:\CNTT20-04\portfolio\css\style.css. Hãy giải thích nguyên nhân và hướng dẫn sửa đường dẫn để website tìm thấy tệp CSS.” ]

- Gợi ý chính của AI:

  [ Dùng đường dẫn tương đối thay cho đường dẫn tuyệt đối trên máy tính.
Nếu tệp CSS thực sự có tên style.css và nằm trong thư mục css cùng cấp với index.html, sửa thành: <link rel="stylesheet" href="css/style.css">]

## 3. Quyết định của tôi

- [ ] Chấp nhận gợi ý
- [ dùng ] Chỉnh sửa gợi ý rồi áp dụng
- [ ] Bác bỏ gợi ý

- Tôi quyết định làm gì: [ ôi chọn dùng đường dẫn tương đối css/style.css nếu kiểm tra thấy tệp trong thư mục css đúng là style.css. Nếu tên tệp khác, tôi sẽ thay style.css bằng đúng tên tệp đang có.

 ]
- Lý do, dựa trên dữ kiện nào: [dựa trên dữ kiện nào: Repository có thư mục css và index.html nằm ở thư mục gốc; đường dẫn tuyệt đối hiện tại chứa tên ổ đĩa và thư mục riêng trên máy tính Windows nên không phù hợp để dùng chung trên website.. ]

## 4. Thực hiện và kiểm chứng

- Tệp/vị trí đã sửa (không sửa thì ghi rõ): [Chưa sửa tệp trên repository. Vị trí dự kiến sửa là dòng <link rel="stylesheet"> trong index.html. ]
- Nội dung thay đổi hoặc cách xử lý khác: [ Dự kiến thay đường dẫn tuyệt đối D:\CNTT20\portfolio\css\style.css bằng đường dẫn tương đối css/style.css sau khi xác nhận tên tệp CSS. Chưa xác nhận và chưa thực hiện thay đổi. ]
- Commit của bản sửa, nếu có: [ Chưa có. ]
- Bản sửa đã deploy: [ ] Có  [ x] Chưa  [ ] Không phát sinh bản sửa

| Nội dung kiểm tra | Trước xử lý | Sau xử lý/thử lại |
| Request URL và Status của tài nguyên liên quan| Chưa kiểm tra trong Network; trong mã HTML thấy đường dẫn tuyệt đối trên máy tính| Chưa kiểm tra vì chưa sửa và chưa thử lại|
| Request URL và Status của tài nguyên liên quan | [ Giao diện/chức năng trên URL website ] | [ Chưa kiểm tra trên website đã triển khai] |
| Giao diện/chức năng trên URL website | [ . ] | [ ... ] |

- Cách thử lại và kết quả thực tế: [ Sau khi sửa đúng đường dẫn, mở website, nhấn F12 → Network, tải lại trang và lọc CSS. Kiểm tra Request URL trỏ đến tệp CSS trong thư mục css và Status là 200; đồng thời quan sát giao diện có nhận định dạng CSS hay không. Hiện chưa thực hiện bước thử lại nên chưa có kết quả thực tế. ]
- Căn cứ để đối chiếu (URL tệp, commit, đường dẫn ảnh chụp hoặc dữ kiện quan sát): [Repository https://github.com/matrangpao/portfolio và tệp index.html trên nhánh main; dòng liên kết CSS hiện tại là đường dẫn Windows tuyệt đối. Chưa có commit sửa hoặc ảnh chụp Network. ]

## 5. Kết luận

- [ ] Đã xử lý được  [ ] Xử lý được một phần  [ x] Chưa xử lý được
- Điều tôi rút ra hoặc việc cần làm tiếp: [ - Tôi hiểu rằng khi liên kết CSS trong website, nên sử dụng đường dẫn tương đối theo cấu trúc thư mục của dự án, không nên dùng đường dẫn tuyệt đối trên máy tính cá nhân. Việc tiếp theo là mở thư mục css để xác nhận tên tệp, sửa đường dẫn trong index.html, tải lại website và kiểm tra Status trong Network. Chỉ kết luận đã xử lý được khi CSS tải thành công và giao diện hiển thị đúng. ]

---

*Tệp là minh chứng MC2 để nhận định mức đạt của tiết học; không tính điểm MC2 riêng. Nếu có tình huống khác, sao chép mục 1–5 để ghi thêm.*
