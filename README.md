# SCH-Forum

Dưới đây là **đặc tả yêu cầu hệ thống (SRS)** cho một **diễn đàn nội bộ BIDV** dùng để trao đổi, thảo luận kỹ thuật, chia sẻ tài liệu, gửi yêu cầu tính năng,… tương tự như ảnh bạn đã gửi từ diễn đàn Cursor.

---

## 📌 **1. Mục tiêu hệ thống**
Xây dựng một nền tảng diễn đàn nội bộ giúp cán bộ nhân viên BIDV có thể:
- Đăng và thảo luận về các chủ đề liên quan đến công nghệ, sản phẩm, nghiệp vụ.
- Trao đổi kiến thức, chia sẻ tài liệu nội bộ.
- Gửi yêu cầu tính năng, báo lỗi phần mềm nội bộ.
- Giao tiếp, đóng góp ý kiến một cách tập trung và dễ tìm kiếm.

---

## 🧱 **2. Tính năng chính**

### 2.1 Quản lý chủ đề (Topics)
- Người dùng có thể tạo chủ đề mới với tiêu đề, mô tả, tag và phân loại.
- Chủ đề có thể thuộc các danh mục như:
  - Thảo luận chung (Discussion)
  - Hướng dẫn sử dụng (How To)
  - Yêu cầu tính năng (Feature Requests)
  - Báo lỗi (Bug Reports)
  - Phản hồi hệ thống (Feedback)
- Các chủ đề hiển thị với các thông tin:
  - Số lượt xem
  - Số lượt phản hồi
  - Thời gian hoạt động gần nhất
  - Người tạo

### 2.2 Quản lý bài viết / phản hồi
- Bài viết hỗ trợ **markdown**, đính kèm ảnh/tập tin.
- Hệ thống thông báo khi có phản hồi mới vào chủ đề mà người dùng theo dõi.
- Cho phép **gắn thẻ (tag)** người dùng khác để thông báo.
- Có thể bình chọn (upvote/downvote) cho câu trả lời hữu ích.

### 2.3 Tìm kiếm và lọc
- Tìm kiếm theo từ khóa, tiêu đề, nội dung, tag, người đăng, hoặc danh mục.
- Bộ lọc theo thời gian, số lượt xem, danh mục, hoạt động gần đây nhất.

### 2.4 Danh mục (Categories)
- Có thể cấu hình danh sách danh mục và phân quyền tạo chủ đề cho từng danh mục.
- Hiển thị rõ danh mục ở sidebar (giống ảnh bạn cung cấp).

### 2.5 Hệ thống người dùng
- Đăng nhập bằng tài khoản nội bộ BIDV (qua SSO hoặc AD).
- Trang cá nhân hiển thị: ảnh đại diện, các bài đã đăng, huy hiệu đạt được.
- Phân quyền: Quản trị viên / Thành viên thông thường.

### 2.6 Huy hiệu & đóng góp (Gamification)
- Cấp huy hiệu theo thành tích:
  - Tham gia lần đầu
  - Có phản hồi được upvote nhiều
  - Chủ đề được quan tâm nhiều
- Hệ thống điểm thưởng theo hoạt động (post, vote, trả lời…)

### 2.7 Gửi yêu cầu tính năng / báo lỗi
- Giao diện nhập yêu cầu tính năng mới, chọn mức độ ưu tiên.
- Cho phép đính kèm ảnh màn hình, mô tả chi tiết lỗi.

---

## 🛡 **3. Tính năng quản trị**
- Quản lý người dùng (khóa, phân quyền, xóa bài…)
- Quản lý danh mục, từ khóa cấm, nội dung vi phạm.
- Thống kê: số bài viết, chủ đề phổ biến, người dùng hoạt động nhiều nhất…

---

## 📱 **4. Yêu cầu UI/UX**
- Giao diện tương tự Discourse / Cursor:
  - Sidebar chứa danh mục
  - Trang chủ là danh sách topic theo thời gian hoạt động
  - Giao diện mobile responsive
- Hỗ trợ chế độ sáng / tối

---

## 🔐 **5. Yêu cầu bảo mật**
- Chỉ cán bộ nội bộ có tài khoản BIDV mới đăng nhập được.
- Tất cả nội dung lưu trữ nội bộ, không public ra ngoài.
- Ghi log hoạt động: tạo, chỉnh sửa, xóa bài viết.

---

## 🔧 **6. Công nghệ gợi ý**
- Backend: Node.js, Django hoặc Rails
- Frontend: React (Next.js), Vue
- Cơ sở dữ liệu: PostgreSQL hoặc MongoDB
- Hosting: Server nội bộ hoặc Kubernetes (nếu có hạ tầng)

---

Nếu bạn cần mình có thể viết thêm: sơ đồ kiến trúc hệ thống, mockup giao diện, hoặc phân tích chi tiết từng tính năng hơn nữa nhé. Bạn muốn tiếp tục ở hướng nào?
