# 📐 DỰ ÁN HỌC LIỆU CHUYÊN SÂU: ỨNG DỤNG HÌNH HỌC CỦA TÍCH PHÂN
**Phương pháp Sư phạm: Kiến tạo & Tư duy**
**Chương trình Giáo dục Phổ thông 2018 – Môn Toán 12**

**Đơn vị/Cá nhân biên soạn:** Thầy Tâm dạy Toán
**Liên hệ (Zalo):** 0837715745
**Nền tảng công nghệ:** $\LaTeX$
**Mục đích sử dụng:** Tài liệu tự học, tự khám phá dành cho học sinh.
**Phiên bản:** 2.0.0 (Tinh gọn & Chuyên sâu Ý tưởng)

---

## 1. Tầm nhìn và Triết lý Sư phạm 
Tài liệu này được tái cấu trúc hoàn toàn, thoát khỏi lối mòn luyện thi truyền thống ("Mớm sẵn lý thuyết $\rightarrow$ Phân dạng $\rightarrow$ Áp dụng công thức"). Thay vào đó, dự án lấy **Học sinh làm trung tâm**, đặt các em vào vai trò người tự tìm ra tri thức thông qua chuỗi câu hỏi dẫn dắt .

**3 Trụ cột cốt lõi của tài liệu:**
1.  **Học sinh tự tìm ra công thức:** Mở đầu mỗi bài học không phải là hộp "Định lý", mà là một **[Hoạt động Khám phá]** mang tính trực quan (ví dụ: chia nhỏ diện tích mảnh đất, cắt lát một ổ bánh mì) để học sinh tự suy luận ra tích phân.
2.  **Tư duy trước, Giải toán sau:** Không có các "Ví dụ mẫu" áp đặt lời giải ngay. Mọi bài toán đều đi qua chu trình:
    `[Tình huống Mở] -> [Câu hỏi Gợi mở] -> [Hình thành Ý tưởng] -> [Lời giải chi tiết]`.
3.  **Học liệu như một người Thầy:** Các câu hỏi gợi mở được biên soạn khéo léo, đóng vai trò như một cuộc đối thoại trực tiếp, giúp học sinh tự gỡ rối và phát triển tư duy khi đang tự học ở nhà.

## 2. Kiến trúc mã nguồn $\LaTeX$ 
Do tập trung toàn bộ không gian để phát triển ý tưởng và tư duy, dự án được rút gọn thành 3 module lõi, loại bỏ các phần luyện đề không cần thiết:

```text
Chuyen-De-Tich-Phan-12/
│
├── README.md               ← Triết lý sư phạm & Đặc tả dự án
├── PLAN.md                 ← Khung chương trình chi tiết
├── main.tex                ← File biên dịch tổng
│
├── assets/                 
│   ├── style.sty           ← [Cập nhật] Thêm các hộp giao diện mới: hopkhampha, hopgoimo, hopytuong
│   ├── macros.tex          ← Định nghĩa lệnh Toán và đồ họa TikZ/pgfplots
│
├── chapters/               ← Thư mục nội dung
│   ├── 00-loi-noi-dau.tex  ← Hướng dẫn học sinh cách "tự học" với chu trình tư duy
│   ├── 01-dien-tich.tex    ← Bài 1: Khám phá Diện tích hình phẳng
│   └── 02-the-tich.tex     ← Bài 2: Khám phá Thể tích vật thể & Khối tròn xoay
```

## 3. Hệ thống Gói Lệnh Tiêu Chuẩn 
Dự án biên dịch bằng **PDFLaTeX**, sử dụng các gói thư viện tối quan trọng sau:
*   **Tiếng Việt:** `vietnam` (bộ `vntex`) cho bảng mã và font tiếng Việt, `mathptmx` cho font kiểu Times New Roman.
*   **Tiêu chuẩn Toán học:** `amsmath`, `amssymb`, `mathtools`, `bm` (đảm bảo hệ thống ký hiệu chuẩn mực).
*   **Đồ họa & Trực quan:**
    *   `tikz`: Xây dựng mọi hình khối hình học, đường cong, mũi tên và mặt cắt không gian.
    *   `pgfplots`: Vẽ đồ thị hàm số giải tích với độ chính xác tuyệt đối, hỗ trợ lệnh `fill` để tô màu miền diện tích tích phân.
*   **Định dạng Sư phạm:** `tcolorbox` (xây dựng các hộp Định lý, Phương pháp giải, Chú ý với hiệu ứng bo góc, đổ bóng thẩm mỹ cao).
*   **Định dạng Bố cục:** `fancyhdr` (kiểm soát Header/Footer chuyên nghiệp), `geometry` (căn lề chuẩn in ấn sách A4 hoặc B5).

## 4. Hướng dẫn Đóng góp và Biên dịch 
1.  **Thiết lập môi trường:** Khuyến nghị sử dụng **Overleaf** (đã có sẵn gói `vntex`), **TeXstudio** hoặc **VS Code (với tiện ích LaTeX Workshop)** kèm bản TeX Live/MiKTeX đầy đủ.
2.  **Biên dịch:** Mở file `main.tex` và chạy luồng biên dịch `PDFLaTeX -> PDFLaTeX` (2 lượt) để đảm bảo hệ thống mục lục và tham chiếu chéo được cập nhật chính xác.
3.  **Quy chuẩn viết code:** Mọi công thức Toán học inline sử dụng `$...$`, công thức block sử dụng môi trường `\begin{equation} ... \end{equation}` hoặc `\[...\]`. Không lạm dụng việc ngắt dòng thủ công `\\` trong văn bản thường.
4.  Xem thêm hướng dẫn chi tiết về quy trình đóng góp tại [`CONTRIBUTING.md`](CONTRIBUTING.md) và điều khoản sử dụng tại [`LICENSE.md`](LICENSE.md).
