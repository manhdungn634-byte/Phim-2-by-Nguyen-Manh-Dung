# Web Phim 2 by Nguyen Manh Dung

Web xem thông tin phim (poster, điểm đánh giá, thể loại, trailer) dùng dữ liệu hợp pháp từ TMDB.
Chỉ có 1 file `index.html`, không cần cài đặt gì, đưa lên GitHub Pages là chạy.

## Tính năng
Đề xuất, Phim bộ, Phim lẻ, Hoạt hình, Thể loại, Tìm kiếm, Lịch chiếu, Yêu thích, avatar đăng nhập (bản mẫu), nút API, xem trailer YouTube, giao diện sáng/tối.

## Bước 1: Lấy API key TMDB (miễn phí)
1. Vào https://www.themoviedb.org và đăng ký tài khoản, xác nhận email.
2. Vào Settings → API → Create → chọn Developer, điền thông tin (mục đích: học tập/cá nhân).
3. Copy **API Key (v3 auth)**, là chuỗi 32 ký tự.

## Bước 2: Tạo repository trên GitHub
1. Đăng nhập https://github.com (chưa có thì đăng ký).
2. Bấm dấu **+** góc trên phải → **New repository**.
3. Đặt tên, ví dụ `web-phim-2`, chọn **Public**, bấm **Create repository**.

## Bước 3: Tải file lên
1. Trong repo vừa tạo, bấm **uploading an existing file** (hoặc Add file → Upload files).
2. Kéo thả `index.html` và `README.md` vào.
3. Bấm **Commit changes**.

## Bước 4: Bật GitHub Pages
1. Vào **Settings** → **Pages** (menu bên trái).
2. Mục Source chọn **Deploy from a branch**.
3. Branch chọn **main**, thư mục **/ (root)**, bấm **Save**.
4. Đợi 1–2 phút, trang hiện link dạng `https://TEN-GITHUB.github.io/web-phim-2/`.

## Bước 5: Nhập API key
Cách 1 (dễ nhất): mở web, bấm nút **API**, dán key, bấm **Lưu và tải phim**. Key chỉ lưu trên trình duyệt của người đang dùng.

Cách 2: sửa `index.html` trên GitHub (biểu tượng bút chì), tìm dòng
`var API_KEY = "";` và điền key vào giữa hai dấu ngoặc kép, rồi Commit. Mọi người vào web đều thấy phim ngay.
Lưu ý: key đặt trong code sẽ hiển thị công khai. Với TMDB, key miễn phí nên chấp nhận được, nhưng đừng dùng key trả phí.

## Dùng tên miền riêng (không bắt buộc)
Settings → Pages → Custom domain, nhập tên miền và trỏ DNS CNAME về `TEN-GITHUB.github.io`.

## Lỗi thường gặp
- **Trang trắng/404**: chờ vài phút, kiểm tra file tên đúng là `index.html` (chữ thường).
- **Không hiện phim**: key sai hoặc chưa nhập, bấm nút API để kiểm tra.
- **Không có trailer**: phim đó chưa có video trên TMDB.

## Lưu ý pháp lý
Web chỉ hiển thị thông tin và trailer. Hãy dẫn người dùng tới nền tảng xem phim chính thức, không đăng phim vi phạm bản quyền.
Theo điều khoản TMDB, cần giữ dòng ghi nguồn ở cuối trang.
