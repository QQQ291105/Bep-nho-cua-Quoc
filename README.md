# Bếp nhỏ của Sơn – bản Android PWA

## Có gì trong bản này?
- Ghi khoản chi theo ngày, số tiền, danh mục và ghi chú.
- Sửa/xóa giao dịch.
- Tổng quan ngân sách tuần, chi tiêu tháng, trung bình/ngày.
- Thống kê theo danh mục và ngày.
- Danh sách đi chợ có giá dự toán, số lượng và trạng thái đã mua.
- Đổi ngân sách tuần.
- Sao lưu/khôi phục JSON và xuất CSV.
- Lưu dữ liệu cục bộ trên trình duyệt bằng localStorage.
- Có service worker để dùng ngoại tuyến sau khi mở ứng dụng lần đầu.

## Cách cài lên Android
Ứng dụng PWA cần được đưa lên một website có HTTPS (không thể cài PWA hoàn chỉnh chỉ bằng cách mở file HTML).

Cách đơn giản:
1. Tạo tài khoản GitHub nếu chưa có.
2. Tạo repository mới, ví dụ `bep-nho-cua-son`.
3. Giải nén ZIP này trên máy tính.
4. Tải toàn bộ các file `index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg` lên thư mục gốc repository.
5. Trong GitHub, vào Settings → Pages.
6. Chọn Deploy from a branch, chọn branch `main`, folder `/ (root)`, rồi Save.
7. Chờ GitHub Pages cấp địa chỉ HTTPS. Mở địa chỉ đó trên Chrome Android.
8. Chọn menu ⋮ → Install app (Cài đặt ứng dụng) hoặc Add to Home screen (Thêm vào màn hình chính).

Tên mục có thể khác đôi chút tùy phiên bản Chrome/Android.

## Cách sử dụng
- Vào Tổng quan để ghi khoản chi nhanh.
- Vào Sổ chi tiêu để lọc, sửa hoặc xóa giao dịch.
- Vào Thống kê để xem tổng chi theo tuần/tháng/danh mục.
- Vào Đi chợ để sửa giá dự toán và đánh dấu đã mua.
- Vào Cài đặt & sao lưu để xuất JSON hoặc CSV.

## Lưu ý quan trọng về dữ liệu
- Dữ liệu hiện được lưu trên trình duyệt của thiết bị, không tự đồng bộ giữa điện thoại và máy tính.
- Không xóa dữ liệu trang web/trình duyệt nếu chưa sao lưu.
- Nên xuất file JSON mỗi tuần và lưu ở nơi an toàn (Google Drive hoặc máy tính).
- Khi đổi điện thoại, cài ứng dụng rồi dùng chức năng Khôi phục dữ liệu.
- Giá thực phẩm là số dự toán ban đầu; hãy sửa theo hóa đơn thực tế.
- Danh sách đi chợ và giao dịch chi tiêu độc lập: đánh dấu đã mua không tự tạo giao dịch, tránh ghi trùng.

## Giới hạn bản 1.0
- Chưa có đăng nhập/tài khoản và đồng bộ đám mây.
- Chưa tự động lấy giá từ chợ/siêu thị.
- Chưa có thông báo nhắc ghi chi tiêu.
- Đây là PWA cài từ website, chưa phải APK đăng trên Google Play.
