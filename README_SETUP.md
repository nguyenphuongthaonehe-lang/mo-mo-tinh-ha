# MỘ MỘ TINH HÀ

## Cài đặt database
1. Mở Supabase project.
2. Vào SQL Editor → New query.
3. Mở file supabase/schema.sql trong GitHub, copy toàn bộ nội dung và Run.
4. Trên website, đăng ký tài khoản bằng email.
5. Nếu Supabase yêu cầu xác nhận email, hãy xác nhận trước khi đăng nhập.
6. Để cấp quyền quản trị cho tài khoản vừa tạo, chạy trong SQL Editor:
   update public.profiles set role='admin' where email='EMAIL_DANG_KY_CUA_BAN';
7. Đăng xuất rồi đăng nhập lại. Nút Quản trị sẽ xuất hiện.

## Bật GitHub Pages
Vào Settings → Pages → Build and deployment. Chọn GitHub Actions làm Source. Workflow deploy.yml sẽ tự triển khai sau khi có commit.
Địa chỉ dự kiến: https://nguyenphuongthaonehe-lang.github.io/mo-mo-tinh-ha/

## Tính năng
- Kho truyện, tìm kiếm, lọc thể loại, trang chi tiết, danh sách chương và trình đọc.
- Đăng ký/đăng nhập Supabase Auth.
- Tủ sách yêu thích và đồng bộ tiến độ đọc.
- Quản trị thêm/sửa/xóa truyện và thêm chương.
- Row Level Security bảo vệ dữ liệu và quyền quản trị.

Publishable key là khóa công khai dùng trên trình duyệt. Không đưa service_role key vào website. Ảnh bìa hiện dùng URL công khai; chưa có chức năng upload ảnh, thanh toán hoặc bình luận.
