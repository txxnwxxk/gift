# Công cụ, năng lực model và "Style Transformation" (v0.1)

> Nghiên cứu theo yêu cầu: bộ công cụ do **từng dự án** quyết định; model ảnh và model video được chọn theo việc cần làm; hiểu "Style Transformation". Phần prompt chi tiết sẽ làm ở các Gate sau, dựa trên bảng này.

**Nhãn độ tin cậy:** **[ĐÃ KIỂM CHỨNG]** có nguồn · **[SUY RA]** · **[GIẢ ĐỊNH]** · **[BẠN NÓI]** thông tin do bạn cung cấp.

**Cảnh báo về nguồn:** hầu hết nguồn là blog so sánh, trang của nhà cung cấp hoặc bài tổng hợp, **không phải thử nghiệm độc lập**. Năng lực model đổi rất nhanh (ví dụ Sora 2 đã ngừng theo các nguồn tìm được). Có chỗ các nguồn mâu thuẫn nhau (ghi rõ bên dưới). Vì vậy mỗi dự án có một **bài thử 1 shot ở đầu Gate 3** để kiểm chứng điều quan trọng nhất; việc này không phải tra lại thông số chuẩn (L9).

---

## 1. Quy tắc chọn công cụ (L11)

**Bộ công cụ do từng dự án quyết định** và được hỏi ở phiếu brief (L10). Hai bộ gợi ý từ bạn:

| Loại dự án | Ảnh (nhân vật, thế giới, storyboard) | Video | Nơi chạy |
|---|---|---|---|
| **YouTube** [BẠN NÓI] | Nano Banana Pro | Gemini Omni Flash | Trực tiếp |
| **Film thi giải / điện ảnh** [BẠN NÓI] | **Vẫn Nano Banana Pro** cho ảnh tham chiếu nhân vật, thế giới và storyboard | Chọn **theo từng shot** theo diễn biến (ví dụ cần gấp thì Seedance…) | Topview hoặc CapCut/Dreamina, dùng các model trong đó |

- **Model video chọn theo từng shot ở Gate 3** (Bảng chọn công cụ). Tiêu chí: loại cảnh (thoại, hành động, cảnh rộng, cận mặt), độ dài clip cần, có cần âm thanh hay lipsync, có cần tham chiếu không, tốc độ và ngân sách credit.
- **Nền tảng tập hợp nhiều model:** Topview có Canvas, Film Studio, Drama Studio, 3D Shot Composer, character swap, motion control, và dùng được Nano Banana Pro cho ảnh [ĐÃ KIỂM CHỨNG]. Dreamina của CapCut có Seedance 2.5 và 2.0, Seedream 5.0, Nano Banana Pro; một số nguồn còn liệt kê Sora 2 và Veo 3.1 [ĐÃ KIỂM CHỨNG, có mâu thuẫn về Sora 2]. 
- **CapCut web gồm hai không gian** [ĐÃ KIỂM CHỨNG qua kết quả tìm kiếm; chưa xem tận trang vì môi trường này chặn capcut.com và trang cần đăng nhập]:
  - **Design Studio** (`capcut.com/ai-design`, phía ảnh): Seedream 5.0, Seedream 5.0 Pro, Nano Banana 2, **Nano Banana Pro**, GPT Image 2; 2K gốc, nâng lên 4K; trang giới thiệu nêu 10 lượt miễn phí mỗi ngày.
  - **Video Studio** (phía video): canvas vô hạn thay cho timeline; ba loại dự án (Canvas, Storyboard, tự động); AI agent viết kịch bản; dựng nhân vật nhất quán; **Seedance 2.0 clip tối đa 15 giây**, sáu tỉ lệ khung; Veo và Sora ở gói trả phí; Seedance 2.0 ra mắt theo vùng (Đông Nam Á, MENA, Mỹ Latinh, châu Phi).
  - Mình chưa xác nhận bản Seedance trong CapCut đã lên 2.5 chưa (Dreamina thì có 2.5).
  - **Việc cần xác nhận trong tài khoản của bạn:** danh sách model thực tế theo vùng và gói, chi phí credit mỗi lần sinh, và giới hạn ảnh tham chiếu. Các thông tin này không có trên trang công khai nên cần bạn chụp màn hình gửi mình.

---

## 2. Ma trận năng lực

### 2.1 Model ảnh – Nano Banana Pro

| Làm tốt | Làm kém |
|---|---|
| Chữ trong ảnh dễ đọc (ngắn, tương phản cao, nêu bố cục) | Chữ dài; đôi khi "trôi" khỏi độ chân thực |
| Giữ danh tính tốt; tuân thủ prompt tốt; lặp lại nhanh | **Không khóa được khuôn mặt 100%**: mỗi lần sinh lại diễn giải khuôn mặt |
| Nhận tới **14 ảnh tham chiếu**, giữ nhất quán tới **5 nhân vật** trong bố cảnh phức tạp | Lệch nhỏ ở cảnh đông người; chi tiết texture rất nhỏ |
| Ra tới 4K; chỉnh góc máy | Không khớp từng điểm ảnh với ảnh tham chiếu (ưu tiên tự do sáng tạo) |
| Lưới storyboard **3×3 (9 góc máy)** giữ chủ thể, trang phục, ánh sáng, môi trường, chỉ đổi khoảng cách và góc | |

**Hệ quả cho prompt** [SUY RA từ các nguồn trên]:
1. **Nhất quán đến từ cách dùng ảnh tham chiếu, không phải từ prompt dài.** Ảnh nền rõ, sáng, dễ phân biệt; mỗi lần sinh đều đính kèm và nhắc ảnh nền, không mô tả lại nhân vật.
2. Chữ trong ảnh: ngắn, tương phản cao, nêu vị trí.
3. Storyboard lưới: ghi rõ "giữ nguyên chủ thể, trang phục, ánh sáng, môi trường; chỉ đổi khoảng cách và góc máy".
4. Tối đa 5 nhân vật mỗi khung hình (khớp với trần quy mô của mình). Tránh cảnh đông người.
5. Khuôn mặt vẫn có thể lệch qua các lần sinh, nên kiểm tra từng keyframe với sheet nhân vật (Gate 4).

### 2.2 Model video

| Model | Clip | Làm tốt | Làm kém hoặc lưu ý |
|---|---|---|---|
| **Gemini Omni Flash** | 3, 5, 10 giây; 720p | Âm thanh đồng bộ sinh cùng lúc; nhận hỗn hợp chữ, ảnh, âm thanh, video; chỉnh sửa theo hội thoại; giữ nhất quán nhân vật qua các lần sửa; có thể thêm tham chiếu giọng hoặc Avatar | **Không nhận âm thanh đầu vào** (không dẫn lời dẫn có sẵn vào được); video tham chiếu tối đa 3 clip × 3 giây, âm thanh của video tham chiếu bị bỏ qua; ngắn và 720p |
| **Seedance 2.5** | 4–30 giây | Tới 30 ảnh + 10 video + 10 âm thanh tham chiếu; âm thanh nhiều lớp (nền, SFX, lời) đồng bộ; chỉnh sửa, kéo dài; 4K | Sinh khá chậm (khoảng 45–90 giây mỗi clip chuẩn; chế độ Fast nhanh hơn nhưng giảm chất lượng; nguồn không nói rõ bản 2.0 hay 2.5); khớp miệng và foley lệch dần về cuối clip 15 giây (nguồn nói về bản 2.0); không giữ chuẩn giọng tham chiếu; clip 30 giây vẫn có thể mất danh tính nhân vật |
| **Seedance 2.0** | tới 15 giây | Tham chiếu tới 9 ảnh + 3 video + 3 âm thanh; âm thanh đồng bộ | Chuyển động ít chi tiết hơn (theo một nguồn) |
| **Kling 3.0** | 10 giây (15 giây chế độ nhiều shot) | **Hành động, vật lý, chuyển động nhân vật phức tạp**; mặt, tay, cơ thể tốt hơn | Dải phong cách hẹp, các cảnh dễ giống nhau. **Mâu thuẫn:** một nguồn nói không có âm thanh gốc, nguồn khác nói lipsync 8 ngôn ngữ |
| **Veo 3.1** | 8 giây | Bám prompt, ánh sáng, chất liệu, phong cách nhất quán, chất điện ảnh | Chuyển động kém chân thực hơn Kling |
| Sora 2 | 12–20 giây | – | **Đã ngừng** theo các nguồn tìm được |

[ĐÃ KIỂM CHỨNG qua các bảng so sánh 2026, độ tin cậy trung bình. Sora 2 và Seedance 2.0 trong hai nguồn khác nhau có nơi nhầm tên nhau, nên chỉ lấy những điểm nhiều nguồn trùng khớp.]

**Về "cần gấp thì dùng Seedance":** bạn đã nói đây **chỉ là ví dụ**; nguyên tắc là chọn model phù hợp với mục đích của từng shot (L11), không có model mặc định cho mọi shot. Ghi chú kèm theo: mình không tìm được dữ liệu so sánh tốc độ sinh giữa các model. Với riêng Seedance, nguồn cho thấy chế độ chuẩn không nhanh (45–90 giây) và chỉ chế độ Fast mới nhanh hơn, đổi lại giảm chất lượng. Nếu ý bạn là "cảnh nhịp nhanh, nhiều hành động" thì nguồn lại nghiêng về **Kling 3.0**. Mình cần bạn nói rõ ý.

**Hệ quả cho prompt video** [SUY RA]:
1. Mỗi clip một chủ thể, một hành động chính, một chuyển động máy [ĐÃ KIỂM CHỨNG: hướng dẫn viết prompt].
2. Dùng ảnh keyframe từ Nano Banana Pro làm khung hình đầu; không mô tả lại nhân vật bằng chữ.
3. Với model có âm thanh: thoại khớp miệng ≤ 5 giây mỗi câu (đã chốt); với Omni Flash không đưa được lời dẫn có sẵn nên lời dẫn phải làm riêng bằng giọng AI rồi đặt lên timeline.
4. Clip dài (Seedance 15–30 giây): nhân vật và khớp miệng dễ lệch về cuối, nên cắt theo shot ngắn khi cần thoại.

### 2.3 Video-to-video (đổi phong cách, đổi nhân vật)

| Công cụ | Làm gì | Giới hạn |
|---|---|---|
| Runway Aleph 2.0 | Viết lại clip có sẵn theo prompt, giữ chuyển động; nhận ảnh tham chiếu phong cách | Clip đầu vào 2–30 giây, ra tới 1080p |
| Luma Modify | Đổi phong cách, đổi bối cảnh, retexture nhân vật và đạo cụ, giữ chuyển động | – |
| Topview Character Swap, Motion Control | Thay nhân vật trong video, giữ ngôn ngữ cơ thể và biểu cảm; chuyển chuyển động sang nhân vật khác | – |
| Seedance 2.5, Gemini Omni Flash | Chỉnh sửa, kéo dài; chỉnh sửa theo hội thoại | Theo giới hạn clip ở trên |

**Rủi ro nền tảng:** trong nghiên cứu về chuyển phong cách video, **nhấp nháy và mất nhất quán theo thời gian** là khó khăn cốt lõi, đặc biệt khi chuyển động lớn hoặc có che khuất [ĐÃ KIỂM CHỨNG: nghiên cứu học thuật]. Các công cụ mới đều quảng cáo "giữ chuyển động" nhưng mình chưa thấy đánh giá độc lập.

---

## 3. "Style Transformation" nghĩa là gì?

> **Đã chốt: bỏ qua ở thời điểm này** vì chưa quan trọng với phim AI hiện tại, dù hiểu theo nghĩa A, B hay C. Phần dưới giữ lại để tham khảo; nếu cần sẽ làm kỹ thuật tùy chọn ở Gate 4.

**Mình không xác định được định nghĩa gốc của khóa học.** Slide chỉ ghi "Biến hóa phong cách hình ảnh" ở bước 6, sau âm thanh và trước hậu kỳ. Qua nghiên cứu, thuật ngữ này trong làm phim AI có ba nghĩa khả dĩ:

| Nghĩa | Làm gì | Công cụ | Xử lý trong quy trình của mình |
|---|---|---|---|
| **A. Đổi phong cách ảnh** | Áp phong cách (anime, sơn dầu, đất sét…) lên ảnh tham chiếu, keyframe | Nano Banana Pro với ảnh phong cách tham chiếu | Đã nằm ở **Gate 2** (visual bible): phong cách chốt trước khi tạo nhân vật |
| **B. Đổi phong cách video (video-to-video)** | Render lại clip đã có theo phong cách mới, giữ chuyển động | Runway Aleph, Luma Modify, Seedance/Omni edit | **Kỹ thuật tùy chọn ở Gate 4 – B7**, mỗi lần một clip ≤ 30 giây |
| **C. Đổi nhân vật hoặc chuyển động** | Thay nhân vật, chuyển động sang nhân vật khác | Topview Character Swap, Motion Control | Tùy chọn ở Gate 4 – B7 |

Mình **đang nghiêng về nghĩa B**, vì vị trí của nó trong khóa học (sau khi đã có hình và tiếng, trước hậu kỳ).

**Điều chỉnh lại một nhận định cũ của mình:** trước đây mình nói đổi phong cách sau khi có video "thường làm nhân vật lệch, nhấp nháy và tốn credit gấp đôi". Phần nhấp nháy và mất nhất quán có cơ sở trong nghiên cứu, còn **"tốn credit gấp đôi" chưa có nguồn**. Quyết định vẫn giữ: chốt phong cách ở Gate 2, dùng chuyển đổi video như kỹ thuật tùy chọn.

---

## 4. Việc tiếp theo

- **Gate 2 – B3:** prompt tạo sheet nhân vật và thế giới bằng Nano Banana Pro (dựa mục 2.1).
- **Gate 3 – B5:** prompt storyboard lưới và Bảng chọn công cụ theo từng shot (dựa mục 2.2); bài thử 1 shot.
- **Gate 4:** prompt keyframe và video theo model; kỹ thuật Style Transformation (mục 3).

## Nguồn
- Nano Banana Pro: https://magichour.ai/blog/nano-banana-pro-full-review-guide · https://arxiv.org/html/2512.15110v2 · https://help.apiyi.com/en/nano-banana-pro-face-consistency-guide-en.html · https://selfielab.me/blog/nano-banana-pro-consistent-character-sheets-guide-20260216 · https://learn.metalabs.global/p/how-to-create-cinematic-grids-with-nano-banana-pro · https://pixeldojo.ai/guides/nano-banana-pro-prompting-guide
- Gemini Omni Flash: https://ai.google.dev/gemini-api/docs/omni · https://invideo.io/faq/what-is-gemini-omni-flash-and-what-can-it-do/ · https://blog.segmind.com/gemini-omni-flash-video-generation-guide-features-examples-how-it-compares/
- Seedance: https://seed.bytedance.com/en/blog/one-take-creation-flexible-referencing-introducing-seedance-2-5 · https://www.mindstudio.ai/blog/seedance-2-5-features-explained · https://wavespeed.ai/blog/posts/seedance-2-0-review-issues-and-alternatives/ · https://atoms.dev/blog/seedance-2-5-review-30-second-ai-video-production-workflow
- So sánh Veo, Kling: https://www.aimagicx.com/blog/veo-3-vs-kling-3-vs-sora-2-april-2026-comparison · https://www.vo3ai.com/blog/kling-30-vs-sora-2-pro-vs-veo-31-motion-control-video-quality-and-production-val-2026-03-10 · https://lushbinary.com/blog/ai-video-generation-sora-veo-kling-seedance-comparison/
- Nền tảng: https://www.topview.ai/ · https://www.topview.ai/guides/character-swap · https://dreamina.capcut.com/ · https://techcrunch.com/2026/03/26/bytedances-new-ai-video-generation-model-dreamina-seedance-2-0-comes-to-capcut/
- Video-to-video: https://magichour.ai/blog/best-video-to-video-ai-tools-2026 · https://www.atlabs.ai/blog/runway-aleph-vs-luma-modify-video · https://picsart.com/ai-models/runway-aleph-2-0/ · https://arxiv.org/html/2510.07546
- Quy trình làm phim AI: https://frameo.ai/blog/ai-film-production-workflow-guide/ · https://www.deepfiction.ai/blog/ai-filmmaking-pipeline-script-to-screen-2026
- CapCut: https://www.capcut.com/tools/ai-design · https://www.capcut.com/resource/seedream-5-vs-nano-banana-pro · https://www.globenewswire.com/news-release/2026/08/10/3341889/0/en/capcut-design-studio-levels-up-new-skills-ecosystem-and-seedream-5-0-pro-model-bring-pro-grade-ai-design-to-everyone.html · https://x.com/capcutapp/status/2036943209956344181 · https://nofilmschool.com/capcut-vido-studio-seedance-2-0
