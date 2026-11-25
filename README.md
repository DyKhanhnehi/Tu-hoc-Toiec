# 🪜 Bậc Thang TOEIC

Ứng dụng web học tiếng Anh **từ cơ bản đến nâng cao theo chuẩn TOEIC**, chia thành 6 bậc.
Mỗi bậc có bài kiểm tra. **Phải đạt bài kiểm tra mới được học lên bậc tiếp theo.**

- Chạy hoàn toàn trên trình duyệt, **không cần AI, không cần server, không cần đăng nhập**
- Cài lên màn hình chính iPhone / Android như một app (PWA)
- Dùng được **khi không có mạng** sau lần mở đầu tiên
- Tiến độ học được lưu ngay trên máy của người học

---

## 📚 Lộ trình 6 bậc

| Bậc | Tên | Điểm TOEIC | CEFR | Nội dung chính |
|---|---|---|---|---|
| 1 | Nền tảng | 10–250 | A1 | to be, hiện tại đơn, mạo từ, giới từ in/on/at |
| 2 | Sơ cấp | 250–400 | A2 | hiện tại tiếp diễn, quá khứ đơn, so sánh, đại từ |
| 3 | Tiền trung cấp | 400–550 | B1 | hiện tại hoàn thành, tương lai, từ loại, bị động |
| 4 | Trung cấp | 550–700 | B1+ | mệnh đề quan hệ, câu điều kiện, V-ing / to V, liên từ |
| 5 | Trung cao cấp | 700–850 | B2 | điều kiện loại 3, rút gọn mệnh đề, giả định, collocations |
| 6 | Nâng cao | 850–990 | C1 | đảo ngữ, từ dễ nhầm, chiến thuật Part 3–4 và Part 6–7 |

Tổng cộng: **24 bài học · 192 từ vựng · 234 câu hỏi** theo các dạng TOEIC Part 2, 3, 4, 5, 6, 7.

## 🔒 Quy tắc lên bậc

1. Mỗi bậc có **4 bài**, mỗi bài gồm 3 phần: **Ngữ pháp → Từ vựng → Luyện tập**.
2. Phần luyện tập đạt **≥ 60%** thì bài được tính là hoàn thành.
3. Hoàn thành đủ 4 bài thì **mở bài kiểm tra** của bậc: 15 câu, 15 phút. Mỗi đoạn nghe chỉ được nghe tối đa 2 lần.
4. Bài kiểm tra đạt **≥ 70% (11/15 câu)** thì **mở khóa bậc tiếp theo**. Chưa đạt thì làm lại.

Người đã có nền tảng có thể làm **Bài xếp lớp** (24 câu, 4 câu mỗi bậc). Bậc nào đúng ≥ 3/4 câu, và các bậc dưới cũng đạt, sẽ được mở khóa luôn.

## ✨ Tính năng

- 📖 **Ngữ pháp**: quy tắc ngắn gọn, ví dụ song ngữ và mẹo làm bài TOEIC
- 🃏 **Từ vựng**: phiên âm IPA, nút nghe phát âm, thẻ ghi nhớ lật được, đánh dấu từ đã nhớ
- 🎧 **Luyện nghe**: dùng giọng đọc tiếng Anh có sẵn trên máy, có giọng nam/nữ cho hội thoại, chỉnh được tốc độ đọc
- ✅ **Luyện tập**: có giải thích tiếng Việt ngay sau mỗi câu
- ⏱ **Bài kiểm tra**: có đồng hồ đếm ngược, tự nộp khi hết giờ, xem lại từng câu sau khi nộp
- 📒 **Sổ lỗi sai**: tự lưu các câu làm sai; ôn lại mà trả lời đúng thì câu đó được gỡ khỏi sổ
- 🔥 **Theo dõi tiến độ**: số ngày học liên tiếp, % hoàn thành, mức TOEIC ước tính
- 💾 **Sao lưu / khôi phục** tiến độ bằng file `.json` để chuyển sang máy khác

---

## 🚀 Đưa lên GitHub Pages

1. Tạo repo mới trên GitHub, ví dụ `bac-thang-toeic` (để **Public**).
2. Bấm **Add file → Upload files** và kéo vào cả 7 file:
   ```
   index.html
   manifest.json
   sw.js
   icon-180.png
   icon-192.png
   icon-512.png
   README.md
   ```
3. Bấm **Commit changes**.
4. Vào **Settings → Pages**. Ở mục **Source** chọn `Deploy from a branch`, branch `main`, thư mục `/ (root)`, rồi bấm **Save**.
5. Đợi khoảng 1–2 phút. App sẽ có địa chỉ dạng:
   ```
   https://<tên-tài-khoản>.github.io/bac-thang-toeic/
   ```

## 📱 Cài lên iPhone

1. Mở địa chỉ GitHub Pages ở trên bằng **Safari**.
2. Bấm nút **Chia sẻ** (ô vuông có mũi tên đi lên).
3. Chọn **Thêm vào MH chính** (Add to Home Screen), rồi bấm **Thêm**.
4. Mở app từ biểu tượng 🪜 trên màn hình chính.

> Trên Android: mở bằng Chrome → menu ⋮ → **Cài đặt ứng dụng** / **Thêm vào màn hình chính**.

---

## 🗂 Cấu trúc file

| File | Vai trò |
|---|---|
| `index.html` | Toàn bộ app: giao diện, logic và nội dung bài học (nằm chung trong một file) |
| `manifest.json` | Thông tin để cài app lên màn hình chính (tên, icon, màu) |
| `sw.js` | Service worker: lưu app vào máy để dùng khi không có mạng |
| `icon-*.png` | Biểu tượng app |

## ✏️ Thêm hoặc sửa câu hỏi

Nội dung bài học nằm trong `index.html`, ở các khối `window.TOEIC_LEVELS.push({ ... })`. Có thể sửa trực tiếp ngay trên GitHub (bấm biểu tượng ✏️ khi xem file).

**Câu hỏi Part 5** (điền vào chỗ trống):
```js
{ p: "5", q: "The workers ___ in the factory now.", o: ["are", "is", "am", "be"], e: "The workers số nhiều → are." }
```

**Câu nghe Part 2** (`s` là câu được đọc lên):
```js
{ p: "2", s: "Where do you work?", o: ["At a car factory.", "Every day.", "I work hard.", "With my colleagues."], e: "Where → hỏi nơi chốn." }
```

**Hội thoại Part 3**: bắt đầu lời người nói bằng `M:` (giọng nam) hoặc `W:` (giọng nữ):
```js
{ p: "3", s: "M: Is the report ready? W: Yes, I sent it an hour ago.", q: "What does the woman say?", o: ["She sent the report.", "...", "...", "..."], e: "..." }
```

**Câu đọc hiểu Part 7** (`r` là đoạn văn, xuống dòng bằng `\n`):
```js
{ p: "7", r: "NOTICE\nThe cafeteria is closed on weekends.", q: "When is the cafeteria closed?", o: ["On weekends", "On Mondays", "On Fridays", "At noon"], e: "..." }
```

**Từ vựng**: `[từ, phiên âm, từ loại, nghĩa, câu ví dụ]`
```js
["engineer", "/ˌendʒɪˈnɪr/", "n.", "kỹ sư", "He is an electrical engineer."]
```

> ⚠️ **Quy tắc quan trọng:** đáp án đúng **luôn là phần tử đầu tiên** trong mảng `o`. App tự xáo trộn thứ tự A/B/C/D khi hiển thị.

Sau khi sửa `index.html`, nên đổi tên bộ nhớ đệm trong `sw.js`, ví dụ `bacthang-toeic-v1` → `bacthang-toeic-v2`, để máy đã cài app nhận bản mới.

---

## ℹ️ Lưu ý

- **Tiến độ lưu theo từng máy và từng trình duyệt.** Muốn chuyển sang máy khác, vào **Cài đặt → Sao lưu tiến độ**, rồi trên máy mới chọn **Khôi phục tiến độ**.
- Xóa dữ liệu duyệt web của Safari/Chrome sẽ xóa luôn tiến độ. Nên sao lưu định kỳ.
- Giọng đọc phần nghe là giọng tổng hợp của thiết bị, nên chất lượng phụ thuộc vào máy. Trên iPhone có thể tải thêm giọng tiếng Anh trong **Cài đặt → Trợ năng → Nội dung được đọc → Giọng nói → English**.
- Điểm TOEIC hiển thị trong app chỉ là **ước tính để định hướng học**, không thay cho kết quả thi chính thức.
