# Gate 1 – B2 Kịch bản (v0.1 – CHỜ DUYỆT)

> Phần tiếp theo của `gate-1-phat-trien.md` (B1). Thông số lấy từ `gate-1-thong-so.md`, áp dụng luật L9. Nhãn độ tin cậy: **[ĐÃ KIỂM CHỨNG]**, **[SUY RA]**, **[GIẢ ĐỊNH]**, **[ĐỀ XUẤT]**.

## 1. Mục tiêu và vị trí

B2 biến bộ nguyên liệu của B1 thành **kịch bản làm hình được**, kèm **bảng bóc tách** để Gate 2 thiết kế nhân vật, bối cảnh và giọng. B2 gồm **4 bước, 2 điểm chốt mới (CHỐT 4 và CHỐT 5)**. Cả Gate 1 vì vậy có 10 bước, 5 điểm chốt, và chỉ đóng khi cả 5 đã ĐÃ CHỐT.

```
Nguyên liệu B1 → 2.1 Danh sách cảnh [CHỐT 4] → 2.2 Ngân sách lời nói → 2.3 Viết kịch bản → 2.4 Kiểm tra & bóc tách [CHỐT 5] → Gate 2
```
Từ 2.2 đến 2.4 mình chạy liền và trình cùng lúc ở CHỐT 5 (bạn vẫn chốt được từng phần).

## 2. Đầu vào

Chín nguyên liệu bàn giao từ B1: brief, ý gốc + "giữ nguyên", lõi truyện, beat sheet, treatment, danh sách bóc tách sơ bộ, bảng cờ đỏ AI + cách giải, ước tính số lần tạo, nhật ký quyết định.

## 3. Nguyên tắc viết (có nguồn)

| Nguyên tắc | Độ tin cậy |
|---|---|
| Mỗi cảnh phải **đổi một giá trị** (từ hy vọng sang tuyệt vọng, bình yên sang hỗn loạn…). Cảnh nào bắt đầu và kết thúc giống nhau là thừa | [ĐÃ KIỂM CHỨNG: No Film School, TripTee] |
| Mỗi cảnh có **mong muốn** và **xung đột**; cảnh phải đẩy truyện hoặc làm lộ nhân vật | [ĐÃ KIỂM CHỨNG] |
| **Vào cảnh muộn, ra cảnh sớm** (Syd Field, William Goldman) | [ĐÃ KIỂM CHỨNG] |
| Hành động viết ở **thì hiện tại**, chỉ tả cái **nhìn thấy và nghe thấy**, không nội tâm ("anh ấy thấy bị phản bội" không có giá trị; "anh đặt chìa khóa lên bàn rồi bước ra" thì có) | [ĐÃ KIỂM CHỨNG] |
| Đoạn hành động **tối đa 3–4 dòng**; không chỉ dẫn máy quay hay chuyển cảnh trong kịch bản (việc của đạo diễn) | [ĐÃ KIỂM CHỨNG] |
| Cho video AI: mỗi dòng **một chủ thể, một hành động chính (một động từ)**; cảm xúc gắn với biểu cảm hoặc cử chỉ nhìn thấy được | [ĐÃ KIỂM CHỨNG] (blog của các nhà cung cấp công cụ, độ tin cậy trung bình) |
| **1 trang ≈ 1 phút** (trung bình, không chính xác) | [ĐÃ KIỂM CHỨNG: Final Draft, No Film School] |
| Tiếng Việt đọc khoảng **5,2 âm tiết/giây**; voice-over tiếng Anh khoảng 150 từ/phút (tài liệu 110–130, quảng cáo 140–190) | [ĐÃ KIỂM CHỨNG: Pellegrino 2011; Bunny Studio] |
| Thoại điện ảnh có nhịp nghỉ: dùng **4,5 âm tiết/giây** | [SUY RA] từ 5,2 trừ khoảng nghỉ; hiệu chỉnh ở Gate 2 bằng giọng thật |

**Cách đếm tiếng Việt:** 1 tiếng (chữ cách nhau bằng khoảng trắng) = 1 âm tiết. Ví dụ "Ba ơi, đồng hồ chạy lại rồi." = 7 tiếng ≈ 1,6 giây.

---

## 4. Bốn bước

### Bước 2.1 – Danh sách cảnh  ▸ ĐIỂM CHỐT 4

**Đầu vào:** beat sheet, treatment, lõi truyện, hồ sơ.

**Claude làm (nội bộ):**
1. Gán mỗi beat vào ít nhất một cảnh. **Cảnh = một địa điểm + một khoảng thời gian liên tục.**
2. Với mỗi cảnh, trả lời 5 câu: ai muốn gì · cái gì cản · giá trị đổi từ gì sang gì · kết cục khác lúc đầu ở đâu · cảnh này đẩy truyện hay làm lộ nhân vật.
3. Cảnh nào không đổi giá trị thì bỏ hoặc gộp.
4. Áp "vào muộn, ra sớm": cắt phần dẫn vào và phần thừa ở cuối.
5. Đối chiếu quy mô với bảng hồ sơ (nhân vật có sheet, bối cảnh) và các yếu tố "giữ nguyên".

**Luật và giới hạn:**
- **Số cảnh ≤ số beat** (mỗi cảnh chứa ít nhất một beat) và **≥ số cặp (bối cảnh, mốc thời gian) khác nhau**. Trần số cảnh theo hồ sơ chính là trần số beat ở bảng 3.5 của `gate-1-thong-so.md`.
- **Tổng giây các cảnh = tổng giây beat sheet ±5%**; từng cảnh ghi giây riêng và cộng lại phải bằng tổng.
- Không thêm nhân vật, bối cảnh hoặc tình tiết ngoài beat sheet đã chốt (L2).

**Mỗi cảnh ghi:** mã cảnh (C01…) · tiêu đề cảnh (NỘI/NGOẠI – địa điểm – thời gian) · mã beat · giây · nhân vật có mặt · đạo cụ then chốt · mong muốn · cản trở · giá trị đổi (từ → sang) · cờ AI liên quan.

**Đầu ra:** `P01_G1_2.1_danh_sach_canh_v1.md` (bảng).

**Điều kiện đạt:** mỗi beat nằm trong ít nhất một cảnh · mỗi cảnh đổi một giá trị · số cảnh trong giới hạn · tổng giây khớp ±5% · quy mô trong trần hồ sơ.

**Bạn làm:** `chốt` hoặc `sửa: …`.

### Bước 2.2 – Ngân sách lời nói

**Mục đích:** thoại và voice-over quyết định độ dài shot và khẩu hình, nên phải tính trước khi viết.

**Claude làm (nội bộ):** với mỗi cảnh quyết định ai nói, loại lời (thoại / voice-over / không lời), số câu, và số giây có lời; từ đó tính trần âm tiết.

**Luật và giới hạn:**
- **Trần âm tiết của cảnh = số giây có lời × 4,5** [SUY RA].
- **Tỉ lệ giây có lời trên tổng thời lượng:** hồ sơ B và D ≤ **70%**; hồ sơ A, C, E, F ≤ **50%** [GIẢ ĐỊNH].
- Mỗi câu thoại ≤ **20 tiếng** [GIẢ ĐỊNH].
- Tối đa **2 lượt thoại qua lại liên tiếp** (cách giải của cờ F2).
- Số nhân vật có thoại ≤ trần hồ sơ.
- Mặc định **ưu tiên voice-over hoặc không lời** nếu brief không yêu cầu thoại, vì thoại nhiều người là cờ F2 [SUY RA].
- Với nhân vật có thoại, ghi sơ bộ giọng (độ tuổi, vùng, tính cách) để Gate 2 chọn giọng.

**Đầu ra:** `P01_G1_2.2_ngan_sach_loi_v1.md` (bảng theo cảnh).

**Điều kiện đạt:** mọi cảnh có giây có lời ≤ giới hạn tỉ lệ · số câu và âm tiết ≤ trần · nhân vật có thoại ≤ trần.

### Bước 2.3 – Viết kịch bản

**Claude làm (nội bộ):** viết từng cảnh theo danh sách 2.1 và ngân sách 2.2, tuân thủ mục 3.

**Định dạng (6 thành phần chuẩn) cộng nhãn của mình:** tiêu đề cảnh · hành động · tên nhân vật · thoại · chú thích diễn xuất (chỉ khi đổi nghĩa) · chuyển cảnh (hạn chế). Sau tiêu đề cảnh thêm nhãn `[mã cảnh · beat · giây]` [ĐỀ XUẤT].

**Luật và giới hạn:**
- Mỗi dòng hành động có **một chủ thể và một hành động chính**; đoạn ≤ 3 dòng.
- Không góc máy, không nội tâm, không chuyển cảnh kỹ thuật (để Gate 3).
- Thoại đúng bảng 2.2.
- Độ dài ước tính ≈ **thời lượng (phút) trang ±25%** [SUY RA].
- Hồ sơ riêng: **microdrama** có Hook giây 0–3, một Spike (đảo chiều), Button 10–15 giây cuối [ĐÃ KIỂM CHỨNG]; **kinh dị** có midpoint ở 50% ±10% [SUY RA]; **quảng cáo** có thông điệp chính trong 3 giây đầu [ĐÃ KIỂM CHỨNG].
- Giữ các yếu tố "giữ nguyên" của ý gốc (L1).

**Đầu ra:** `P01_G1_2.3_kich_ban_v1.md`.

**Mẫu (minh họa)** – phim 60 giây "Chiếc đồng hồ của ba", cảnh đầu:
```
C01 · NỘI. PHÒNG CỦA CÔ – NGÀY                      [B1–B3 · 26 giây]

Ngăn kéo mở ra.
Chiếc đồng hồ cũ nằm trong khăn lụa. Kim dừng ở 3:07.
Cô lau bụi mặt kính bằng ngón cái.
Cô ngừng lại. Ánh mắt cô dừng ở bức ảnh người cha.
Kim giây giật một nhịp. Rồi chạy.

CÔ (VO)
Ba ơi, đồng hồ chạy lại rồi.
```
Cảnh này có 6 dòng hành động cho 26 giây (≈ 4,3 giây mỗi dòng, khớp giả định 4 giây/shot) và 1 câu 7 tiếng ≈ 1,6 giây.

### Bước 2.4 – Kiểm tra và bóc tách  ▸ ĐIỂM CHỐT 5

**Claude kiểm tra (đạt/không đạt, hiển thị cho bạn):**
1. Tổng giây cảnh = thời lượng brief ±5%; mỗi cảnh khớp beat.
2. Nhân vật có sheet, nhân vật có thoại, bối cảnh trong trần hồ sơ.
3. Mỗi cờ đỏ F1–F8 đã có cách giải được áp dụng trong văn bản; F8 = 0.
4. Mỗi dòng hành động lên hình được: không câu nào là nội tâm.
5. Âm tiết lời mỗi cảnh ≤ giây có lời × 4,5; tỉ lệ giây có lời trong giới hạn.
6. Mỗi cảnh đổi một giá trị.
7. Các yếu tố "giữ nguyên" còn đủ; logline và thông điệp thể hiện được.
8. Yêu cầu riêng của hồ sơ (microdrama, kinh dị, quảng cáo) đã đạt.
9. K1 vẫn đúng.
10. **Số dòng hành động chính ≈ tổng giây ÷ 4 (±25%).** Nếu lệch hơn, báo ngay vì nó cho biết giả định shot 4 giây có hợp thực tế không (nối với Gate 3) [SUY RA].

**Bóc tách (đầu vào cho Gate 2):**
- **Nhân vật:** tên · vai · số cảnh · có thoại không · giọng sơ bộ · ngoại hình sơ bộ (từ 1.4).
- **Bối cảnh:** mã · mô tả · cảnh dùng · thời điểm trong ngày · ánh sáng sơ bộ.
- **Đạo cụ then chốt, trang phục sơ bộ.**
- **Âm thanh then chốt:** SFX và nhạc theo cảnh.

**Đầu ra:** kịch bản v1 + `P01_G1_2.4_boc_tach_v1.md` + bảng 10 kiểm tra.

**Điều kiện đạt:** cả 10 kiểm tra đạt.

**Bạn làm:** `chốt` toàn bộ, hoặc chốt từng phần (kịch bản / bóc tách).

---

## 5. Bàn giao sang Gate 2 và Gate 3

| # | Nguyên liệu | Dùng ở |
|---|---|---|
| 1 | Kịch bản đã chốt | Gate 2 (giọng), Gate 3 (storyboard) |
| 2 | Bảng bóc tách (nhân vật, bối cảnh, đạo cụ, trang phục) | Gate 2 – B3 |
| 3 | Bảng lời nói (ai nói, âm tiết, giây) | Gate 2 – B4 |
| 4 | Danh sách cảnh (mã cảnh, beat, giây) | Gate 3 – B5 |
| 5 | Bảng cờ đỏ AI + cách giải đã áp dụng | Gate 3, Gate 4 |
| 6 | Brief và hồ sơ | Toàn bộ |
| 7 | Ước tính số lần tạo (cập nhật theo số dòng hành động) | Gate 3 |
| 8 | Nhật ký quyết định Gate 1 | Toàn bộ |

**Gate 1 đóng khi:** cả 5 điểm chốt đã ĐÃ CHỐT · 10 kiểm tra ở 2.4 đạt · cổng ra của B1 đạt · 8 nguyên liệu trên đã sẵn sàng.

## 6. Bảng độ tin cậy riêng của B2

| Thông số | Độ tin cậy |
|---|---|
| Nguyên tắc cảnh (đổi giá trị, mong muốn–xung đột, vào muộn ra sớm) | [ĐÃ KIỂM CHỨNG] |
| Quy tắc dòng hành động (hiện tại, thấy/nghe, ≤ 3–4 dòng, không góc máy) | [ĐÃ KIỂM CHỨNG] |
| Một chủ thể, một hành động mỗi dòng | [ĐÃ KIỂM CHỨNG] (nguồn nhà cung cấp công cụ) |
| 1 trang ≈ 1 phút | [ĐÃ KIỂM CHỨNG] (trung bình) |
| Tốc độ đọc tiếng Việt 5,2 âm tiết/giây | [ĐÃ KIỂM CHỨNG] |
| 4,5 âm tiết/giây cho thoại điện ảnh | [SUY RA] |
| Số cảnh ≤ số beat | Lập luận logic từ định nghĩa |
| Tỉ lệ giây có lời 50% / 70% | [GIẢ ĐỊNH] |
| Câu thoại ≤ 20 tiếng | [GIẢ ĐỊNH] |
| Độ dài kịch bản ±25% | [SUY RA] |
| Kiểm tra số dòng hành động ≈ giây ÷ 4 (±25%) | [SUY RA] |

## 7. Cần bạn chốt

- [ ] Cấu trúc B2: 4 bước, 2 điểm chốt (CHỐT 4 sau danh sách cảnh, CHỐT 5 sau kiểm tra và bóc tách)
- [ ] Ngân sách lời nói (2.2): trần 4,5 âm tiết/giây, tỉ lệ giây có lời, câu thoại ≤ 20 tiếng
- [ ] Mặc định ưu tiên voice-over hoặc không lời khi brief không yêu cầu thoại
- [ ] Kịch bản không có góc máy (để Gate 3)
- [ ] Danh sách 10 kiểm tra ở 2.4 và danh sách bàn giao

## Nguồn
- Cảnh: https://nofilmschool.com/how-to-write-a-scene · https://tripteepictures.com/articles/turn-your-scene · https://theweeklyemail.storyandplot.com/five-questions-for-every-scene/ · https://thescriptlab.com/screenwriting/script-tips/620-scenes-start-late-get-out-early/
- Hành động và định dạng: https://filmdaft.com/action-lines-in-screenplays-definition/ · https://neilchasefilm.com/how-to-write-effective-screenplay-action-lines/ · https://tonyfolden.wordpress.com/2015/03/09/write-compelling-action-lines-spec-scripts/ · https://www.studiobinder.com/blog/brilliant-script-screenplay-format/
- Kịch bản cho video AI: https://www.renderforest.com/blog/write-script-ai-video-generation · https://lumalabs.ai/news/write-ai-video-prompts
- 1 trang ≈ 1 phút: https://www.finaldraft.com/blog/does-one-page-equal-one-minute-of-screen-time · https://nofilmschool.com/one-page-equals-one-minute
- Tốc độ nói: http://www.ddl.cnrs.fr/fulltext/pellegrino/Pellegrino_2011_Language.pdf · https://www.science.org/content/article/human-speech-may-have-universal-transmission-rate-39-bits-second · https://bunnystudio.com/blog/voiceover-words-per-minute-choosing-the-ideal-information-rate/
