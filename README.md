# 📐 DỰ ÁN HỌC LIỆU CHUYÊN SÂU: ỨNG DỤNG HÌNH HỌC CỦA TÍCH PHÂN
**Phương pháp Sư phạm: Lấy người học làm trung tâm & Phát triển tư duy**
**Chương trình Giáo dục Phổ thông 2018 – Môn Toán 12**

**Đơn vị/Cá nhân biên soạn:** Thầy Tâm dạy Toán
**Liên hệ (Zalo):** 0837715745
**Nền tảng công nghệ:** $\LaTeX$
**Mục đích sử dụng:** Tài liệu tự học, tự khám phá dành cho học sinh.
**Phiên bản:** 2.0.0 (Tinh gọn, chú trọng vào tư duy và đường lối giải quyết vấn đề)

---

## 1. Tầm nhìn và Triết lý Sư phạm 
Tài liệu này được tái cấu trúc hoàn toàn, thoát khỏi lối mòn học vẹt hay luyện thi rập khuôn ("Mớm sẵn lý thuyết $\rightarrow$ Phân dạng mẫu $\rightarrow$ Lắp công thức"). Thay vào đó, dự án đặt học sinh vào vị trí trung tâm, trao cho các em cơ hội tự mình tìm ra bản chất tri thức thông qua chuỗi các hoạt động dẫn dắt tự nhiên.

**3 Trụ cột cốt lõi của tài liệu:**
1. **Học sinh tự tìm ra công thức:** Mở đầu mỗi bài học không phải là một định lý khô khan, mà là một **[Hoạt động khám phá]** rất trực quan (như cắt nhỏ diện tích một mảnh đất hay chia lát một ổ bánh mì) để từ đó các em tự suy luận ra khái niệm tích phân.
2. **Suy ngẫm tư duy trước, đặt bút giải sau:** Tài liệu không áp đặt ngay lời giải mẫu. Mọi bài toán đều được dẫn dắt theo chu trình rõ ràng: 
   `[Tình huống mở đầu] $\rightarrow$ [Câu hỏi gợi mở từng bước] $\rightarrow$ [Phân tích ý tưởng và đường lối] $\rightarrow$ [Lời giải chi tiết]`.
3. **Người thầy đồng hành trong từng trang sách:** Các câu hỏi gợi mở được biên soạn khéo léo như một cuộc trò chuyện 1-1, giúp học sinh biết cách tự gỡ rối, tự đặt câu hỏi và tự vượt qua khó khăn khi đang ngồi tự học ở nhà.

## 2. Cấu trúc mã nguồn $\LaTeX$ 
Vì tài liệu dành toàn bộ không gian để phát triển chuỗi tư duy và phân tích ý tưởng, cấu trúc mã nguồn đã được tinh gọn lại thành các thành phần cốt lõi sau:

```text
Chuyen-De-Tich-Phan-12/
│
├── README.md               ← Giới thiệu triết lý và định hướng của dự án
├── PLAN.md                 ← Bảng kế hoạch và phân bổ nội dung chi tiết
├── main.tex                ← File tổng hợp để biên dịch toàn bộ tài liệu
│
├── assets/                 
│   ├── style.sty           ← Cấu hình giao diện, bổ sung các hộp hội thoại: khám phá, gợi mở, ý tưởng
│   └── macros.tex          ← Các lệnh toán học viết tắt và hệ thống hình vẽ trực quan
│
├── chapters/               ← Thư mục chứa nội dung chính
│   ├── 00-loi-noi-dau.tex  ← Lời tâm tình và hướng dẫn học sinh cách tự học hiệu quả
│   ├── 01-dien-tich.tex    ← Bài 1: Hành trình khám phá diện tích hình phẳng
│   └── 02-the-tich.tex     ← Bài 2: Hành trình khám phá thể tích vật thể và khối tròn xoay
```
## 3. Tiêu chuẩn trình bày và định dạng 
Tài liệu được biên dịch bằng PDFLaTeX với hệ thống công cụ chuẩn mực:

* **Hệ thống chữ viết:** Sử dụng gói tiếng Việt truyền thống kết hợp với phông chữ mềm mại, trang nhã, mang lại cảm giác dễ chịu khi đọc.
* **Ngôn ngữ toán học:** Sử dụng các gói ký hiệu tiêu chuẩn, đảm bảo công thức hiển thị sắc nét, đúng chuẩn mực toán học phổ thông.
* **Hệ thống hình vẽ:** 100% đồ thị hàm số, hình khối không gian và mặt cắt được vẽ bằng mã lệnh toán học chuyên dụng, đảm bảo độ chính xác tuyệt đối và không bị vỡ nét khi in ấn.
* **Trình bày trực quan:** Sử dụng các hộp màu có thiết kế riêng biệt để làm nổi bật phần hoạt động khám phá, câu hỏi gợi mở và phân tích ý tưởng, giúp trang sách sinh động và mạch lạc hơn.

## 4. Hướng dẫn sử dụng và biên dịch dành cho người dạy
* **Thiết lập môi trường:** Khuyến nghị sử dụng nền tảng Overleaf hoặc phần mềm soạn thảo chuyên dụng đi kèm với hệ thống phân giải TeX đầy đủ.
* **Biên dịch tài liệu:** Mở file `main.tex` và chạy biên dịch 2 lượt để hệ thống tự động cập nhật mục lục và các liên kết chéo.
* **Quy chuẩn soạn thảo:** Các công thức toán được viết gọn gàng trong các ký hiệu phù hợp, hạn chế tối đa việc ngắt dòng thủ công để đoạn văn luôn giữ được mạch liền mạch, tự nhiên.
