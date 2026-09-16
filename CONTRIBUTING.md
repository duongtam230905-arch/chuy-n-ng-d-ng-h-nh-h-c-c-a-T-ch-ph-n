# HƯỚNG DẪN ĐÓNG GÓP (CONTRIBUTING)

Cảm ơn bạn đã quan tâm đến việc đóng góp cho dự án **Ứng dụng hình học của Tích phân -- Toán 12**! Tài liệu này áp dụng cho giáo viên, sinh viên sư phạm, hoặc bất kỳ ai muốn giúp hoàn thiện học liệu.

## 1. Các hình thức đóng góp

*   **Báo lỗi nội dung:** Phát hiện sai sót trong đề bài, lời giải, đáp án, hoặc công thức Toán học.
*   **Báo lỗi kỹ thuật $\LaTeX$:** Lỗi biên dịch, hình TikZ/pgfplots hiển thị sai, overfull/underfull hbox.
*   **Bổ sung bài tập:** Đóng góp thêm ví dụ, câu hỏi trắc nghiệm (đúng cấu trúc 3 phần: nhiều lựa chọn / Đúng-Sai / trả lời ngắn).
*   **Cải thiện trình bày:** Đề xuất cải tiến bố cục, màu sắc, hộp `tcolorbox`, miễn là giữ đúng bảng màu và phong cách đã thiết lập trong `assets/style.sty`.

## 2. Quy trình báo lỗi / đề xuất

1.  Xác định rõ vị trí lỗi: tên file (ví dụ `chapters/02-the-tich-vat-the.tex`), số Ví dụ/Câu hỏi liên quan.
2.  Mô tả ngắn gọn: lỗi hiện tại là gì, kết quả đúng nên là gì (kèm cách tính nếu có thể).
3.  Gửi phản hồi qua Zalo **0837715745** hoặc tạo Pull Request/Issue nếu dự án được lưu trữ trên nền tảng Git.

## 3. Quy chuẩn kỹ thuật khi đóng góp mã nguồn $\LaTeX$

Để giữ tính nhất quán của toàn dự án, mọi đóng góp mã nguồn cần tuân thủ:

| Hạng mục | Quy chuẩn |
|---|---|
| **Trình biên dịch** | PDFLaTeX (không dùng XeLaTeX/LuaLaTeX) |
| **Bảng mã/Font tiếng Việt** | `\usepackage[utf8]{vietnam}` + `\usepackage{mathptmx}` |
| **Hộp trình bày** | Dùng lại các môi trường có sẵn: `hopdinhly`, `hopvidu`, `hopchuy`, `hopphuongphap`, `loigiai` (định nghĩa trong `assets/style.sty`) -- không tạo hộp `tcolorbox` mới nếu môi trường có sẵn đã đáp ứng đủ |
| **Đánh số** | Dùng lệnh `\cauhoi` cho câu hỏi trắc nghiệm; các bộ đếm Định lý/Ví dụ/Chú ý tự động qua `\refstepcounter` -- **không gõ tay số thứ tự** |
| **Hình vẽ** | 100% dùng `TikZ`/`pgfplots`, tuyệt đối không `\includegraphics` ảnh bitmap |
| **Công thức dài** | Nếu một dòng công thức có nguy cơ tràn lề (overfull hbox), tách bằng môi trường `align*` thay vì để nguyên một dòng `\[...\]` |
| **Màu sắc** | Chỉ dùng các màu đã định nghĩa: `navy`, `navylight`, `teal`, `tealbg`, `amber`, `amberbg`, `shadowgray`, `softgray` |

## 4. Kiểm tra trước khi gửi đóng góp

Trước khi gửi bất kỳ thay đổi nào, vui lòng tự kiểm tra:

- [ ] Biên dịch thành công bằng `pdflatex main.tex` (chạy 2 lần), không phát sinh lỗi mới.
- [ ] Không có cảnh báo `Overfull \hbox` / `Underfull \hbox` mới trong log.
- [ ] Đáp án đã được tính tay lại (hoặc dùng công cụ CAS) để xác nhận chính xác trước khi thêm vào bộ đếm `\cauhoi`.
- [ ] Văn phong nhất quán với phần còn lại của tài liệu (xưng hô "các em", giọng văn sư phạm, rõ ràng, không viết tắt tùy tiện).

## 5. Bản quyền đóng góp

Bằng việc gửi đóng góp (nội dung, hình vẽ, mã nguồn), bạn đồng ý rằng đóng góp đó sẽ được phát hành theo cùng giấy phép của dự án -- xem chi tiết tại [`LICENSE.md`](LICENSE.md). Tên của người đóng góp sẽ được ghi nhận trong phần "Cảm ơn" (nếu có) ở lần cập nhật kế tiếp, trừ khi có yêu cầu khác.

---

*Mọi thắc mắc xin liên hệ Thầy Tâm dạy Toán qua Zalo 0837715745.*
