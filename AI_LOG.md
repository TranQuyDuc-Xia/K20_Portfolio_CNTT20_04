# AI_LOG — Nhật ký sử dụng AI

## Ghi chú lỗi được cung cấp

- **Hiện tượng:** ghi chú ban đầu nêu lỗi server 404, lỗi trang, ảnh không hiển thị và sai đường dẫn.
- **Kết quả được ghi nhận:** “Đã sửa được lỗi”.
- **Thông tin chưa có trong ghi chú:** thời điểm xảy ra; URL hoặc Request URL và HTTP Status cụ thể; trang/ảnh bị ảnh hưởng; nhận định trước khi dùng AI; công cụ/prompt; cách sửa; commit; và kết quả kiểm tra lại trên URL Pages. Không suy diễn các thông tin này. Người thực hiện cần bổ sung nếu còn nhật ký hoặc ảnh/log gốc.

## Hỗ trợ hoàn thiện README

- **Ngày:** 2026-10-30.
- **Hiện tượng/yêu cầu:** README ban đầu chỉ có tên dự án và mô tả ngắn; yêu cầu bài đánh giá cần hướng dẫn để người khác chạy và kiểm tra sản phẩm.
- **Nhận định trước khi dùng AI:** trong phiên làm việc không có ghi nhận riêng về nhận định của sinh viên trước khi hỏi AI.
- **Công cụ và yêu cầu gửi AI:** Copilot trong VS Code; yêu cầu bổ sung README theo các mục của đề bài. AI đọc các trang HTML, CSS, cấu trúc thư mục và README hiện có.
- **Gợi ý của AI:** mô tả cấu trúc và cách chạy website tĩnh; hướng dẫn kiểm tra điều hướng, responsive, bàn phím và form; nêu rõ form chỉ mô phỏng; thêm repo, Pages, hồ sơ tác giả và nguồn xuất bản.
- **Quyết định:** áp dụng các nội dung phù hợp với mã nguồn đã đọc. Không mô tả form như chức năng gửi email/lưu dữ liệu. Dùng liên kết Pages và GitHub đã kiểm tra được.
- **Thay đổi:** cập nhật `README.md` với hướng dẫn sử dụng, cấu trúc thư mục, chức năng thực tế và các liên kết.
- **Kiểm chứng đã thực hiện:** URL GitHub Pages và repository trả HTTP 200 trong lần kiểm tra; `git diff --check` thành công.
- **Giới hạn kiểm chứng:** chưa ghi nhận kiểm tra thủ công từng trang/chức năng trên trình duyệt, đối chiếu SHA giữa local–repository–lần deploy, hoặc lưu ảnh/log minh chứng. HTTP 200 chỉ xác nhận URL phản hồi, không thay thế các kiểm tra đó.

## Hỗ trợ lập release notes

- **Ngày:** 2026-10-30.
- **Hiện tượng/yêu cầu:** đề bài yêu cầu `RELEASE_NOTES.md` mô tả phiên bản, thay đổi, lỗi sửa, commit, hạn chế và cách tiếp tục kiểm tra/bàn giao.
- **Nhận định trước khi dùng AI:** trong phiên làm việc không có ghi nhận riêng về nhận định của sinh viên trước khi hỏi AI.
- **Công cụ và yêu cầu gửi AI:** Copilot trong VS Code; yêu cầu lập release notes cho bản v7.
- **Dữ kiện AI đối chiếu:** mã nguồn hiển thị Lab 5 / PORTFOLIO V5; `main` và `origin/main` cùng trỏ commit `34f3886047fd9eefedcbec8647f94553243ebde1`; URL Pages trả HTTP 200. Không có bằng chứng liên kết SHA này với lần deploy hiện tại.
- **Gợi ý của AI:** tạo release notes ở trạng thái bản nháp, ghi commit nền nhưng phân biệt với commit phát hành, nêu giới hạn xác minh và liệt kê các bước kiểm tra trước khi bàn giao.
- **Quyết định:** dùng trạng thái bản nháp để không khẳng định sản phẩm đã là v7 hoặc đã kiểm chứng deploy khi chưa có căn cứ. Ghi rõ các lỗi cũ chỉ được trích từ ghi chú ban đầu.
- **Thay đổi:** tạo `RELEASE_NOTES.md` và thêm liên kết tới tài liệu trong `README.md`.
- **Kiểm chứng:** đối chiếu nội dung trang và SHA local/remote; thử HTTP status của URL Pages. Cần chạy `git diff --check` sau khi ghi hồ sơ.
