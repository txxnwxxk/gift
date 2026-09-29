# Gate 1 – Phát triển: từ ý tưởng thô đến treatment

> Bản nháp v0.1 – **chờ chốt**. Phần này gồm B1 (ý tưởng → treatment). B2 (kịch bản) sẽ phân tích sau khi B1 được chốt.

## Mục tiêu

Biến một ý tưởng thô bất kỳ (một câu, một hình ảnh, một bài hát, một cảm xúc, một tin tức) thành **bộ hồ sơ giao cho kịch bản**. Bộ hồ sơ này phải đủ rõ để Claude viết kịch bản mà không phải đoán, và đủ thực tế để làm được bằng AI trong ngân sách.

## Cơ sở nghiên cứu

- Chuỗi phát triển chuẩn của ngành phim: logline → beat sheet → treatment → kịch bản. Chốt các beat trước khi tạo hình thì mọi bước sau đều rẻ hơn, vì tạo hình có chủ đích thay vì mò ý tưởng trong model ảnh.
- Phim ngắn cần ít nhân vật, quan hệ nhân quả chặt. Story Spine của Pixar (8 câu) chỉ cần 1–2 câu "vì thế" cho phim ngắn.
- Ở các liên hoan phim AI, chất lượng kỹ thuật giữa các phim gần như ngang nhau. Thứ phân định là **độ độc đáo của ý tưởng, sự mạch lạc của câu chuyện và cảm xúc**.
- Điểm yếu hiện tại của video AI: nhân vật lệch giữa các khung, tay và chuyển động cơ thể, cảnh nhiều nhân vật tương tác và đối thoại qua lại. Ý tưởng phải được lọc theo các giới hạn này **ngay từ đầu**.

## Đã loại hoặc gộp so với phát triển phim truyền thống

| Phim truyền thống | Ở phim AI |
|---|---|
| Pitch deck gọi vốn | Loại bỏ |
| Mua / option bản quyền | Loại bỏ (chỉ kiểm tra không vi phạm) |
| Phòng biên kịch, nhiều vòng góp ý nhà sản xuất | Thay bằng 3 điểm chốt của bạn |
| Dự toán theo ngày quay | Thay bằng ước tính credit từ beat sheet |
| Casting sơ bộ, khảo sát bối cảnh sơ bộ | Chuyển sang Gate 2 |

## 6 bước và 3 điểm chốt

### Bước 1.1 – Tiếp nhận ý tưởng & brief  ▸ ĐIỂM CHỐT 1

- **Đầu vào:** ý tưởng thô ở bất kỳ dạng nào.
- **Claude làm:** hỏi nhanh 6 câu, mỗi câu có sẵn đáp án mặc định:
  1. Mục đích: liên hoan phim / kênh cá nhân / quảng cáo / portfolio
  2. Nền tảng và tỉ lệ khung: 16:9, 2.39:1, 9:16
  3. Thời lượng
  4. Khán giả: tiếng Việt / quốc tế, độ tuổi
  5. Bắt buộc có / tuyệt đối tránh
  6. Ngân sách credit tối đa
- **Đầu ra:** Brief dự án (1 trang).
- **Bạn:** chốt brief.

### Bước 1.2 – Khai triển ý tưởng

- **Claude làm:**
  - Tìm **cảm xúc lõi** của ý tưởng thô (một cảm xúc chính người xem mang về).
  - Tạo **5 concept** bằng cách xoay các trục: thể loại, góc nhìn nhân vật, câu hỏi "nếu như…", cú twist, bối cảnh/thời đại.
  - Mỗi concept gồm: tên tạm, logline, hook 3 giây đầu, cảm xúc lõi, 1 khoảnh khắc hình ảnh "đắt giá".
  - Tra cứu phim và trào lưu tương tự để tránh ý tưởng đã nhàm.
- **Đầu ra:** 5 concept.

### Bước 1.3 – Chấm điểm & lọc khả thi AI  ▸ ĐIỂM CHỐT 2

- **Claude làm:** chấm mỗi concept từ 1–5 theo 7 tiêu chí:

  | Tiêu chí | Câu hỏi |
  |---|---|
  | Cảm xúc | Người xem có cảm thấy điều gì rõ ràng không? |
  | Độc đáo | Đã thấy ý tưởng này nhiều chưa? |
  | Rõ ràng | Xem một lần có hiểu không? |
  | Tiềm năng hình ảnh | Có khoảnh khắc nào đáng chụp màn hình không? |
  | Khả thi AI | Bao nhiêu "cờ đỏ" bên dưới? |
  | Chi phí credit | Ước tính có vừa ngân sách không? |
  | Hợp thời lượng | Kể trọn được trong thời lượng đã chốt không? |

- **Cờ đỏ khả thi AI** (mỗi cờ phải có cách giải hoặc bỏ concept):
  - Hơn 3 nhân vật chính, hoặc hơn 3–4 bối cảnh
  - Đối thoại qua lại dài giữa nhiều nhân vật
  - Tiếp xúc cơ thể phức tạp: đánh nhau, ôm, nhảy đôi
  - Tay thao tác chi tiết: đánh đàn, viết chữ, sửa máy
  - Đám đông tương tác
  - Chữ trên hình (biển hiệu, màn hình, thư)
  - Hành động nhanh, liên tục, cần khớp giữa các shot
  - Mặt hoặc giọng người thật, thương hiệu thật
- **Hướng mạnh của AI** (cộng điểm): cảm xúc qua gương mặt và không khí, voice-over, cảnh rộng, thế giới kỳ ảo, chuyển động chậm, biểu tượng hình ảnh, biến hình.
- **Đầu ra:** bảng điểm + đề xuất 2 concept tốt nhất kèm lý do.
- **Bạn:** chọn 1 concept.

### Bước 1.4 – Xây lõi truyện

- **Claude làm:**
  - **Logline chuẩn:** [nhân vật] muốn [mục tiêu] nhưng [trở ngại], nếu thất bại thì [cái giá].
  - **Thông điệp:** 1 câu.
  - **Nhân vật chính:** muốn gì, thật sự cần gì, khuyết điểm. Lực cản là ai/cái gì.
  - **Kết thúc:** cảm xúc để lại, twist (nếu có).
  - **Story Spine 8 câu:** Ngày xưa… / Mỗi ngày… / Cho đến một ngày… / Vì thế… / Vì thế… / Cho đến cuối cùng… / Kể từ đó…
  - **Giới hạn quy mô:** 1 nhân vật trung tâm, tối đa 3 nhân vật có thoại, tối đa 3–4 bối cảnh.
- **Đầu ra:** Lõi truyện (1 trang).

### Bước 1.5 – Beat sheet có thời lượng

- **Claude làm:** chia truyện thành các beat, mỗi beat gồm: thấy gì, nghe gì, số giây, số shot ước tính, khoảnh khắc hình ảnh chính.
- Khung mẫu cho phim 60–90 giây:

  | Beat | Thời lượng gợi ý |
  |---|---|
  | Hook | 0–5 giây |
  | Thế giới bình thường | ~10% |
  | Biến cố | ~10% |
  | Leo thang (1–2 beat) | ~40% |
  | Cao trào | ~25% |
  | Kết / dư âm | ~10% |

- **Ước tính sơ bộ:** tổng số shot (≈ thời lượng ÷ 4 giây) và credit. Con số này sẽ được tính chính xác ở Gate 3.
- **Đầu ra:** Beat sheet.

### Bước 1.6 – Treatment  ▸ ĐIỂM CHỐT 3

- **Claude làm:** viết treatment 1–2 trang, văn xuôi thì hiện tại, mô tả những gì người xem **thấy và nghe**. Kèm tone và 2–3 tác phẩm tham chiếu (bằng chữ; moodboard hình làm ở Gate 2).
- **Bạn:** duyệt treatment.

## Bộ hồ sơ giao cho kịch bản (B2)

1. Brief dự án
2. Logline + thông điệp
3. Hồ sơ nhân vật chính và lực cản
4. Story Spine
5. Beat sheet có thời lượng và ước tính shot/credit
6. Treatment
7. Danh sách cờ đỏ AI và cách giải

## Tiêu chí đạt trước khi sang kịch bản

- [ ] Người lạ đọc logline một lần là hiểu
- [ ] Cảm xúc lõi gọi tên được bằng một từ
- [ ] Số nhân vật và bối cảnh nằm trong giới hạn
- [ ] Tổng thời lượng các beat khớp thời lượng trong brief
- [ ] Không còn cờ đỏ AI chưa có cách giải
- [ ] Ước tính credit nằm trong ngân sách

## Câu hỏi còn mở

1. 6 bước và 3 điểm chốt này đã ổn chưa?
2. 5 concept ở bước 1.2 là nhiều hay ít?
3. Khung beat mẫu nên theo thời lượng nào: 60–90 giây, 2–3 phút hay dài hơn?
