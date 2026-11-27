# Lexi – Website học từ vựng tiếng Anh

Ứng dụng web một trang (HTML/CSS/JavaScript thuần, không cần cài đặt hay build) giúp học từ vựng theo phương pháp lặp lại ngắt quãng.

## Tính năng
- **Tổng quan**: số từ cần ôn hôm nay, biểu đồ 7 ngày, timeline học tập
- **Bộ sưu tập**: 18 chủ đề IELTS Speaking (People & Relationships … Environment & Energy) và các chủ đề khác
- **Từ vựng**: phiên âm, nghĩa, định nghĩa, ví dụ, link Cambridge / Oxford, ngày ôn lại tiếp theo của từng từ
- **5 video ngữ cảnh** cho mỗi từ (YouGlish Mỹ/Anh/Úc, PlayPhrase.me, YouTube)
- **Flashcard** với 4 mức đánh giá (Quên / Khó / Ổn / Dễ)
- **Speaking**: câu hỏi đời thường kiểu IELTS Part 1 kèm câu mẫu, nghe bằng giọng đọc của trình duyệt
- **Bài tập**: trắc nghiệm, điền từ, gõ từ
- **Lịch ôn tập** 14 ngày và các hộp ghi nhớ (mốc 1 – 3 – 7 – 14 – 30 ngày)
- **Nhập từ từ file** `.csv` / `.tsv` / `.txt`

## Định dạng file nhập từ
Mỗi dòng một từ, cột cách nhau bằng `|`, Tab hoặc dấu phẩy (UTF-8):

```
word|loại từ|phiên âm|nghĩa tiếng Việt|định nghĩa|ví dụ|chủ đề|câu hỏi speaking|câu mẫu
punctual|adj|/ˈpʌŋk.tʃu.əl/|đúng giờ|arriving at the expected time|She is always punctual.|Work & Economy|Are you a punctual person?|Yes, I try to arrive early because being late feels disrespectful.
```
Chỉ cột `word` là bắt buộc. Hai cột cuối (câu hỏi speaking, câu mẫu) là tùy chọn; nhiều câu thì ngăn cách bằng `##`. Dòng tiêu đề, dòng bắt đầu bằng `#` và từ trùng sẽ bị bỏ qua.

## Chạy trên máy
Mở `index.html` bằng trình duyệt. Cần có mạng để tải font và mở các link từ điển / video.

## Đưa lên GitHub Pages
1. Tạo repository mới trên GitHub và tải lên `index.html`, `README.md`, `.nojekyll`.
2. Vào **Settings → Pages**, chọn **Deploy from a branch**, nhánh `main`, thư mục `/ (root)`, bấm **Save**.
3. Sau ít phút, trang chạy tại `https://<tên-người-dùng>.github.io/<tên-repo>/`.

## Lưu ý
- Tiến độ học lưu bằng `localStorage` trong trình duyệt, nên mỗi thiết bị / trình duyệt có dữ liệu riêng.
- Định nghĩa trong dữ liệu mẫu được viết lại ngắn gọn; để xem bản chuẩn, dùng link Cambridge / Oxford trong từng từ.
