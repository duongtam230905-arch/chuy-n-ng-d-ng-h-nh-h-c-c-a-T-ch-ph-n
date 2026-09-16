# 📐 DỰ ÁN HỌC LIỆU CHUYÊN SÂU: ỨNG DỤNG HÌNH HỌC CỦA TÍCH PHÂN
**Chương trình Giáo dục Phổ thông 2018 – Môn Toán 12**

**Đơn vị/Cá nhân biên soạn:** Thầy Tâm dạy Toán
**Liên hệ (Zalo):** 0837715745
**Nền tảng công nghệ:** $\LaTeX$ (Định dạng chuẩn in ấn quốc tế)
**Phiên bản:** 1.0.0 | **Cập nhật lần cuối:** Tháng 9/2026

---

## 1. Tầm nhìn và Mục tiêu sư phạm (Pedagogical Vision)
Dự án này không chỉ đơn thuần là một tập hợp các bài tập tính toán, mà là một hệ sinh thái học liệu toàn diện được thiết kế chuyên biệt cho chuyên đề **Ứng dụng hình học của Tích phân** (Toán 12). Bám sát định hướng phát triển năng lực của Chương trình GDPT 2018, dự án giải quyết triệt để sự chuyển dịch từ tư duy "giải tích nặng tính toán" sang "mô hình hóa toán học và giải quyết vấn đề thực tiễn".

**Mục tiêu cốt lõi:**
*   **Trực quan hóa không gian:** Chuyển đổi các khái niệm trừu tượng (diện tích hình phẳng phức tạp, thể tích vật thể cắt ngang, khối tròn xoay) thành các hình vẽ vector siêu nét thông qua hệ thống mã lệnh `TikZ` và `pgfplots`.
*   **Mô hình hóa thực tiễn:** Tích hợp sâu chuỗi bài toán ứng dụng (tính toán chi phí vật liệu, thể tích bồn chứa công nghiệp, thiết kế vòm cầu Parabol/Ellipse), giúp học sinh hiểu rõ bản chất "Tích phân dùng để làm gì trong đời sống".
*   **Đón đầu cấu trúc kiểm tra mới:** Cung cấp ma trận đề thi và hệ thống bài tập rèn luyện tuân thủ tuyệt đối định dạng thi mới của Bộ GD&ĐT (Trắc nghiệm nhiều lựa chọn, Trắc nghiệm Đúng/Sai, Trắc nghiệm Trả lời ngắn).

## 2. Kiến trúc mã nguồn $\LaTeX$ (Modular Architecture)
Để đảm bảo tính nhất quán cao nhất về mặt Typography và khả năng mở rộng trong tương lai, dự án được thiết kế theo cấu trúc module (tách biệt hoàn toàn giữa phần định dạng và nội dung).

```text
Chuyen-De-Tich-Phan-12/
│
├── README.md                           ← Tài liệu đặc tả dự án (Project Specification)
├── PLAN.md                             ← Kế hoạch biên soạn và Ma trận nội dung
├── LICENSE.md                          ← Giấy phép sử dụng và chia sẻ học liệu
├── CONTRIBUTING.md                     ← Hướng dẫn đóng góp cho dự án
├── main.tex                            ← File biên dịch tổng (tích hợp toàn bộ chương)
│
├── assets/                             ← Thư mục chứa tài nguyên lõi
│   ├── style.sty                       ← Gói cấu hình tự xây dựng (tcolorbox, fancyhdr, margins)
│   ├── macros.tex                      ← Định nghĩa các lệnh viết tắt Toán học và lệnh TikZ dùng chung
│   └── figures/                        ← Chứa các hình vẽ độc lập hoặc file dữ liệu đồ thị (nếu có)
│
├── chapters/                           ← Thư mục chứa nội dung phân mảnh
│   ├── 00-loi-noi-dau.tex              ← Lời nói đầu và Hướng dẫn sử dụng sách
│   ├── 01-dien-tich-hinh-phang.tex     ← Bài 1: Tính diện tích hình phẳng
│   ├── 02-the-tich-vat-the.tex         ← Bài 2: Thể tích vật thể và khối tròn xoay
│   ├── 03-tong-on-kiem-tra.tex         ← Bài 3: Hệ thống đề tổng ôn và chuẩn hóa
│   └── 04-phu-luc-cong-thuc.tex        ← Phụ lục: Bảng tra cứu công thức nhanh
│
└── output/                             ← Thư mục chứa file PDF thành phẩm và file log
```

## 3. Hệ thống Gói Lệnh Tiêu Chuẩn (Core Packages)
Dự án biên dịch bằng **PDFLaTeX**, sử dụng các gói thư viện tối quan trọng sau:
*   **Tiếng Việt:** `vietnam` (bộ `vntex`) cho bảng mã và font tiếng Việt, `mathptmx` cho font kiểu Times New Roman.
*   **Tiêu chuẩn Toán học:** `amsmath`, `amssymb`, `mathtools`, `bm` (đảm bảo hệ thống ký hiệu chuẩn mực).
*   **Đồ họa & Trực quan:**
    *   `tikz`: Xây dựng mọi hình khối hình học, đường cong, mũi tên và mặt cắt không gian.
    *   `pgfplots`: Vẽ đồ thị hàm số giải tích với độ chính xác tuyệt đối, hỗ trợ lệnh `fill` để tô màu miền diện tích tích phân.
*   **Định dạng Sư phạm:** `tcolorbox` (xây dựng các hộp Định lý, Phương pháp giải, Chú ý với hiệu ứng bo góc, đổ bóng thẩm mỹ cao).
*   **Định dạng Bố cục:** `fancyhdr` (kiểm soát Header/Footer chuyên nghiệp), `geometry` (căn lề chuẩn in ấn sách A4 hoặc B5).

## 4. Hướng dẫn Đóng góp và Biên dịch (Compilation Guide)
1.  **Thiết lập môi trường:** Khuyến nghị sử dụng **Overleaf** (đã có sẵn gói `vntex`), **TeXstudio** hoặc **VS Code (với tiện ích LaTeX Workshop)** kèm bản TeX Live/MiKTeX đầy đủ.
2.  **Biên dịch:** Mở file `main.tex` và chạy luồng biên dịch `PDFLaTeX -> PDFLaTeX` (2 lượt) để đảm bảo hệ thống mục lục và tham chiếu chéo (cross-references) được cập nhật chính xác.
3.  **Quy chuẩn viết code:** Mọi công thức Toán học inline sử dụng `$...$`, công thức block sử dụng môi trường `\begin{equation} ... \end{equation}` hoặc `\[...\]`. Không lạm dụng việc ngắt dòng thủ công `\\` trong văn bản thường.
4.  Xem thêm hướng dẫn chi tiết về quy trình đóng góp tại [`CONTRIBUTING.md`](CONTRIBUTING.md) và điều khoản sử dụng tại [`LICENSE.md`](LICENSE.md).
