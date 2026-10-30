# Release notes

## v7 — Bản nháp bàn giao

- **Ngày cập nhật hồ sơ:** 2026-10-30
- **Trạng thái:** Chưa xác nhận phát hành bản v7. Mã nguồn hiện kiểm tra được vẫn hiển thị “Lab 5” và “PORTFOLIO V5”; cần hoàn thiện, commit và kiểm tra lại trước khi đổi trạng thái thành bản bàn giao.
- **Sản phẩm:** [Portfolio cá nhân trên GitHub Pages](https://tranquyduc-xia.github.io/K20_Portfolio_CNTT20_04/)
- **Repository:** [K20_Portfolio_CNTT20_04](https://github.com/TranQuyDuc-Xia/K20_Portfolio_CNTT20_04)

### Thay đổi hồ sơ trong lần cập nhật này

- Bổ sung README hướng dẫn chạy website tĩnh, kiểm tra điều hướng, responsive, bàn phím và form.
- Chuẩn hóa nhật ký AI thành `AI_LOG.md`; giữ riêng những dữ kiện chưa có để người thực hiện bổ sung, không khẳng định các lỗi lịch sử đã được kiểm chứng lại.

### Lỗi đã sửa và tình trạng xác minh

- Ghi chú ban đầu trong `AI_LOG.md` nêu lỗi 404, lỗi trang, ảnh không hiển thị và sai đường dẫn, đồng thời ghi “Đã sửa được lỗi”. Ghi chú chưa có Request URL, Status, cách sửa, commit hoặc ảnh/log kiểm tra lại nên chưa đủ căn cứ để mô tả chi tiết các lỗi này là đã được xác minh trên bản v7.
- URL GitHub Pages và repository phản hồi HTTP 200 trong lần kiểm tra ngày 2026-10-30. Đây chỉ xác nhận URL truy cập được; chưa xác định SHA được GitHub Pages triển khai và chưa kiểm thử lại từng trang, CSS, ảnh hoặc liên kết trong trình duyệt.

### Commit liên quan

- **Commit nền được kiểm tra:** [`34f3886047fd9eefedcbec8647f94553243ebde1`](https://github.com/TranQuyDuc-Xia/K20_Portfolio_CNTT20_04/commit/34f3886047fd9eefedcbec8647f94553243ebde1) trên `main`; tại thời điểm kiểm tra, `origin/main` trỏ cùng commit.
- Đây là commit nền hiện có, **không được xác nhận là commit phát hành v7**. Các thay đổi đang làm trong workspace chưa được gắn với một commit cuối hoặc một lần deploy cụ thể. Sau khi chốt mã, cập nhật mục này bằng SHA commit đã push và dùng chính SHA đó trong phiếu nộp.

### Hạn chế còn lại

- Website là HTML/CSS tĩnh, không có backend. Form dùng GET, dữ liệu thử sẽ xuất hiện trong URL; không gửi email và không lưu dữ liệu. Chỉ thử với dữ liệu giả.
- Mã hiện tại vẫn mang nhãn Lab 5 / V5, vì vậy chưa thể hiện rõ phiên bản v7.
- Ghi chú lỗi 404/ảnh/đường dẫn chưa có bằng chứng gốc và kết quả kiểm thử cụ thể. Chưa có ảnh/log đối chiếu local – repository – URL, cũng chưa xác nhận SHA triển khai Pages.
- Nội dung form có nhãn “Mật khẩu (20 ký tự trở lên)” nhưng phần nhập liệu đang đặt `minlength="10"` và `maxlength="500"`; cần thống nhất nội dung và giới hạn trước khi bàn giao.

### Tiếp tục kiểm tra và bàn giao

1. Hoàn thiện nội dung và nhãn phiên bản trong mã nguồn; kiểm tra cả `index.html`, `ket-qua.html`, `css/` và các tài nguyên cần dùng.
2. Chạy website local, thử điều hướng, bố cục responsive, bàn phím và xác thực form; ghi lại kết quả cùng ảnh/log thực tế.
3. Xem diff, commit các thay đổi có ý nghĩa và push lên `main`. Ghi SHA commit cuối sau khi push.
4. Chờ GitHub Pages deploy thành công, mở URL trong cửa sổ riêng tư, kiểm tra các trang và tài nguyên; đối chiếu nội dung với commit vừa ghi.
5. Chỉ sau khi hoàn tất các bước trên, cập nhật trạng thái release thành đã phát hành và thay commit nền bằng SHA chính xác của bản v7 được nộp.
