# Quy trình làm phim AI – Topview

> v0.6 – **khung 6 Gate, B1 và bộ thông số chuẩn đã chốt**. Đang duyệt B2 Kịch bản (`gates/gate-1-b2-kich-ban.md`). Tài liệu Gate 1: `gates/gate-1-phat-trien.md` (quy trình B1), `gates/gate-1-thong-so.md` (thông số chuẩn). Khi mọi Gate được chốt, toàn bộ sẽ được đóng thành skill.

## Nguyên tắc đã chốt

1. Đây là quy trình làm **phim AI theo hướng điện ảnh**, không phải phim quay thật.
2. **Claude làm, bạn chốt.** Claude thực hiện mọi bước; bạn chỉ duyệt ở các điểm chốt. Claude không sang bước sau khi chưa có "chốt".
3. Phần nào của phim truyền thống không cần cho phim AI thì **loại bỏ hoặc gộp lại**.
4. Cách làm việc: chốt khung lớn trước, sau đó mới đi sâu từng bước.
5. Sáu giai đoạn gọi là **Gate 1 → Gate 6**. Phải chốt xong Gate trước mới được sang Gate sau.
6. Bên trong mỗi Gate có các **điểm chốt** nhỏ; "Gate" chỉ dùng cho giai đoạn lớn.
7. **Cuối mỗi tin nhắn** luôn có checklist các mục đã chốt và các mục đang chờ chốt.
8. **Bộ thông số chuẩn** (`gates/gate-1-thong-so.md`) áp dụng cho mọi dự án; không tra cứu lại mỗi lần. Chỉ hiệu chỉnh khi bạn yêu cầu hoặc sau dự án thử (luật L9).
9. **Gate 1 gồm B1 (6 bước) và B2 (4 bước): 10 bước, 5 điểm chốt.** Chi tiết B2 ở `gates/gate-1-b2-kich-ban.md`.
10. **Lựa chọn của dự án** (hồ sơ/thời lượng, ngôn ngữ, kiểu lời, tỉ lệ khung…) **hỏi ở từng dự án** theo `gates/gate-1-phieu-brief.md`, kèm lời khuyên theo ý tưởng, rồi khóa cho dự án đó (luật L10). Thông số chuẩn thì không hỏi lại (L9).
11. **Bộ công cụ do từng dự án quyết định** (luật L11): ví dụ YouTube dùng Nano Banana Pro + Gemini Omni Flash; film thi giải/điện ảnh dùng Topview hoặc CapCut/Dreamina nhưng ảnh tham chiếu và storyboard vẫn Nano Banana Pro; model video chọn theo từng shot. Năng lực và giới hạn từng model ở `gates/cong-cu-va-model.md`.

## Khung quy trình: 6 Gate, 9 bước

| Gate | Bước | Claude làm | Điểm chốt |
|---|---|---|---|
| **Gate 1 – Phát triển** | **B1. Ý tưởng → treatment** | 6 bước từ ý tưởng thô đến treatment (xem `gates/gate-1-phat-trien.md` và `gates/gate-1-thong-so.md`) | Brief, chọn concept, duyệt treatment |
| | **B2. Kịch bản** | Kịch bản + bảng bóc tách (nhân vật, bối cảnh, đạo cụ, trang phục) | Chốt kịch bản |
| **Gate 2 – Thiết kế** | **B3. Visual bible & tài sản** | 3a: 2–3 hướng phong cách (style frame, bảng màu, ánh sáng, ống kính). 3b: sheet nhân vật (xoay 360°, biểu cảm, trang phục), bối cảnh, đạo cụ | 3a: chọn phong cách. 3b: duyệt từng tài sản |
| | **B4. Giọng & thoại** | Chọn giọng cho từng nhân vật, tạo toàn bộ thoại, đo thời lượng | Duyệt giọng và thoại |
| **Gate 3 – Dựng trước** | **B5. Storyboard & animatic** | Shot list (mã shot, thời lượng, cỡ cảnh, chuyển động máy, model, ước tính credit), storyboard nháp, animatic ghép thoại + nhạc tạm | **Chốt animatic + ngân sách credit** (điểm chốt quan trọng nhất) |
| **Gate 4 – Sản xuất** | **B6. Keyframe** | Ảnh hoàn chỉnh cho từng shot, đối chiếu với sheet nhân vật | Duyệt keyframe theo từng cảnh |
| | **B7. Video hóa** | Ảnh → video, lipsync, đổi phong cách nếu cần, sửa lỗi và tạo lại | Duyệt take theo từng cảnh |
| **Gate 5 – Hậu kỳ** | **B8. Hậu kỳ tổng hợp** | Dựng theo animatic, SFX, ambience, nhạc, mix, đồng bộ màu giữa các model, upscale, phụ đề, credit cuối | Chốt bản master |
| **Gate 6 – Phát hành** | **B9. Phát hành** | Bản cho từng nền tảng (16:9, 9:16), trailer/teaser, thumbnail, caption, nhãn AI | Chốt gói phát hành |
| **Xuyên suốt** | **Hồ sơ dự án** | Đặt tên file, phiên bản, nhật ký prompt/model/seed, theo dõi credit, nhật ký quyết định, lưu trữ | – |

B3 và B4 có thể chạy song song.

## Phần của phim truyền thống bị loại hoặc gộp

| Phim truyền thống | Ở phim AI |
|---|---|
| Casting diễn viên | Gộp vào B3 (thiết kế nhân vật) và B4 (chọn giọng) |
| Khảo sát bối cảnh, xin phép quay, dựng set | Gộp vào B3 (tạo bối cảnh) |
| Phục trang, đạo cụ, hóa trang | Gộp vào B3 |
| Tập dượt, blocking diễn viên, previs 3D riêng | Gộp vào B5 |
| Lịch quay, call sheet, quản lý đoàn, thuê thiết bị | Loại bỏ; thay bằng ngân sách credit ở B5 |
| Quay chính | Thay bằng B6 + B7 |
| Dailies, giám sát liên tục (script supervisor) | Thay bằng điểm chốt + đối chiếu sheet nhân vật |
| Thu âm hiện trường, ADR, Foley | Loại bỏ; thay bằng thoại AI (B4) và SFX AI (B8) |
| Dựng, âm thanh, màu, VFX là các bộ phận riêng | Gộp thành một bước B8 |
| Bảo hiểm, hợp đồng đoàn, hậu cần | Loại bỏ |
| DIT / quản lý thẻ nhớ | Thay bằng hồ sơ dự án xuyên suốt |

## Phần riêng của phim AI được thêm vào

- **Khóa nhất quán:** sheet nhân vật và bối cảnh ở B3 là "nguồn chuẩn" cho mọi shot.
- **Keyframe trước, video sau:** duyệt ảnh rẻ trước khi tốn credit tạo video.
- **Nhật ký prompt:** mỗi shot ghi lại prompt, model, seed, phiên bản được chọn.
- **Ngân sách credit:** ước tính ở B5, giới hạn số lần tạo lại mỗi shot.
- **QC lỗi AI:** tay, mặt, biến dạng, nhấp nháy, chữ, nhân vật bị lệch.
- **Pháp lý:** giấy phép thương mại của công cụ, không dùng mặt/giọng người thật, gắn nhãn AI.

## Cách một điểm chốt hoạt động

1. Claude trình bày sản phẩm của bước, kèm các phương án nếu có.
2. Claude báo trước chi phí credit của bước tiếp theo.
3. Bạn trả lời **"chốt"** hoặc **"sửa: …"**.
4. Nếu sửa một thứ đã chốt, Claude ghi vào nhật ký quyết định và báo những bước phía sau phải làm lại.

## Điều kiện để Claude tự làm được

- **Văn bản** (ý tưởng, kịch bản, bóc tách, shot list, prompt, hướng dẫn giọng, danh sách dựng): Claude làm được ngay.
- **Tạo ảnh, video, giọng, nhạc:** cần kết nối công cụ (ví dụ plugin Topview sau khi bạn cho phép cài và đăng nhập OAuth). Khi chưa kết nối, Claude chuẩn bị gói prompt sẵn để dán, bạn bấm tạo và gửi kết quả lại để Claude kiểm tra.
- **Kiểm tra chất lượng:** Claude xem được ảnh; với video, Claude trích khung hình để kiểm tra.

## Gate 2 – Thiết kế

Đang duyệt: `gates/gate-2-thiet-ke.md` (B3 Visual bible và tài sản, B4 Giọng và thoại; 5 bước, 3 điểm chốt CHỐT 6, 7, 8). Gate 1 đã xong phần đặc tả; gói bàn giao Gate 1 là bản tạm thời, chỉnh lại sau khi chạy dự án thử thật.

## Dữ liệu bạn nhận khi Gate 1 kết thúc

Mô tả và dữ liệu mẫu ở `gates/gate-1-goi-ban-giao.md`: brief, concept, bảng điểm, lõi truyện, beat sheet, treatment, danh sách cảnh, ngân sách lời, kịch bản, bảng bóc tách và nhật ký quyết định. Chưa có ảnh, giọng, storyboard hay video (các Gate sau).

## Việc để lại cho Gate 2: đo tốc độ giọng thật

Sau khi chọn giọng ở B4, tạo đoạn mẫu 20–30 giây bằng chính giọng đó, đo tốc độ thật (đơn vị/giây của ngôn ngữ phim) và tính lại ngân sách lời của mọi cảnh; cảnh nào vượt thì quay lại bước 2.3 cắt lời. Tiếng Hàn và tiếng Tây Ban Nha chưa có số tốc độ đáng tin nên bắt buộc đo mẫu. Chi tiết: `gates/gate-1-b2-kich-ban.md`, mục 3.1.

## Việc để lại cho Gate 3: Bảng chọn công cụ

Chưa quyết ở Gate 1. Gate 3 phải chốt trọn vẹn: model ảnh (ảnh tham chiếu nhân vật, bối cảnh, storyboard) và model video theo từng loại cảnh; độ dài clip tối đa (phụ thuộc độ phân giải và chế độ sinh), âm thanh/lipsync (độ khớp miệng giảm sau khoảng 6–7 giây), giữ nhất quán, đơn giá credit; từ đó chốt độ dài shot thật và kiểm lại giả định "clip tối đa 8 giây" dùng cho thoại khớp miệng ở B2. Chi tiết: `gates/gate-1-thong-so.md` mục 5 và `gates/gate-1-b2-kich-ban.md` mục 3.2.

## Câu hỏi còn mở

1. "Style Transformation" trong khóa học bạn theo làm gì cụ thể?
2. Định dạng chính: phim ngắn ngang, microdrama dọc, hay cả hai?
3. Công cụ chính: Topview, hay giữ trung lập về công cụ?
