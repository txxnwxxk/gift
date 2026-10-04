# Gate 2 – Thiết kế: phong cách, nhân vật, bối cảnh, giọng (v0.1 – CHỜ DUYỆT)

> Nhãn độ tin cậy: **[ĐÃ KIỂM CHỨNG]** · **[SUY RA]** · **[GIẢ ĐỊNH]** · **[ĐỀ XUẤT]**. Thông số chuẩn áp dụng theo L9; lựa chọn của dự án (ngôn ngữ, công cụ…) lấy từ brief đã chốt (L10, L11).

## 1. Mục tiêu và vị trí

Gate 2 biến bộ dữ liệu của Gate 1 thành **tài sản nhìn và nghe được, khóa cho cả dự án**: phong cách hình ảnh, nhân vật, bối cảnh, đạo cụ, giọng. Hai nhánh chạy song song, có **3 điểm chốt mới (CHỐT 6, 7, 8)**.

```
Dữ liệu Gate 1 ─┬─ B3: 3.1 Visual bible [CHỐT 6] → 3.2 Nhân vật → 3.3 Bối cảnh & đạo cụ [CHỐT 7] ─┐
                └─ B4: 4.1 Ứng viên giọng [CHỐT 8] → 4.2 Tạo lời & đo thật ───────────────────────┴→ Gate 3
```

## 2. Đầu vào (từ Gate 1)

Brief (hồ sơ, tỉ lệ khung, ngôn ngữ, kiểu lời, bộ công cụ) · lõi truyện (ngoại hình sơ bộ, kiểu cung) · treatment (tone, phim tham chiếu) · bảng bóc tách (nhân vật có sheet, bối cảnh, đạo cụ, trang phục, âm thanh) · danh sách cảnh · bảng lời nói · nhật ký quyết định.

## 3. Cách vận hành khi chưa nối công cụ

Mình **không tự tạo được ảnh hay giọng** khi chưa có kết nối công cụ. Quy trình:
1. Mình soạn **gói prompt**: nội dung prompt, ảnh cần đính kèm, tên file đầu ra.
2. Bạn tạo bằng công cụ đã chọn ở brief (ví dụ Nano Banana Pro cho ảnh), rồi gửi ảnh hoặc âm thanh lại cho mình.
3. Mình **kiểm tra** (mình xem được ảnh) theo checklist và báo từng mục đạt hay không. Không đạt thì sửa trong giới hạn **3 vòng** (L6).

Khi công cụ được kết nối (ví dụ plugin Topview sau khi bạn cho phép cài), mình tự tạo thay bước 2.

---

## 4. Các bước

### Bước 3.1 – Visual bible  ▸ ĐIỂM CHỐT 6

**Mình làm (nội bộ):**
1. Từ treatment, tone và phim tham chiếu, đề xuất **2–3 hướng phong cách** [GIẢ ĐỊNH].
2. Mỗi hướng gồm các mục mà lookbook phim thường có: **bảng màu, ánh sáng, ống kính, tham chiếu hình ảnh, ghi chú tâm trạng** [ĐÃ KIỂM CHỨNG: tài liệu về lookbook], cụ thể:
   - Tên và mô tả 3 câu.
   - **Bảng màu 5–7 màu** có mã hex, mỗi màu kèm ý nghĩa cảm xúc [GIẢ ĐỊNH về số màu].
   - **Ánh sáng:** nguồn, độ cứng, nhiệt độ màu, hướng.
   - **Ống kính và độ sâu trường ảnh;** texture và grain.
   - **2–3 tham chiếu** (phim, ảnh, tranh), mỗi cái ghi rõ lấy gì.
   - **Điều không làm.**
   - **3 style frame:** nhân vật chính cận, cảnh rộng, đạo cụ then chốt (nhân vật tạm theo ngoại hình sơ bộ ở lõi truyện) [GIẢ ĐỊNH].
3. **Color script:** mỗi beat một ô màu. Màu sắc (hue) thể hiện trạng thái câu chuyện, độ bão hòa thể hiện cường độ cảm xúc: màu ấm thường gợi gần gũi, nguy hiểm, sức sống; màu lạnh gợi cô đơn, trí tuệ, điều chưa biết; bão hòa cao là hứng khởi, thấp là hoài niệm hoặc tuyệt vọng. Pixar làm 35–60 ô cho một phim dài, mỗi ô một beat chính [ĐÃ KIỂM CHỨNG]; ở phim ngắn của mình là **1 ô mỗi beat** [SUY RA].
4. **Khối prompt phong cách:** một đoạn văn cố định, **≤ 120 từ** [GIẢ ĐỊNH], dán **nguyên văn** vào mọi prompt ở các Gate sau để giữ phong cách nhất quán [SUY RA].

**Luật và giới hạn:** mỗi hướng ≤ 1 trang · không dùng tên hay hình người thật, thương hiệu, nhân vật có bản quyền (F8) · quy mô không vượt trần hồ sơ.

**Đầu ra:** `P01_G2_3.1_visual_bible_v?.md` + 3 style frame mỗi hướng.

**Điều kiện đạt:** đủ mục cho mỗi hướng · color script phủ **đủ mọi beat** · khối prompt ≤ 120 từ · mỗi hướng có danh sách "không làm".

**Bạn làm:** chọn **1 hướng** (được ghép tối đa 2 hướng). Phong cách khóa tại đây.

### Bước 3.2 – Nhân vật

**Đầu vào:** visual bible đã chốt; bảng bóc tách.

**Mình làm với mỗi nhân vật có sheet:**
1. **Ảnh nền:** toàn thân, nhìn thẳng, nét mặt trung tính, nền trơn, ánh sáng đều. **Bạn chốt ảnh nền trước** khi làm các sheet khác, vì nhất quán đến từ ảnh tham chiếu chứ không từ prompt dài [ĐÃ KIỂM CHỨNG].
2. **Bảng xoay 7 góc:** hàng trên 4 toàn thân (trước, trái, phải, sau), hàng dưới 3 chân dung (trước, trái, phải), nền trơn [ĐÃ KIỂM CHỨNG: cách làm sheet phổ biến với model ảnh]. Bỏ đạo cụ cầm tay khỏi bảng xoay, để model không "dính" đồ vật vào mọi góc [ĐÃ KIỂM CHỨNG].
3. **Bảng biểu cảm:** trung tính, vui, giận, buồn, ngạc nhiên, quyết tâm là bộ cơ bản [ĐÃ KIỂM CHỨNG]; **chỉ làm biểu cảm xuất hiện trong kịch bản, tối đa 8** [SUY RA].
4. **Trang phục:** mỗi bộ xuất hiện trong kịch bản một ảnh, ghi chú chất liệu (vải, da, kim loại…).
5. **Bảng màu hex** từng phần: da, tóc, mắt, từng món đồ [ĐÃ KIỂM CHỨNG: model sheet chuẩn có bảng màu].
6. **Tỉ lệ** so với đạo cụ hoặc bối cảnh chính (ví dụ chiều cao so với cánh cửa) [ĐÃ KIỂM CHỨNG: model sheet chuẩn có scale].
7. **Đặc điểm nhận dạng** (sẹo, phụ kiện…) phải thấy rõ ở chân dung [ĐÃ KIỂM CHỨNG].

**Luật và giới hạn:**
- Tối đa **14 ảnh tham chiếu mỗi lần sinh** và **5 nhân vật mỗi khung** (giới hạn của Nano Banana Pro) [ĐÃ KIỂM CHỨNG].
- Mỗi lần sinh **đính kèm ảnh nền và khối prompt phong cách nguyên văn**; không mô tả lại nhân vật bằng chữ.
- Không thêm nhân vật ngoài bảng bóc tách (L2).
- Mỗi sheet ≤ 3 vòng sửa.

**Kiểm tra nhất quán (6 mục, đạt hay không từng mục)** [SUY RA]: khuôn mặt · tóc · vóc dáng và tỉ lệ · trang phục · màu so với mã hex · đặc điểm nhận dạng. Kiểm giữa 7 góc và giữa các sheet. Lưu ý Nano Banana Pro không khóa được khuôn mặt 100% nên kiểm tra là bắt buộc.

**Đầu ra:** `P01_G2_3.2_nhan_vat_<tên>_v?` cho mỗi nhân vật + thư viện ảnh có tên chuẩn.

### Bước 3.3 – Bối cảnh và đạo cụ  ▸ ĐIỂM CHỐT 7

**Mình làm với mỗi bối cảnh, mỗi biến thể thời điểm/ánh sáng (theo danh sách cảnh):**
1. **Bảng bối cảnh 7 ô:** hàng trên 4 (chính diện, góc trái, góc phải, nhìn ngược lại rộng), hàng dưới 3 chi tiết quan trọng [ĐÃ KIỂM CHỨNG: bố cục location reference sheet].
2. **Gói nhất quán bối cảnh** (văn bản): vật liệu tường và sàn · đồ đạc và vị trí · vị trí cửa và cửa sổ · đạo cụ lớn · thời tiết · thời điểm trong ngày · hướng và độ mềm của ánh sáng · nguồn sáng thực · xử lý màu [ĐÃ KIỂM CHỨNG].
3. **Sơ đồ mặt bằng đơn giản:** vị trí nhân vật, hướng camera, đồ vật chính, hướng di chuyển và hướng nhìn, để tránh đồ vật "dịch chuyển" và đảo hướng màn hình [ĐÃ KIỂM CHỨNG].
4. **Đạo cụ then chốt:** mỗi đạo cụ một sheet, nhiều góc nếu cần, kèm kích thước so với tay hoặc nhân vật.

**Luật và giới hạn:** biến thể ánh sáng (ngày, tối) của cùng một địa điểm **không tăng trần bối cảnh** của hồ sơ nhưng tăng số ảnh · không thêm bối cảnh hay đạo cụ ngoài bóc tách (L2) · mỗi sheet ≤ 3 vòng sửa.

**Đầu ra:** `P01_G2_3.3_boi_canh_<tên>_<biến thể>_v?`, `P01_G2_3.3_dao_cu_<tên>_v?`.

**Điều kiện đạt (để vào CHỐT 7):** mọi nhân vật, bối cảnh, biến thể và đạo cụ trong bảng bóc tách đều có sheet · kiểm tra nhất quán 6 mục đạt · mỗi bối cảnh có sơ đồ mặt bằng.

**Bạn làm:** duyệt **từng tài sản** (`chốt nhân vật Cô, sửa phòng ngày`).

### Bước 4.1 – Ứng viên giọng  ▸ ĐIỂM CHỐT 8

**Đầu vào:** bảng lời nói; ngôn ngữ phim đã chốt ở brief.

**Mình làm:**
1. Viết **hồ sơ giọng** cho mỗi người nói (voice-over cũng tính): tuổi, giới, giọng vùng, tính cách, nhịp, cảm xúc chủ đạo.
2. Tìm **2–3 ứng viên** mỗi giọng [GIẢ ĐỊNH về số lượng]: chọn từ thư viện giọng hoặc tạo giọng theo thông số (tuổi, giới, giọng vùng, phong cách). Công cụ phải hỗ trợ ngôn ngữ của phim (kiểm tra trước) [ĐÃ KIỂM CHỨNG: ElevenLabs hỗ trợ tiếng Việt, Tây Ban Nha, Nhật, Hàn].
3. Tạo **đoạn mẫu 20–30 giây** cho mỗi ứng viên bằng câu thật trong kịch bản, **đo tốc độ thật** (đơn vị/giây của ngôn ngữ) và báo ứng viên nào làm ngân sách lời vượt (đã chốt ở B2).

**Luật và giới hạn:**
- Giọng gắn với nhân vật và dùng lại nguyên cho mọi câu; sau khi chốt, đổi giọng là cập nhật mọi câu của nhân vật đó [ĐÃ KIỂM CHỨNG: cách ElevenLabs gắn giọng vào nhân vật].
- **Không nhân bản giọng người thật khi chưa có đồng ý bằng văn bản** (coi như cờ F8). ElevenLabs yêu cầu xác nhận đồng ý; luật nhiều bang Mỹ yêu cầu đồng ý bằng văn bản [ĐÃ KIỂM CHỨNG].
- **Mục đích thương mại phải dùng gói được phép thương mại.** Gói miễn phí không được dùng thương mại và phải ghi nguồn [ĐÃ KIỂM CHỨNG: điều khoản ElevenLabs]. Điều này quan trọng với dự án YouTube có kiếm tiền.

**Đầu ra:** `P01_G2_4.1_giong_v?.md` (hồ sơ giọng, ứng viên, tốc độ đo được).

**Bạn làm:** chọn giọng (CHỐT 8).

### Bước 4.2 – Tạo lời và đo thật

**Mình làm:** tạo toàn bộ câu (lời dẫn và thoại) bằng giọng đã chốt · đo thời lượng thật từng câu · cập nhật bảng lời nói bằng giây thật · kiểm tra: tổng giây có lời ≤ trần hồ sơ, mỗi câu thoại khớp miệng ≤ 5 giây, lời mỗi cảnh ≤ ngân sách.

**Nếu có cảnh vượt:** cắt lời ở bước 2.3. Vì kịch bản đã chốt nên cần bạn xác nhận `mở lại: kịch bản`; mình báo phần bị ảnh hưởng trước (L3).

**Đầu ra:** bộ âm thanh đặt tên `P01_C01_L01` (cảnh, câu) [ĐỀ XUẤT] + bảng lời nói với giây thật.

---

## 5. Khung prompt xem trước (chưa chốt)

Dựa trên điểm mạnh và yếu của Nano Banana Pro ở `cong-cu-va-model.md`:

```
[Đính kèm: ảnh nền của nhân vật]
Mục đích: bảng xoay nhân vật 7 góc.
Bố cục: hàng trên 4 toàn thân (trước, trái, phải, sau); hàng dưới 3 chân dung (trước, trái, phải); nền trơn trung tính.
Danh tính: giữ nguyên khuôn mặt, tóc, vóc dáng, trang phục như ảnh nền; không có đạo cụ cầm tay.
Phong cách: [khối prompt phong cách từ visual bible, nguyên văn]
```
Prompt cho bối cảnh theo cùng khung, thay "danh tính" bằng "gói nhất quán bối cảnh". Prompt chi tiết sẽ soạn khi chạy dự án.

## 6. Ước tính số lần tạo ảnh [GIẢ ĐỊNH]

**Công thức:** số sheet × hệ số thử lại (×2 / ×3 / ×5, đã dùng ở Gate 1). Mỗi nhân vật 3 sheet (ảnh nền, bảng xoay, bảng biểu cảm); mỗi bối cảnh và mỗi biến thể 1 sheet; mỗi đạo cụ 1 sheet. Style frame tính riêng.

**Ví dụ (minh họa, phim 60 giây):** nhân vật Cô (3) + phòng ngày (1) + phòng tối (1) + con hẻm (1) + 4 đạo cụ (4) = **10 sheet**, nên 20 / **30** / 50 lần tạo ảnh. Cộng 9 style frame (3 hướng × 3), tổng khoảng **39** lần ở mức vừa. Chi phí credit phụ thuộc đơn giá công cụ (chưa có), ví dụ CapCut Design Studio nêu 10 lượt miễn phí mỗi ngày.

## 7. Cổng ra Gate 2 và bàn giao Gate 3

**Gate 2 đóng khi:**
- [ ] CHỐT 6, 7, 8 đều ĐÃ CHỐT
- [ ] Mọi mục trong bảng bóc tách có sheet đã chốt; số nhân vật, bối cảnh không phát sinh
- [ ] Kiểm tra nhất quán 6 mục đạt cho mọi nhân vật
- [ ] Mỗi nhân vật và bối cảnh có ảnh nền làm "neo"
- [ ] Bộ âm thanh đã đo; tổng giây có lời thật ≤ trần; mỗi câu thoại ≤ 5 giây
- [ ] Pháp lý: không dùng mặt hay giọng người thật; gói công cụ cho phép thương mại nếu cần

**Bàn giao Gate 3:** visual bible + khối prompt phong cách + color script · sheet nhân vật và ảnh nền · sheet bối cảnh và sơ đồ mặt bằng · sheet đạo cụ · bộ âm thanh và giây thật · nhật ký quyết định cập nhật.

## 8. Bảng độ tin cậy

| Thông số | Độ tin cậy |
|---|---|
| Bảng xoay chuẩn 5 góc (animation), bố cục 7 ô (4 toàn thân + 3 chân dung) trong cách làm với model ảnh | [ĐÃ KIỂM CHỨNG] |
| Bảng biểu cảm cơ bản 6 loại; model sheet có bảng màu hex, scale, callout | [ĐÃ KIỂM CHỨNG] |
| Biểu cảm chỉ làm cái dùng tới, tối đa 8 | [SUY RA] |
| Lookbook có bảng màu, ánh sáng, ống kính, tham chiếu | [ĐÃ KIỂM CHỨNG] |
| Color script (hue = trạng thái, saturation = cường độ; Pixar 35–60 ô) | [ĐÃ KIỂM CHỨNG]; 1 ô mỗi beat cho phim ngắn: [SUY RA] |
| Bảng bối cảnh 7 ô; gói nhất quán bối cảnh; sơ đồ mặt bằng | [ĐÃ KIỂM CHỨNG] |
| 14 ảnh tham chiếu, 5 nhân vật mỗi khung (Nano Banana Pro) | [ĐÃ KIỂM CHỨNG] |
| Ảnh nền làm neo, đính kèm mỗi lần sinh | [ĐÃ KIỂM CHỨNG] |
| 2–3 hướng phong cách; 3 style frame; 5–7 màu; khối prompt ≤ 120 từ; 2–3 ứng viên giọng | [GIẢ ĐỊNH] |
| 6 mục kiểm tra nhất quán | [SUY RA] |
| Điều khoản đồng ý và thương mại của giọng AI | [ĐÃ KIỂM CHỨNG] (nên đọc lại điều khoản khi dùng) |
| Ước tính số lần tạo ảnh | [GIẢ ĐỊNH] |

## 9. Cần bạn chốt

- [ ] Cấu trúc Gate 2: 5 bước, 3 điểm chốt (CHỐT 6 visual bible, CHỐT 7 tài sản, CHỐT 8 giọng)
- [ ] Bảng xoay nhân vật 7 góc; bảng bối cảnh 7 ô; biểu cảm tối đa 8
- [ ] Chốt **ảnh nền trước**, rồi mới làm các sheet khác
- [ ] Color script: 1 ô màu mỗi beat
- [ ] Cách vận hành khi chưa nối công cụ (mình soạn gói prompt, bạn tạo, mình kiểm tra)
- [ ] Luật giọng: không nhân bản giọng người thật; dùng gói được phép thương mại khi cần

## Nguồn
- Model sheet, bảng xoay: https://spines.com/character-turnaround/ · https://blog.cg-wire.com/character-sheet-animation/ · https://ezcharacter.com/character-reference-sheets · https://www.dreampixelforge.com/blog/character-turnaround
- Sheet nhân vật bằng Nano Banana: https://invideo.io/faq/how-do-you-create-a-character-reference-sheet-using-nano/ · https://www.pixelsham.com/2026/04/18/creating-a-character-sheet-for-ai-videos-using-nano-banana/ · https://blog.designhero.tv/character-sheet/ · https://selfielab.me/blog/nano-banana-pro-consistent-character-sheets-guide-20260216
- Lookbook và visual bible: https://storyflow.so/blog/how-to-make-a-lookbook-for-a-film-2026 · https://darkskiesfilm.com/what-to-include-in-a-look-book-for-film/ · https://brilliantio.com/lookbook-for-film/
- Color script: https://hyperallergic.com/the-art-of-pixar-chronicle-books/ · https://blog.prototypr.io/how-to-use-pixars-color-script-in-ux-design-1864fe7c5734 · https://colorpick.app/blog/color-film-cinematography-color-grading-guide
- Bối cảnh: https://morphic.com/resources/how-to/make-location-reference-sheet · https://invideo.io/faq/how-do-you-use-reference-images-in-ai-video-generation/ · https://tmff.net/character-consistency-in-ai-filmmaking-why-it-breaks-and-what-fixes-it/
- Giọng AI: https://elevenlabs.io/docs/help-center/product/studio/audiobooks/what-is-character-casting · https://elevenlabs.io/use-cases/ai-game-characters · https://terms.law/ai-output-rights/elevenlabs/ · https://margabagus.com/elevenlabs-voice-cloning-consent/
