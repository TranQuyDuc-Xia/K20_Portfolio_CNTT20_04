# Portfolio cá nhân — K20_Portfolio_CNTT20_04

**Tác giả:** TranQuyDuc ([hồ sơ GitHub](https://github.com/TranQuyDuc-Xia))

**Mô tả:** Portfolio tĩnh phục vụ bài thực hành thiết kế web và triển khai hệ thống phần mềm. Trang giới thiệu sinh viên, kỹ năng, dự án mẫu, lộ trình học tập và một biểu mẫu liên hệ mô phỏng; được xây dựng bằng HTML5 và CSS3, không dùng framework hay backend.

## Liên kết

- **Sản phẩm đã xuất bản:** [GitHub Pages](https://tranquyduc-xia.github.io/K20_Portfolio_CNTT20_04/)
- **Mã nguồn:** [TranQuyDuc-Xia/K20_Portfolio_CNTT20_04](https://github.com/TranQuyDuc-Xia/K20_Portfolio_CNTT20_04)
- **Hồ sơ tác giả:** [github.com/TranQuyDuc-Xia](https://github.com/TranQuyDuc-Xia)
- **Nhật ký AI và kiểm chứng:** [AI_LOG.md](./AI_LOG.md)
- **Ghi chú phát hành:** [RELEASE_NOTES.md](./RELEASE_NOTES.md)

## Cấu trúc thư mục

```text
K20_Portfolio_CNTT20_04/
├── index.html       # Trang portfolio chính
├── ket-qua.html     # Trang kết quả mô phỏng gửi form
├── README.md        # Hướng dẫn sử dụng, kiểm tra và xuất bản
├── AI_LOG.md        # Nhật ký AI, quyết định và kiểm chứng
├── RELEASE_NOTES.md # Phiên bản, thay đổi và tình trạng bàn giao
├── css/
│   └── style.css    # Giao diện, bố cục responsive và trạng thái tương tác
└── assets/          # Tài nguyên hình ảnh của dự án
```

## Chạy trên máy

Đây là website tĩnh, không cần cài dependency hoặc build. Có thể mở `index.html` trực tiếp bằng trình duyệt. Để kiểm tra đầy đủ luồng form qua HTTP, mở PowerShell tại thư mục dự án và chạy:

```powershell
py -m http.server 8000
```

Sau đó truy cập <http://localhost:8000/>. Dừng máy chủ bằng `Ctrl+C`.

## Kiểm tra trang và chức năng

1. Mở `index.html` và dùng menu **Giới thiệu**, **Kỹ năng**, **Dự án**, **Lộ trình**, **Liên hệ** để kiểm tra các mục điều hướng trong trang.
2. Thu nhỏ hoặc mở rộng cửa sổ trình duyệt để kiểm tra bố cục responsive; các thẻ dự án chuyển từ một cột sang hai hoặc ba cột theo chiều rộng màn hình.
3. Dùng phím `Tab` để kiểm tra điều hướng bàn phím và viền focus. Các liên kết trong thẻ dự án dẫn tới mục tương ứng trên cùng trang.
4. Tại phần **Liên hệ**, thử gửi form để xem trình duyệt kiểm tra trường bắt buộc, định dạng email, tên tối thiểu 2 ký tự và nội dung tối thiểu 10, tối đa 500 ký tự. Form gửi bằng GET sang `ket-qua.html`; các giá trị thử nghiệm sẽ xuất hiện trong URL.
5. Trang `ket-qua.html` thông báo kết quả mô phỏng. Form không gửi email và không lưu dữ liệu vào cơ sở dữ liệu. **Chỉ dùng dữ liệu giả, không nhập mật khẩu hoặc thông tin cá nhân thật.**

## Xuất bản và minh chứng

Website được xuất bản bằng **GitHub Pages** từ repository này; đây là website HTML/CSS thuần, không có bước build. Có thể kiểm tra sản phẩm trực tiếp tại [URL Pages](https://tranquyduc-xia.github.io/K20_Portfolio_CNTT20_04/) và đối chiếu mã nguồn, lịch sử dự án tại [repository GitHub](https://github.com/TranQuyDuc-Xia/K20_Portfolio_CNTT20_04). Hồ sơ tác giả: [TranQuyDuc-Xia](https://github.com/TranQuyDuc-Xia).
