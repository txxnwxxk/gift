# Gate 1 – Phát triển: từ ý tưởng thô đến bộ nguyên liệu cho kịch bản

> v0.3 – **quy trình 6 bước / 3 điểm chốt đã được đồng ý.** Các **thông số** (thời lượng, ngưỡng đạt, quy mô nhân vật, số beat…) đã được cập nhật và gắn nhãn độ tin cậy tại **`gate-1-thong-so.md`**. **Nếu hai file mâu thuẫn, ưu tiên `gate-1-thong-so.md`.** Các con số cố định trong file này (≤ 180 giây, ngưỡng 70%, ≤ 4 nhân vật…) là bản cũ và sẽ được thay khi nhập bản cuối.

---

## 0. Quy ước chung (áp dụng cho mọi bước)

### 0.1 Từ khóa của bạn
| Bạn nói | Nghĩa | Claude làm |
|---|---|---|
| `chốt` | Duyệt toàn bộ những gì đang trình | Đóng dấu ĐÃ CHỐT + ngày, sang bước tiếp |
| `chốt A, sửa B` | Duyệt một phần | Khóa A, chỉ sửa B |
| `sửa: …` | Sửa đúng chỗ chỉ định | Sửa chỗ đó, tạo bản mới (v+1), nêu rõ phần nào **không đổi** |
| `làm lại` | Bỏ bản này | Quay về đầu bước, làm bản khác |
| `mở lại: <tài liệu>` | Muốn đổi thứ đã chốt | Báo những tài liệu bị ảnh hưởng, ghi nhật ký, chờ bạn xác nhận |
| Câu khác | Thảo luận | Không đổi trạng thái tài liệu nào |

### 0.2 Trạng thái tài liệu
`NHÁP` → `CHỜ CHỐT` → `ĐÃ CHỐT (ngày)`. Claude chuyển sang CHỜ CHỐT. **Chỉ bạn** chuyển sang ĐÃ CHỐT. Tài liệu ĐÃ CHỐT bị khóa.

### 0.3 Đặt tên và lưu
`projects/P01/gate-1/P01_G1_<bước>_<tên>_v<số>.md`. Không ghi đè bản cũ; mỗi lần sửa là một phiên bản mới.

### 0.4 Luật chống lệch hướng
| # | Luật |
|---|---|
| L1 | **Ý tưởng gốc của bạn là nguồn chuẩn.** Được chép nguyên văn ở bước 1.1 và dùng để đối chiếu ở mọi bước sau |
| L2 | Sau bước 1.4, **không thêm** nhân vật, bối cảnh hoặc tình tiết lớn mà chưa hỏi bạn |
| L3 | Không đổi thứ đã chốt. Nếu phát hiện xung đột thì dừng, báo, chờ quyết định |
| L4 | Mỗi tài liệu có **giới hạn cứng** (số từ, số lượng). Vượt giới hạn thì phải rút gọn, không được bỏ qua |
| L5 | Mọi con số phải có **nguồn** hoặc nhãn **[GIẢ ĐỊNH]**. Không đoán rồi ghi như sự thật |
| L6 | Tối đa **3 vòng sửa** mỗi điểm chốt. Sang vòng 4, Claude đề xuất quay lại bước trước hoặc đổi hướng |
| L7 | Nếu bạn chọn phương án có rủi ro, Claude nêu rủi ro **một lần**, rồi làm theo bạn. Ngoại lệ: rủi ro pháp lý (F8) thì không làm |
| L8 | Mọi tin nhắn kết thúc bằng checklist: đã chốt / đang chờ chốt |
| L9 | **Bộ thông số chuẩn** trong `gate-1-thong-so.md` áp dụng cho mọi dự án; không tra cứu lại mỗi lần. Chỉ hiệu chỉnh khi bạn yêu cầu hoặc sau dự án thử |

---

## 1. Luồng tổng thể

```
Ý tưởng thô ─▶ 1.1 Brief ─▶[CHỐT 1]─▶ 1.2 Năm concept ─▶ 1.3 Chấm điểm & lọc ─▶[CHỐT 2: chọn 1]
   ─▶ 1.4 Lõi truyện ─▶ 1.5 Beat sheet ─▶ 1.6 Treatment ─▶[CHỐT 3]─▶ Bộ nguyên liệu ─▶ Gate 1 xong ─▶ B2 Kịch bản
```
Từ 1.4 đến 1.6, Claude chạy liền và trình cả ba tài liệu cùng lúc ở điểm chốt 3, theo thứ tự lõi truyện → beat sheet → treatment. Bạn có thể chốt từng phần (`chốt lõi truyện, sửa beat sheet`).

---

## 2. Chi tiết từng bước

### Bước 1.1 – Tiếp nhận ý tưởng & brief  ▸ ĐIỂM CHỐT 1

**Đầu vào:** ý tưởng thô ở bất kỳ dạng nào (câu chữ, hình, bài hát, link, cảm xúc, tin tức).

**Claude làm (nội bộ):**
1. Chép **nguyên văn** ý tưởng vào mục "Ý tưởng gốc". Không diễn giải lại.
2. Đối chiếu với 6 trường brief để xem trường nào bạn đã nói, trường nào còn thiếu.
3. Điền giá trị **mặc định** cho trường thiếu. Mỗi trường gắn nhãn `[BẠN NÓI]` hoặc `[MẶC ĐỊNH]`.
4. Chỉ hỏi những trường mà mặc định có rủi ro cao. Tối đa 6 câu, mỗi câu kèm đáp án mặc định. Nếu bạn đã nói đủ thì không hỏi.
5. Kiểm tra pháp lý sơ bộ: ý tưởng có dùng người thật, thương hiệu hoặc nhân vật có bản quyền không? Nếu có thì gắn cờ F8 ngay.

**Sáu trường brief:**
| Trường | Giá trị hợp lệ | Mặc định | Luật |
|---|---|---|---|
| Mục đích | liên hoan / kênh / quảng cáo / portfolio / khác | portfolio | – |
| Tỉ lệ khung | 16:9 · 2.39:1 · 9:16 | 16:9 | **Khóa tại đây.** Đổi sau này là làm lại từ Gate 3 |
| Thời lượng | 30–180 giây | 60 giây | Giới hạn cứng v1: **≤ 180 giây**. Dài hơn thì chia chương |
| Khán giả & ngôn ngữ | **ngôn ngữ thoại/voice-over (bắt buộc chọn)**: Việt / Anh / Tây Ban Nha / Nhật / Hàn / khác / không lời; nếu phát hành nhiều ngôn ngữ thì ghi ngôn ngữ gốc và danh sách bản địa hóa; kiểu lời: thoại / voice-over / không lời; nhóm tuổi | kiểu lời: voice-over hoặc không lời. **Ngôn ngữ không có mặc định: bạn không nói thì mình hỏi** | Ngôn ngữ quyết định cách đếm và tốc độ đọc ở bước 2.2 (đổi ngôn ngữ sau này là tính lại ngân sách lời). Ít thoại thì ít rủi ro lipsync |
| Bắt buộc / cấm | danh sách tự do | trống | Mỗi mục "cấm" là điều kiện loại ở 1.2 và 1.3 |
| Trần ngân sách | số credit hoặc USD, hoặc "chưa xác định" | chưa xác định | Không được đoán. Xem 1.5 |

**Đầu ra:** `P01_G1_1.1_brief_v1.md`, ≤ 250 từ, gồm "Ý tưởng gốc" + 6 trường + cờ pháp lý.

**Điều kiện đạt:** đủ 6 trường có giá trị · mỗi trường có nhãn nguồn · ý tưởng gốc chép nguyên văn · đã kiểm cờ pháp lý.

**Bạn làm:** `chốt` hoặc `sửa: …`.

---

### Bước 1.2 – Khai triển ý tưởng → 5 concept

**Đầu vào:** brief ĐÃ CHỐT + ý tưởng gốc.

**Claude làm (nội bộ):**
1. **Trích cảm xúc lõi:** đúng 1 từ (ví dụ: nhớ nhung, sợ hãi, hy vọng, cô đơn, kinh ngạc). Đây là thứ người xem mang về.
2. **Tách "giữ nguyên" và "tự do":** liệt kê tối đa **3 yếu tố** trong ý gốc bắt buộc giữ; phần còn lại được phép thay đổi. Gửi bạn xác nhận cùng tài liệu concept (bạn không cần chốt riêng).
3. **Sinh đúng 5 concept:**
   - **Concept A** trung thành nhất với ý gốc: giữ 100% yếu tố "giữ nguyên".
   - **B–E**: mỗi concept **chỉ xoay 1 trục**, các trục khác giữ nguyên để so sánh công bằng. Trục gồm: thể loại · góc nhìn nhân vật · câu hỏi "nếu như…" · twist · bối cảnh/thời đại.
4. **Tra cứu:** tìm 3–5 phim/video tương tự cho mỗi concept. Nếu trùng ý tưởng nổi tiếng thì gắn cờ `TRÙNG` và đổi hoặc loại.
5. **Đối chiếu mục "cấm"** trong brief. Concept nào vi phạm thì loại ngay.

**Mỗi concept gồm 6 trường:** tên tạm · logline (≤ 30 từ) · hook 3 giây đầu (1 câu tả hình) · cảm xúc lõi · khoảnh khắc hình ảnh đắt giá (1 câu) · trục xoay. Tối đa 80 từ mỗi concept.

**Đầu ra:** `P01_G1_1.2_concepts_v1.md`.

**Điều kiện đạt:** đúng 5 concept · mỗi concept đủ 6 trường · B–E mỗi cái đúng 1 trục · A giữ đủ yếu tố "giữ nguyên" · đã tra trùng, có ghi nguồn.

---

### Bước 1.3 – Chấm điểm & lọc khả thi AI  ▸ ĐIỂM CHỐT 2

**Đầu vào:** 5 concept.

**Claude làm (nội bộ):**
1. Rà **8 cờ đỏ** cho từng concept:

| Mã | Cờ đỏ | Cách giải mẫu |
|---|---|---|
| F1 | Hơn 3 nhân vật lên hình | Gộp nhân vật, hoặc để ngoài khung hình |
| F2 | Đối thoại qua lại dài | Chuyển voice-over; tối đa 2 lượt thoại liên tiếp |
| F3 | Tiếp xúc cơ thể phức tạp (đánh nhau, ôm, nhảy đôi) | Dùng bóng, che khuất, cận chi tiết, cắt cảnh |
| F4 | Tay thao tác chi tiết | Cận đồ vật thay vì tay, hoặc để tay ngoài khung |
| F5 | Đám đông tương tác | Cảnh rộng, bóng lưng, đám đông nền |
| F6 | Chữ trên hình | Thêm chữ ở hậu kỳ (Gate 5), không nhờ AI sinh chữ |
| F7 | Hành động nhanh liên tục cần khớp nhiều shot | Làm chậm, cắt vào kết quả |
| F8 | Mặt/giọng người thật, thương hiệu, nhân vật có bản quyền | **Không có mẹo. Loại hoặc thay bằng nhân vật hư cấu** |

2. Chấm 7 tiêu chí, thang 1–5, theo mốc:

| Tiêu chí (trọng số) | 1 điểm | 3 điểm | 5 điểm |
|---|---|---|---|
| Cảm xúc (×3) | Không gọi tên được cảm xúc | Gọi tên được nhưng chỉ ở một điểm | Rõ từ hook và tăng dần tới kết |
| Độc đáo (×2) | Nhiều phim tương tự | Quen nhưng có góc riêng | Tra 5 nguồn không thấy bản trùng |
| Rõ ràng (×2) | Cần giải thích mới hiểu | Hiểu sau khi đọc 2 lần | Đọc logline 1 lần là hiểu |
| Hình ảnh (×2) | Không có khoảnh khắc nào tả được bằng 1 câu | 1 khoảnh khắc | ≥ 2 khoảnh khắc và hook có hình |
| Khả thi AI (×3) | ≥ 2 cờ chưa có cách giải | 2 cờ đều đã có cách giải | 0 cờ |
| Chi phí – số tài sản (×1) | ≥ 8 tài sản | 6 tài sản | ≤ 3 tài sản |
| Hợp thời lượng (×1) | > 12 beat, hoặc phải cắt mạch truyện | 7–10 beat | ≤ 6 beat |

   - "Tài sản" = số nhân vật + số bối cảnh. Ở bước này chưa có beat sheet nên chưa tính được credit tuyệt đối; số tài sản là chỉ số thay thế.
   - Điểm Khả thi AI: 4 = 1 cờ đã có cách giải; 2 = 1 cờ chưa giải, hoặc ≥ 3 cờ đều đã có cách giải.
3. Tính **điểm % = tổng có trọng số ÷ 70**.

**Luật loại:**
- Điểm < **70%** → loại.
- Khả thi AI < 3 → loại, dù tổng điểm cao (quyền phủ quyết).
- Còn cờ đỏ chưa có cách giải → loại.
- Có cờ F8 → loại.
- **Trượt K1 hoặc K2 → loại khỏi danh sách đề xuất** (K1: điền đủ nhân vật, mục tiêu, trở ngại, cái giá; K2: hợp khán giả và hồ sơ trong brief). Hai kiểm tra này đạt/không đạt, không tính vào điểm.
- Nếu **0 concept đạt**: quay lại 1.2 tạo 5 concept mới (tối đa **2 lần**). Lần thứ 3 vẫn không đạt thì hỏi bạn.

**Đầu ra:** `P01_G1_1.3_bang_diem_v1.md`: bảng điểm 5 concept + lý do + **đề xuất tối đa 2 concept**.

**Bạn làm:** chọn 1 concept. Được **ghép tối đa 2 concept** (ví dụ "hook của B + kết của D"); Claude viết lại rồi chấm lại, phải vẫn qua các luật loại. Điểm số chỉ hỗ trợ quyết định: bạn được chọn concept điểm thấp hơn, Claude nêu rủi ro một lần (L7) rồi làm theo.

---

### Bước 1.4 – Xây lõi truyện

**Đầu vào:** concept đã chọn + brief + danh sách "giữ nguyên".

**Claude làm (nội bộ):**
1. Viết logline theo công thức cố định: *[nhân vật] muốn [mục tiêu] nhưng [trở ngại]; nếu thất bại thì [cái giá].* Kiểm tra đủ 4 thành phần.
2. Xác định nhân vật chính, lực cản, nhân vật phụ.
3. Viết Story Spine. Kiểm tra nhân quả: chèn "vì thế / nhưng" giữa các câu; câu nào chỉ nối bằng "và rồi" là lỗi, phải viết lại.
4. Đối chiếu ý gốc: các yếu tố "giữ nguyên" phải còn trong Story Spine.
5. Đếm quy mô so với giới hạn.

**Giới hạn cứng (đề xuất v1):**
| Mục | Giới hạn |
|---|---|
| Logline | 25–40 từ, 1 câu, đủ 4 thành phần |
| Thông điệp | 1 câu, ≤ 15 từ |
| Nhân vật chính | 1 (ghi: muốn gì bên ngoài / cần gì bên trong / khuyết điểm / ngoại hình 1 câu) |
| Kiểu cung nhân vật | **thay đổi** (nhân vật đổi) hoặc **phẳng** (nhân vật giữ nguyên, đi làm đổi người khác hoặc thế giới); ghi rõ chọn kiểu nào và vì sao |
| Nhân vật phụ | ≤ 2, mỗi người ghi chức năng 1 câu; bỏ nếu không đổi được kết quả |
| Nhân vật lên hình | **≤ 4**, trong đó có thoại **≤ 3** |
| Bối cảnh | **≤ 4** |
| Story Spine | 7 câu chuẩn, tối đa 8 câu; mỗi câu ≤ 25 từ; có 1–2 câu "Vì thế"; **mỗi câu gắn vào một hồi**: Ngày xưa / Mỗi ngày / Cho đến một ngày = Hồi 1; Vì thế = Hồi 2; Cho đến cuối cùng / Kể từ đó = Hồi 3 |
| Kết thúc | ghi loại (vui / buồn / mở), cảm xúc để lại, có twist hay không |

**Đầu ra:** `P01_G1_1.4_loi_truyen_v1.md`, ≤ 1 trang.

**Điều kiện đạt:** đủ mọi mục trên · không câu nào trong Story Spine là "và rồi" · các yếu tố "giữ nguyên" đều có mặt · nằm trong giới hạn quy mô.

---

### Bước 1.5 – Beat sheet có thời lượng

**Đầu vào:** lõi truyện.

**Claude làm (nội bộ):**
1. Chia truyện thành **6–12 beat** (mã B01, B02…) bám theo Story Spine.
2. Điền từng beat, phân bổ số giây theo khung tỉ lệ.
3. Tính số shot và số lần tạo ước tính.
4. Kiểm tra tổng giây, kiểm tra khoảnh khắc hình ảnh.

**Mỗi beat gồm:** mã · **hồi (1/2/3)** · **thấy gì** (≤ 25 từ) · **nghe gì** (thoại / voice-over / nhạc / SFX chính) · số giây · số shot · nhân vật có mặt · bối cảnh · cờ AI liên quan · có phải khoảnh khắc hình ảnh không.

**Đồng hồ ba hồi (đã chốt, thay bảng tỉ lệ cũ)** [ĐÃ KIỂM CHỨNG: Syd Field 25/50/25; Save the Cat 20/60/20; dung sai SUY RA]:
| Phần | Tỉ lệ |
|---|---|
| Hồi 1 – Mở đầu | 20–25% (kết thúc ở Break into Two / plot point 1) |
| Hồi 2 – Xung đột | 50–60% (midpoint ở 50% ±10%; All Is Lost ở khoảng 75%) |
| Hồi 3 – Kết | 20–25% (bắt đầu ở Break into Three, khoảng 75–80%) |
| Hook | ≤ 5 giây (phim ≤ 90 giây), nằm trong Hồi 1 |

**Luật số liệu:**
- **Tổng số giây các beat = thời lượng trong brief ± 5%.**
- **Số shot của beat = làm tròn lên (số giây ÷ 4)** [GIẢ ĐỊNH: shot trung bình 4 giây; chốt lại ở Gate 3].
- **Số lần tạo video ước tính = tổng shot × hệ số thử lại**, ghi 3 kịch bản: thấp ×2 · dự kiến ×3 · cao ×5 [GIẢ ĐỊNH; hiệu chỉnh sau khi thử ở Gate 4].
- **Chưa quy ra credit** ở bước này, vì công cụ và đơn giá chưa chốt. Khi có đơn giá thật (từ bảng giá công cụ) mới quy đổi, và ghi rõ ngày lấy giá. Nếu bạn đã cho trần ngân sách ở 1.1, Claude báo "đủ / có thể vượt / chưa tính được".
- Có từ **1 đến 3** khoảnh khắc hình ảnh đắt giá trong cả phim.

**Đầu ra:** `P01_G1_1.5_beat_sheet_v1.md` (dạng bảng).

**Điều kiện đạt:** 6–12 beat · tổng giây khớp ± 5% · tỉ lệ các phần nằm trong khung · mỗi câu Story Spine ứng với ≥ 1 beat · có ước tính 3 kịch bản, có nhãn giả định.

---

### Bước 1.6 – Treatment  ▸ ĐIỂM CHỐT 3

**Đầu vào:** lõi truyện + beat sheet.

**Claude làm (nội bộ):**
1. Viết văn xuôi, thì hiện tại, đi theo thứ tự beat.
2. Loại mọi câu tả thứ **không thể lên hình** (ví dụ "cô ấy nhớ lại…") trừ khi có cách thể hiện bằng hình hoặc voice-over.
3. Không viết chỉ dẫn máy quay (để Gate 3).
4. Ghi tone và tác phẩm tham chiếu.
5. Rút danh sách bóc tách sơ bộ.

**Giới hạn:**
| Mục | Giới hạn |
|---|---|
| Độ dài | 250–500 từ (phim ≤ 90 giây); 400–700 từ (90–180 giây) |
| Tone | ≤ 3 tính từ |
| Tác phẩm tham chiếu | 2–3, mỗi cái ghi rõ **lấy gì** (nhịp / không khí / màu / cách kể) |
| Ngôn ngữ | cùng ngôn ngữ với bạn |
| Danh sách bóc tách sơ bộ | nhân vật · bối cảnh · đạo cụ then chốt |

**Đầu ra:** `P01_G1_1.6_treatment_v1.md`.

**Điều kiện đạt:** trong giới hạn từ · mỗi beat ứng với ≥ 1 câu · không còn câu tả nội tâm không lên hình · danh sách bóc tách khớp lõi truyện.

**Bạn làm:** duyệt cả ba tài liệu (lõi truyện, beat sheet, treatment); `chốt` toàn bộ hoặc chốt từng phần.

---

## 3. Bộ nguyên liệu bàn giao cho kịch bản (B2)

| # | Nguyên liệu | Kịch bản dùng để | Bắt buộc |
|---|---|---|---|
| 1 | **Brief** ĐÃ CHỐT | Biết khung: thời lượng, tỉ lệ, ngôn ngữ, điều cấm | ✔ |
| 2 | **Ý gốc + danh sách "giữ nguyên"** | Đối chiếu, không lệch hướng | ✔ |
| 3 | **Lõi truyện** (logline, thông điệp, nhân vật, lực cản, kết, Story Spine) | Xương sống kịch bản | ✔ |
| 4 | **Beat sheet** (thấy/nghe, giây, shot) | Chia cảnh, ước lượng độ dài từng cảnh | ✔ |
| 5 | **Treatment** | Giọng kể, tone, thứ tự hình ảnh | ✔ |
| 6 | **Danh sách bóc tách sơ bộ** | Đầu vào để bóc tách chính thức ở B2 và thiết kế ở Gate 2 | ✔ |
| 7 | **Bảng cờ đỏ AI + cách giải** | Kịch bản phải viết theo cách giải đã chốt | ✔ |
| 8 | **Ước tính số lần tạo** (3 kịch bản) | Giữ độ dài kịch bản trong trần | ✔ |
| 9 | **Nhật ký quyết định Gate 1** | Biết cái gì đã chốt, cái gì đã bị loại và vì sao | ✔ |

## 4. Cổng ra Gate 1 (checklist đạt)

- [ ] Brief ĐÃ CHỐT, đủ 6 trường
- [ ] Ý gốc chép nguyên văn; mọi yếu tố "giữ nguyên" xuất hiện trong treatment
- [ ] Logline 25–40 từ, đủ 4 thành phần
- [ ] Story Spine: không câu nào chỉ là "và rồi"
- [ ] Nhân vật lên hình ≤ 4 (thoại ≤ 3), bối cảnh ≤ 4
- [ ] Beat 6–12, tổng giây khớp brief ±5%, tỉ lệ các phần trong khung
- [ ] Treatment trong giới hạn từ, chỉ tả cái thấy/nghe
- [ ] Không còn cờ đỏ chưa có cách giải; F8 = 0
- [ ] Ước tính số lần tạo ghi đủ 3 kịch bản, có nhãn [GIẢ ĐỊNH]
- [ ] Ba điểm chốt đều ĐÃ CHỐT

## 5. Thông số đề xuất cần bạn chốt

| Thông số | Đề xuất v1 |
|---|---|
| Thời lượng tối đa | 180 giây |
| Số concept | 5 |
| Ngưỡng đạt điểm | 70% |
| Trọng số | Cảm xúc 3 · Khả thi AI 3 · Độc đáo 2 · Rõ ràng 2 · Hình ảnh 2 · Chi phí 1 · Hợp thời lượng 1 |
| Nhân vật lên hình / có thoại / bối cảnh | ≤ 4 / ≤ 3 / ≤ 4 |
| Số beat | 6–12 |
| Độ dài shot giả định | 4 giây |
| Hệ số thử lại | ×2 / ×3 / ×5 |
| Số vòng sửa tối đa | 3 |

## 6. Câu hỏi mở (từ trước)

- "Style Transformation" trong khóa học nghĩa cụ thể là gì?
- Định dạng chính: ngang, dọc hay cả hai?
- Công cụ chính: Topview hay trung lập?
