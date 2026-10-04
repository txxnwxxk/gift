# Gate 1 – B2 Kịch bản (v0.2 – ĐÃ CHỐT)

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
| Tốc độ **đọc văn bản** trong thí nghiệm: tiếng Việt 5,22 · tiếng Anh 6,19 · tiếng Nhật 7,84 âm tiết/giây. Voice-over tiếng Anh trung bình khoảng 150 từ/phút (tài liệu 110–130, quảng cáo 140–190) | [ĐÃ KIỂM CHỨNG: Pellegrino 2011; Bunny Studio] |
| Thoại thật có nhịp nghỉ và diễn xuất nên chậm hơn đọc văn bản: tiếng Anh nói thường khoảng 4 âm tiết/giây (khoảng 3,3–5,9) so với 6,19, tức **hệ số 0,65** | [SUY RA] từ hai số đã kiểm chứng |

### 3.1 Ngôn ngữ của phim quyết định cách tính lời

Mỗi ngôn ngữ có tốc độ và đơn vị đếm khác nhau, nên **ngôn ngữ thoại/voice-over phải được chốt ở brief (bước 1.1)** và là đầu vào bắt buộc của bước 2.2. Công thức chung:

**Ngân sách lời của cảnh = số giây có lời × tốc độ của ngôn ngữ (đơn vị/giây).**

| Ngôn ngữ | Đơn vị đếm | Tốc độ mặc định (đã tính nhịp nghỉ) | Cơ sở | Độ tin cậy |
|---|---|---|---|---|
| Tiếng Việt | **tiếng** (chữ cách nhau bằng khoảng trắng; 1 tiếng = 1 âm tiết) | **3,4 tiếng/giây** (≈ 204 tiếng/phút) | 5,22 × 0,65; cùng bậc với khoảng 200–240 từ/phút của một nguồn tiếng Việt (độ tin cậy thấp) | [SUY RA] |
| Tiếng Anh | **từ** | **2,5 từ/giây** (voice-over, 150 từ/phút); **2,2 từ/giây** cho thoại phim (130 từ/phút) | Đo trực tiếp | [ĐÃ KIỂM CHỨNG] |
| Tiếng Nhật | **âm tiết/mora**, đếm theo kana khi đọc; chữ Hán cần bản đọc | khoảng **5,1/giây** | 7,84 × 0,65 (một nguồn khác nêu 8,03) | [SUY RA] |
| Tiếng Hàn | **âm tiết** (mỗi khối chữ Hangul = 1 âm tiết) | **chưa có số đáng tin** | Chỉ biết thứ hạng: nhanh hơn tiếng Trung, chậm hơn tiếng Nhật | thứ hạng [ĐÃ KIỂM CHỨNG]; số: đo mẫu |
| Tiếng Tây Ban Nha | từ hoặc âm tiết | **chưa có số đáng tin** | Một nguồn thứ cấp xếp vào nhóm nói nhanh (khoảng 260 từ/phút) nhưng độ tin cậy thấp nên không dùng | đo mẫu |
| Ngôn ngữ khác | tùy ngôn ngữ | đo mẫu | – | đo mẫu |

Ví dụ: "Ba ơi, đồng hồ chạy lại rồi." = 7 tiếng ≈ 2,1 giây.

**Đo mẫu theo giọng thật:** tốc độ ở bảng chỉ để lập kế hoạch trước khi chọn giọng. Sau khi chọn giọng ở Gate 2 (B4), tạo một đoạn mẫu 20–30 giây bằng chính giọng đó, đo tốc độ thật (đơn vị/giây) và tính lại ngân sách của mọi cảnh. Cảnh nào vượt thì quay lại bước 2.3 cắt lời (tính là vòng sửa). Đây là hiệu chỉnh theo giọng cụ thể, không phải tra cứu lại thông số chuẩn (L9).

**Phát hành nhiều ngôn ngữ:** bản dịch có thể dài hơn bản gốc. Từ tiếng Anh sang tiếng Tây Ban Nha hoặc Pháp thường giãn 20–25%, sang tiếng Đức tới 35%, còn tiếng Trung, Hàn, Nhật thường co lại [ĐÃ KIỂM CHỨNG: Eriksen]. Chưa có số cho tiếng Việt. [ĐỀ XUẤT] khi phát hành nhiều ngôn ngữ, chừa dư 25% thời lượng có lời cho bản dài nhất.

**Công cụ theo ngôn ngữ (xử lý ở Gate 2 và 3):** giọng AI của ElevenLabs hỗ trợ tiếng Việt, Tây Ban Nha, Nhật, Hàn (Eleven v3: 74 ngôn ngữ; v4: trên 90) [ĐÃ KIỂM CHỨNG]. Lipsync của Kling 3.0 hỗ trợ 8 ngôn ngữ nhưng nguồn không nêu danh sách, phải kiểm tra [CHƯA RÕ].

### 3.2 Độ dài clip của model và lời

**Clip (model sinh ra) khác shot (đoạn dùng trong phim).** Clip dài hơn shot thì cắt bớt; shot dài hơn clip thì phải nối clip hoặc đổi cách quay. Độ dài clip tối đa theo model [ĐÃ KIỂM CHỨNG: các bảng so sánh 2026, mức tin cậy trung bình]:

| Model | Clip tối đa |
|---|---|
| Seedance 2.5 | 4–30 giây |
| Vidu Q3 | 16 giây |
| Kling 3.0, Wan 2.7 | 15 giây (Kling: 10 giây chế độ thường, 15 giây chế độ nhiều shot) |
| Runway Gen-4.5, Luma Ray 3.2 | 10 giây |
| Veo 3.1 | 8 giây |

Độ dài còn phụ thuộc độ phân giải và tốc độ khung hình: tăng độ phân giải thường làm giảm mức trần. (Sora 2 được liệt kê 12–20 giây nhưng theo các nguồn đã ngừng hoạt động.)

**Lipsync gắn sau (công cụ riêng):** nhận âm thanh dài hơn nhiều: Kling lipsync tới 60 giây, Runway Act-Two 30 giây, Pollo 30 giây, HeyGen 10 phút, Hedra Character 3 tới 600 giây [ĐÃ KIỂM CHỨNG]. Nhưng **độ khớp miệng chỉ giữ chính xác khoảng 6–7 giây với một người nói** trong khung hình [một nguồn, độ tin cậy trung bình]. Vì vậy trần 5 giây mỗi câu vẫn hợp lý dù model sinh được clip 30 giây.

**Hai loại lời bị ràng buộc khác nhau:**
| | Thoại khớp miệng | Lời dẫn (voice-over) |
|---|---|---|
| Tạo thế nào | Cùng clip (model có âm thanh) hoặc lipsync gắn sau | Giọng AI riêng, đặt lên timeline |
| Ràng buộc bởi clip | **Có**: câu ≤ min(5 giây, clip tối đa − 3 giây) | **Không** |
| Ràng buộc bởi cảnh | Có | Có (giây có lời của cảnh) |
| Ảnh hưởng đến shot | Shot chứa thoại ≥ câu + 1 giây, nên shot không còn đều 4 giây | Chỉ cần ngắt câu ở điểm cắt khi có thể |

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

**Đầu vào bắt buộc:** ngôn ngữ thoại/voice-over đã chốt ở brief (mục 3.1). Brief chưa có thì mình hỏi trước, không tự đoán.

**Claude làm (nội bộ):** với mỗi cảnh quyết định ai nói, loại lời (thoại / voice-over / không lời), số câu, và số giây có lời; từ đó tính ngân sách lời theo tốc độ của ngôn ngữ.

**Luật và giới hạn:**
- **Ngân sách lời của cảnh = số giây có lời × tốc độ của ngôn ngữ** (bảng 3.1). Tiếng Việt mặc định 3,4 tiếng/giây [SUY RA].
- **Tỉ lệ giây có lời trên tổng thời lượng:** hồ sơ B và D ≤ **70%**; hồ sơ A, C, E, F ≤ **50%** [GIẢ ĐỊNH].
- **Thoại khớp miệng** (nhân vật nói trên hình): **mỗi câu ≤ 5 giây** (khoảng 17 tiếng Việt, khoảng 12 từ Anh) và **tổng thoại trong một clip ≤ clip tối đa của model − 3 giây**. Chưa chọn model ở bước này nên dùng giả định bảo thủ **clip tối đa 8 giây**, kiểm tra lại ở Gate 3 [SUY RA]. Shot chứa thoại phải dài ít nhất bằng câu + 1 giây [GIẢ ĐỊNH].
- **Lời dẫn (voice-over, không khớp miệng):** tạo riêng rồi đặt lên timeline nên **không bị trần độ dài clip**; chỉ bị giới hạn bởi giây có lời của cảnh. Nên ngắt câu ở điểm cắt shot; một câu có thể trải qua nhiều shot.
- Tối đa **2 lượt thoại qua lại liên tiếp** (cách giải của cờ F2).
- Số nhân vật có thoại ≤ trần hồ sơ.
- **Kiểu lời do từng dự án quyết định** (hỏi ở brief, xem `gate-1-phieu-brief.md`). Khi tư vấn, mình nghiêng về voice-over hoặc không lời vì thoại nhiều người là cờ F2 [SUY RA].
- Với nhân vật có thoại, ghi sơ bộ giọng (độ tuổi, vùng, tính cách) để Gate 2 chọn giọng.

**Đầu ra:** `P01_G1_2.2_ngan_sach_loi_v1.md` (bảng theo cảnh).

**Điều kiện đạt:** ngôn ngữ đã chốt · mọi cảnh có giây có lời ≤ giới hạn tỉ lệ · lời mỗi cảnh ≤ ngân sách · mỗi câu ≤ 5 giây · nhân vật có thoại ≤ trần.

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
C01 · NỘI. PHÒNG CỦA CÔ – NGÀY                      [B1–B3 · 22 giây]

Ngăn kéo mở ra.
Chiếc đồng hồ cũ nằm trong khăn lụa. Kim dừng ở 3:07.
Cô lau bụi mặt kính bằng ngón cái.
Cô ngừng lại. Ánh mắt cô dừng ở bức ảnh người cha.
Kim giây giật một nhịp. Rồi chạy.

CÔ (VO)
Ba ơi, đồng hồ chạy lại rồi.
```
Cảnh này có 6 dòng hành động cho 22 giây (≈ 3,7 giây mỗi dòng, trong dải ±25% của giả định 4 giây/shot) và 1 câu 7 tiếng ≈ 2,1 giây (tiếng Việt, 3,4 tiếng/giây).

### Bước 2.4 – Kiểm tra và bóc tách  ▸ ĐIỂM CHỐT 5

**Claude kiểm tra (đạt/không đạt, hiển thị cho bạn):**
1. Tổng giây cảnh = thời lượng brief ±5%; mỗi cảnh khớp beat.
2. Nhân vật có sheet, nhân vật có thoại, bối cảnh trong trần hồ sơ.
3. Mỗi cờ đỏ F1–F8 đã có cách giải được áp dụng trong văn bản; F8 = 0.
4. Mỗi dòng hành động lên hình được: không câu nào là nội tâm.
5. Lời mỗi cảnh ≤ giây có lời × tốc độ của ngôn ngữ (tạm, đo lại ở Gate 2); mỗi câu ≤ 5 giây; tỉ lệ giây có lời trong giới hạn.
6. Mỗi cảnh đổi một giá trị.
7. Các yếu tố "giữ nguyên" còn đủ; logline và thông điệp thể hiện được.
8. Yêu cầu riêng của hồ sơ (microdrama, kinh dị, quảng cáo) đã đạt.
9. K1 vẫn đúng.
10. **Số dòng hành động không thoại ≈ (tổng giây − giây thoại khớp miệng) ÷ 4 (±25%).** Nếu lệch hơn, báo ngay vì nó cho biết giả định shot 4 giây có hợp thực tế không (nối với Gate 3) [SUY RA].
11. **Tỉ lệ ba hồi khớp:** Hồi 1 20–25% · Hồi 2 50–60% · Hồi 3 20–25% · midpoint 50% ±10% [ĐÃ KIỂM CHỨNG: Syd Field, Save the Cat; dung sai SUY RA].

**Bóc tách (đầu vào cho Gate 2):**
- **Nhân vật:** tên · vai · số cảnh · có thoại không · giọng sơ bộ · ngoại hình sơ bộ (từ 1.4).
- **Bối cảnh:** mã · mô tả · cảnh dùng · thời điểm trong ngày · ánh sáng sơ bộ.
- **Đạo cụ then chốt, trang phục sơ bộ.**
- **Âm thanh then chốt:** SFX và nhạc theo cảnh.

**Đầu ra:** kịch bản v1 + `P01_G1_2.4_boc_tach_v1.md` + bảng 11 kiểm tra.

**Điều kiện đạt:** cả 11 kiểm tra đạt.

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

**Gate 1 đóng khi:** cả 5 điểm chốt đã ĐÃ CHỐT · 11 kiểm tra ở 2.4 đạt · cổng ra của B1 đạt · 8 nguyên liệu trên đã sẵn sàng.

## 6. Bảng độ tin cậy riêng của B2

| Thông số | Độ tin cậy |
|---|---|
| Nguyên tắc cảnh (đổi giá trị, mong muốn–xung đột, vào muộn ra sớm) | [ĐÃ KIỂM CHỨNG] |
| Quy tắc dòng hành động (hiện tại, thấy/nghe, ≤ 3–4 dòng, không góc máy) | [ĐÃ KIỂM CHỨNG] |
| Một chủ thể, một hành động mỗi dòng | [ĐÃ KIỂM CHỨNG] (nguồn nhà cung cấp công cụ) |
| 1 trang ≈ 1 phút | [ĐÃ KIỂM CHỨNG] (trung bình) |
| Tốc độ đọc văn bản: Việt 5,22 · Anh 6,19 · Nhật 7,84 âm tiết/giây | [ĐÃ KIỂM CHỨNG] |
| Hệ số nhịp nghỉ 0,65 (4 ÷ 6,19) và tốc độ thoại tiếng Việt 3,4 tiếng/giây | [SUY RA] |
| Tốc độ tiếng Hàn, Tây Ban Nha | Chưa có số đáng tin; đo mẫu ở Gate 2 |
| Số cảnh ≤ số beat | Lập luận logic từ định nghĩa |
| Tỉ lệ giây có lời: 50% (phim) có nguồn; 70% quảng cáo suy ra; 70% microdrama giả định | Xem mục 6.1 |
| Thoại khớp miệng mỗi câu ≤ 5 giây; tổng trong clip ≤ clip tối đa − 3 giây | [SUY RA] từ giới hạn clip và độ khớp miệng 6–7 giây; "−3 giây" là [GIẢ ĐỊNH] |
| Độ dài clip tối đa theo model (Seedance 2.5: 4–30 giây; Veo 3.1: 8 giây…) | [ĐÃ KIỂM CHỨNG] mức trung bình, đổi nhanh theo thời gian |
| Lời dẫn không bị trần clip | Lập luận từ cách làm (tạo riêng, đặt lên timeline) |
| Độ dài kịch bản ±25% | [SUY RA] |
| Kiểm tra số dòng hành động ≈ giây ÷ 4 (±25%) | [SUY RA] |

### 6.1 Nguồn gốc các con số của bước 2.2 (đã tra)

Khi viết bản đầu, phần lớn các con số này **chưa được dẫn nguồn**. Sau khi tra:

**Sửa lỗi:** bản đầu dùng trần 4,5 âm tiết/giây, tính bằng 5,2 × (130 ÷ 150). Cách tính đó sai nền: 5,2 là tốc độ đọc văn bản trong thí nghiệm, còn 130 và 150 là hai tốc độ đã có nhịp nghỉ, nên tỉ lệ giữa chúng không áp dụng được cho 5,2. Con số đúng hơn là 5,22 × 0,65 = 3,4 tiếng/giây, thấp hơn khoảng 24%.

| Con số | Nguồn / cách suy ra | Độ tin cậy |
|---|---|---|
| Đọc văn bản: Việt 5,22 · Anh 6,19 · Nhật 7,84 âm tiết/giây | Pellegrino 2011 | [ĐÃ KIỂM CHỨNG] |
| **Tốc độ thoại tiếng Việt 3,4 tiếng/giây** | 5,22 × 0,65. Hệ số 0,65 = tiếng Anh nói thường khoảng 4 âm tiết/giây ÷ 6,19 khi đọc văn bản | [SUY RA] |
| **Giây có lời ≤ 50%** (hồ sơ A, C, E, F) | Trung bình thoại chiếm dưới 50% thời lượng phim (năm 1940: 60%; năm 2005: 35,6%); phim dài thường 40–60% | [ĐÃ KIỂM CHỨNG trung bình], dùng làm trần |
| Kinh dị ≤ 35% (đề xuất mới) | Kinh dị là thể loại ít lời nhất (khoảng 6.243 từ thoại mỗi phim, so với 10.289 của phim hình sự) | [SUY RA] |
| **Giây có lời ≤ 70%** (hồ sơ B quảng cáo) | 30 giây ≈ 60–75 từ ở 2,5 từ/giây; hình sản phẩm, logo, phản ứng có thể chiếm khoảng 1/3 thời lượng mà không có lời | [SUY RA] |
| Giây có lời ≤ 70% (hồ sơ D microdrama) | **Chưa có nguồn trực tiếp.** Nguồn chỉ nêu tập 90 giây ≈ 400–600 từ cả hành động lẫn thoại, và tập 60 giây ≈ 120–150 từ | [GIẢ ĐỊNH] |
| **Thoại khớp miệng mỗi câu ≤ 5 giây** | Clip ngắn nhất trong nhóm model có âm thanh là 8 giây (Veo 3.1), trừ khoảng 3 giây cho nghỉ và phản ứng; độ khớp miệng chỉ chính xác khoảng 6–7 giây với một người nói. Tính theo giây để dùng cho mọi ngôn ngữ (≈ 17 tiếng Việt, ≈ 12 từ Anh). Chỉ áp cho thoại khớp miệng, không áp cho lời dẫn | [SUY RA] |
| Microdrama: câu dưới 12 từ | Hướng dẫn viết microdrama: dưới 12 từ mỗi câu, mỗi lượt nói tối đa 2 dòng, hành động mỗi beat ≤ 7 từ, 3–5 beat hình ảnh mỗi tập. 12 từ tiếng Anh ≈ 4,8 giây nên khớp với trần 5 giây | [ĐÃ KIỂM CHỨNG] hướng dẫn từ blog, độ tin cậy trung bình |
| Tối đa 2 lượt thoại qua lại | Cách giải do mình đặt cho cờ F2 | [GIẢ ĐỊNH] |
| Mặc định ưu tiên voice-over | Cờ F2; nghiên cứu cho biết hệ thống tạo truyện bằng AI còn thiếu tương tác và đối thoại giữa các nhân vật | [SUY RA] |
| **Cách chia giữa voice-over và thoại** | **Chưa có con số nào.** Hiện chỉ có mặc định định tính ở dòng trên | – |

**Hai điểm phát hiện thêm, để xử lý ở Gate 3:**
- Kling 3.0 cải thiện lipsync cho 8 ngôn ngữ, nhưng nguồn **không nói có tiếng Việt hay không**. Phải kiểm tra trước khi chọn làm thoại tiếng Việt.
- Theo các nguồn tìm được, **Sora 2 đã ngừng** (ứng dụng ngừng ngày 26/4/2026, API đóng ngày 24/9/2026). Không dựa vào nó khi chọn công cụ.

**Đã chốt:** ngôn ngữ và kiểu lời (voice-over hay thoại) **do từng dự án quyết định**, hỏi ở brief (L10). Cách chia voice-over/thoại theo hồ sơ chỉ dùng làm **lời khuyên khi hỏi**, không phải luật cố định (bảng trong `gate-1-phieu-brief.md`).

**Đã chốt:** trần giây có lời ≤ **35%** cho kinh dị.

## 7. Đã chốt

- [x] Cấu trúc B2: 4 bước, 2 điểm chốt (CHỐT 4 sau danh sách cảnh, CHỐT 5 sau kiểm tra và bóc tách)
- [x] Ngân sách lời nói (2.2): tính theo ngôn ngữ (mục 3.1), tỉ lệ giây có lời, mỗi câu thoại khớp miệng ≤ 5 giây, đo mẫu giọng ở Gate 2; kinh dị ≤ 35%
- [x] Tách hai loại lời: thoại khớp miệng (bị ràng buộc bởi clip) và lời dẫn (không bị ràng buộc bởi clip), mục 3.2
- [x] Kịch bản không có góc máy (để Gate 3)
- [x] Danh sách 11 kiểm tra ở 2.4 và 8 nguyên liệu bàn giao

## Nguồn
- Cảnh: https://nofilmschool.com/how-to-write-a-scene · https://tripteepictures.com/articles/turn-your-scene · https://theweeklyemail.storyandplot.com/five-questions-for-every-scene/ · https://thescriptlab.com/screenwriting/script-tips/620-scenes-start-late-get-out-early/
- Hành động và định dạng: https://filmdaft.com/action-lines-in-screenplays-definition/ · https://neilchasefilm.com/how-to-write-effective-screenplay-action-lines/ · https://tonyfolden.wordpress.com/2015/03/09/write-compelling-action-lines-spec-scripts/ · https://www.studiobinder.com/blog/brilliant-script-screenplay-format/
- Kịch bản cho video AI: https://www.renderforest.com/blog/write-script-ai-video-generation · https://lumalabs.ai/news/write-ai-video-prompts
- 1 trang ≈ 1 phút: https://www.finaldraft.com/blog/does-one-page-equal-one-minute-of-screen-time · https://nofilmschool.com/one-page-equals-one-minute
- Tốc độ nói: http://www.ddl.cnrs.fr/fulltext/pellegrino/Pellegrino_2011_Language.pdf · https://www.science.org/content/article/human-speech-may-have-universal-transmission-rate-39-bits-second · https://bunnystudio.com/blog/voiceover-words-per-minute-choosing-the-ideal-information-rate/
- Mật độ thoại: https://stephenfollows.com/p/has-the-way-movies-use-dialogue-changed · https://darkskiesfilm.com/how-many-words-are-in-a-movie/ · https://www.redsharknews.com/lets-talk-about-dialogue
- Quảng cáo và microdrama: https://www.screenweaver.ai/blog/commercial-script-length-timing · https://robertstarling.com/how-many-words-fit-in-a-30-second-commercial-a-voiceover-script-timing-guide/ · https://www.screenweaver.ai/blog/short-drama-script-format · https://www.axisaistudios.com/blog/script-structure-for-vertical-dramas-episode-by-episode-guide
- Độ dài clip và lipsync: https://wavespeed.ai/blog/posts/seedance-2-0-vs-kling-3-0-sora-2-veo-3-1-video-generation-comparison-2026/ · https://aimlapi.com/blog/best-ai-video-generators-2026-veo-3-1-kling-sora-2-seedance-more-compared
- AI thiếu đối thoại giữa nhân vật: https://arxiv.org/pdf/2508.08487
- Tốc độ nói theo ngôn ngữ: https://en.wikipedia.org/wiki/Speech_tempo · https://www.sciencedirect.com/science/article/abs/pii/S0379073815000432 · https://timviec365.vn/blog/toc-do-doc-trung-binh-cua-nguoi-viet-nam-new15516.html
- Bản dịch giãn hoặc co: https://eriksen.com/language/text-expansion/
- Giọng AI theo ngôn ngữ: https://elevenlabs.io/docs/overview/capabilities/text-to-speech · https://elevenlabs.io/blog/introducing-vietnamese-norwegian-and-hungarian
- Độ dài clip theo model: https://prompt-architects.com/blog/234-video-duration-parameters-by-model · https://www.atlascloud.ai/blog/tips/best-ai-video-generation-models-2026
- Lipsync: https://www.atlascloud.ai/blog/tips/kling-ai-lip-sync · https://invideo.io/faq/how-long-can-ai-lip-sync-stay-accurate-before-it-breaks/ · https://developers.heygen.com/docs/usage-limits · https://magichour.ai/blog/guide-to-hedra-ai
