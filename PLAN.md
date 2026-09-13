# 📋 KẾ HOẠCH TỔNG THỂ VÀ MA TRẬN NỘI DUNG
**Dự án: Chuyên đề Ứng dụng hình học của Tích phân (GDPT 2018)**

> **Định mức dự kiến:** ~50 trang A4 | **Cấp độ:** Lớp 12 | **Phân khúc:** Cơ bản đến Vận dụng cao

---

## PHẦN I: THỐNG KÊ VÀ PHÂN BỔ THỜI LƯỢNG BIÊN SOẠN

| Mã học phần | Phân hệ nội dung | Độ dài dự kiến | Tiến độ |
|:---|:---|:---:|:---:|
| **MOD-00** | Bìa sách, Mục lục tự động, Lời mở đầu | 4 trang | 0% |
| **MOD-01** | Bài 1: Tính diện tích hình phẳng | 15 trang | 0% |
| **MOD-02** | Bài 2: Tính thể tích vật thể và khối tròn xoay | 16 trang | 0% |
| **MOD-03** | Bài 3: Kiểm tra Đánh giá (Định dạng mới) | 12 trang | 0% |
| **MOD-04** | Phụ lục & Bảng tra cứu công thức nhanh | 3 trang | 0% |
| **TỔNG** | **Bản thảo hoàn chỉnh** | **~50 trang** | **0%** |

---

## PHẦN II: KHUNG XƯƠNG NỘI DUNG CHI TIẾT (SYLLABUS)

### 🟢 Bài 1: Diện tích hình phẳng (Dự kiến 15 trang)
**Mục tiêu:** Học sinh nắm vững ý nghĩa hình học của tích phân, thành thạo kỹ năng xét dấu để phá giá trị tuyệt đối và ứng dụng tính diện tích các mô hình phẳng.

*   [ ] **1. Nền tảng Lý thuyết & Định lý cơ bản**
    *   Định lý và công thức diện tích hình phẳng giới hạn bởi 1 đường cong $y=f(x)$, trục $Ox$ và $x=a, x=b$.
    *   Định lý và công thức diện tích hình phẳng giới hạn bởi 2 đường cong $y=f(x), y=g(x)$.
    *   *Kỹ thuật trình bày:* Xây dựng hộp `tcolorbox` làm nổi bật công thức, đi kèm 2 hình vẽ `TikZ` minh họa tổng quát.

*   [ ] **2. Dạng 1: Tính diện tích khi giả thiết cho sẵn hàm số và cận**
    *   Phương pháp phá dấu trị tuyệt đối bằng cách giải phương trình $f(x)=0$ hoặc $f(x)=g(x)$ trên đoạn $[a; b]$.
    *   Bài tập chia thành các nhóm hàm: Đa thức (bậc 2, bậc 3), Phân thức, Hàm lượng giác, Hàm mũ/logarit.

*   [ ] **3. Dạng 2: Tính diện tích khi thiếu cận (Giới hạn bởi các đường cong khép kín)**
    *   Kỹ năng thiết lập phương trình hoành độ giao điểm để tìm cận.
    *   Xử lý trường hợp 2 đường cong cắt nhau tạo thành 2 miền diện tích riêng biệt (phải chẻ tích phân).

*   [ ] **4. Dạng 3: Kỹ năng đọc hiểu đồ thị và tư duy hình học**
    *   Bài toán cho sẵn hình vẽ, ẩn đi một phần hoặc toàn bộ biểu thức giải tích.
    *   Sử dụng hình vẽ để xác định tính trên/dưới của các đường cong $\Rightarrow$ Bỏ dấu giá trị tuyệt đối mà không cần giải phương trình.
    *   *Kỹ thuật trình bày:* Mã hóa `pgfplots` để tạo các miền gạch sọc (pattern) phức tạp.

*   [ ] **5. Dạng 4: Mô hình hóa Toán học (Bài toán thực tiễn)**
    *   Gắn hệ trục tọa độ $Oxy$ vào các công trình kiến trúc (cổng hình Parabol, cửa sổ Elip, mặt cắt đường hầm).
    *   Tính toán chi phí nguyên vật liệu (lát gạch, sơn tường, làm kính) dựa trên diện tích tích phân.

---

### 🔵 Bài 2: Thể tích vật thể và Khối tròn xoay (Dự kiến 16 trang)
**Mục tiêu:** Phát triển năng lực tưởng tượng không gian. Phân định rạch ròi khái niệm "Thể tích vật thể biết diện tích thiết diện" và "Thể tích khối tròn xoay".

*   [ ] **1. Nền tảng Lý thuyết & Định lý cơ bản**
    *   Định lý tính thể tích vật thể $V = \int_a^b S(x) dx$ (Nhấn mạnh: KHÔNG có $\pi$, KHÔNG có bình phương).
    *   Công thức thể tích khối tròn xoay quanh trục $Ox$: $V = \pi \int_a^b f^2(x) dx$.
    *   *Kỹ thuật trình bày:* Sử dụng thư viện đồ họa 3D trong TikZ để vẽ phác thảo thiết diện cắt ngang và khối tròn xoay.

*   [ ] **2. Dạng 1: Tính thể tích vật thể có diện tích mặt cắt ngang $S(x)$**
    *   Thiết lập hàm diện tích $S(x)$ khi thiết diện là các hình cơ bản: Hình vuông, Tam giác đều, Nửa hình tròn phụ thuộc vào biến $x$.
    *   Rèn luyện kỹ năng tính toán tích phân nguyên hàm cơ bản.

*   [ ] **3. Dạng 2: Khối tròn xoay giới hạn bởi 1 đường cong và trục $Ox$**
    *   Áp dụng trực tiếp công thức. Các bài tập rèn kỹ năng khai triển hằng đẳng thức hoặc sử dụng tích phân từng phần/đổi biến số sau khi bình phương hàm $f(x)$.

*   [ ] **4. Dạng 3: Khối tròn xoay tạo bởi hình phẳng giới hạn bởi 2 đường cong**
    *   Công thức vòng đệm (Washer method): $V = \pi \int_a^b |f^2(x) - g^2(x)| dx$.
    *   Cảnh báo sai lầm kinh điển của học sinh: Tránh nhầm lẫn giữa $\pi \int |f^2 - g^2|$ và $\pi \int (f - g)^2$.

*   [ ] **5. Dạng 4: Ứng dụng thực tiễn - Tối ưu hóa trong thiết kế**
    *   Tính thể tích chất lỏng trong bồn chứa nằm ngang/thẳng đứng.
    *   Tính dung tích của các vật dụng sinh hoạt (cốc thủy tinh, chao đèn, vòm nón, thùng rượu vang).

---

### 🟣 Bài 3: Kiểm tra, Đánh giá năng lực (Dự kiến 12 trang)
**Mục tiêu:** Tổng hợp kiến thức, rèn luyện áp lực thời gian và làm quen với cấu trúc đề thi tốt nghiệp THPT từ năm 2025 theo chuẩn Công văn 7991/BGDĐT-GDTrH.

*   [ ] **1. Sơ đồ tư duy (Mindmap Tổng kết)**
    *   Vẽ sơ đồ khối bằng `TikZ` tóm tắt toàn bộ công thức cốt lõi.

*   [ ] **2. Phần I: Cấu trúc trắc nghiệm nhiều phương án lựa chọn**
    *   Số lượng: 15 - 20 câu. Tập trung kiểm tra mức độ Biết - Hiểu. Yêu cầu phản xạ nhanh với công thức và kỹ năng bấm máy tính cầm tay.
    *   *Trình bày:* Bố cục 2 cột gọn gàng.

*   [ ] **3. Phần II: Cấu trúc trắc nghiệm Đúng/Sai**
    *   Số lượng: 3 - 4 cụm bài toán (mỗi cụm 4 ý a, b, c, d).
    *   Tập trung vào các câu hỏi phân tích đồ thị phức tạp. Yêu cầu học sinh phải lập luận tính đúng sai của các biểu thức tích phân được gài bẫy tinh vi.

*   [ ] **4. Phần III: Cấu trúc trắc nghiệm Trả lời ngắn**
    *   Số lượng: 4 - 6 câu.
    *   Toàn bộ là các bài toán mô hình hóa thực tế hoặc tính toán phức tạp đòi hỏi ra đáp án cuối cùng (làm tròn số theo quy định). Loại bỏ hoàn toàn tư duy thử đáp án.

---

## PHẦN III: TIÊU CHUẨN KỸ THUẬT VÀ NGHIỆP VỤ $\LaTeX$ (Quality Assurance)

Để văn bản đạt chất lượng xuất bản thương mại (Publishing-grade), người biên soạn phải cam kết tuân thủ các quy tắc sau:
1.  **Zero Warnings:** Triệt tiêu hoàn toàn các lỗi `Overfull \hbox` và `Underfull \hbox` bằng cách kiểm soát ngắt dòng và độ rộng của các phương trình Toán học.
2.  **Đồ họa thuần túy (Native Graphics):** 100% hình học, đồ thị hàm số và mô hình 3D phải được render trực tiếp bằng mã `TikZ`/`pgfplots`. Tuyệt đối **không** dùng lệnh `\includegraphics` để chèn ảnh bitmap (`.png`, `.jpg`) cắt từ các phần mềm ngoại lai.
3.  **Tự động hóa số liệu:** Sử dụng bộ đếm (counters) tự động cho toàn bộ hệ thống Câu hỏi, Ví dụ, Định lý. Không gõ chay số thứ tự để dễ dàng xáo trộn hoặc bổ sung ngân hàng đề sau này.
