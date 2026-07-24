# Chính sách Bảo mật — Gia Sư Pro

Cập nhật lần cuối: 24/7/2026

Chính sách này mô tả cách ứng dụng Gia Sư Pro ("chúng tôi", "ứng dụng") thu thập, sử dụng, lưu trữ và bảo vệ dữ liệu cá nhân của người dùng, phù hợp với Luật Bảo vệ dữ liệu cá nhân (Luật số 91/2025/QH15) và Nghị định 356/2025/NĐ-CP của Việt Nam.

---

## 1. Đơn vị chịu trách nhiệm xử lý dữ liệu

- Nhà phát triển: Vũ Doãn Duy
- Email hỗ trợ / liên hệ về dữ liệu: vudoanduy02@gmail.com
- Phạm vi áp dụng: Việt Nam

---

## 2. Đối tượng sử dụng dữ liệu

Gia Sư Pro được thiết kế cho **giáo viên/gia sư** quản lý thông tin học sinh, bao gồm cả thông tin liên hệ của phụ huynh. Người trực tiếp nhập dữ liệu học sinh vào ứng dụng (thường là giáo viên/gia sư) có trách nhiệm đảm bảo đã thông báo và có sự đồng ý của phụ huynh/người giám hộ trước khi lưu trữ thông tin liên quan đến trẻ em trên ứng dụng.

---

## 3. Dữ liệu chúng tôi thu thập

### 3.1. Đăng nhập tài khoản — Firebase Authentication (Google Sign-In)

| Mục | Nội dung |
|---|---|
| Dữ liệu thu thập | Email, tên hiển thị, ảnh đại diện Google, mã định danh người dùng (UID) |
| Mục đích | Xác thực và cho phép đăng nhập lại trên nhiều thiết bị |
| Nơi lưu trữ | Hạ tầng Firebase Authentication (Google Cloud) |
| Ai truy cập | Nhà phát triển (qua Firebase Console, quyền hạn chế); Google với vai trò bên xử lý dữ liệu thay mặt chúng tôi |

### 3.2. Dữ liệu học sinh & phụ huynh (sao lưu) — Cloud Firestore

| Mục | Nội dung |
|---|---|
| Dữ liệu thu thập | Họ tên học sinh, lớp/khóa học, ghi chú học tập, số điện thoại phụ huynh, học phí, lịch học
| Mục đích | Sao lưu dữ liệu để khôi phục khi người dùng đổi thiết bị hoặc cài lại ứng dụng |
| Nơi lưu trữ | Cloud Firestore (Google Cloud), khu vực máy chủ:  asia-southeast1
| Ai truy cập | Người dùng chỉ truy cập được dữ liệu do chính mình tạo (thông qua Firestore Security Rules gắn với tài khoản đăng nhập); nhà phát triển có thể truy cập cho mục đích vận hành, hỗ trợ kỹ thuật hoặc xử lý sự cố |
| Chia sẻ với bên thứ ba | Không chia sẻ cho bên thứ ba ngoài Google/Firebase (đơn vị cung cấp hạ tầng lưu trữ) |
| Thời gian lưu trữ | lưu đến khi người dùng chủ động xóa hoặc yêu cầu xóa tài khoản

**Lưu ý về dữ liệu trẻ em:** Số điện thoại phụ huynh và thông tin học sinh là dữ liệu cá nhân của trẻ em/nhóm dữ liệu nhạy cảm liên quan đến bên thứ ba. Việc nhập các dữ liệu này vào ứng dụng cần có sự đồng ý của phụ huynh/người giám hộ. Chúng tôi không sử dụng dữ liệu này cho mục đích quảng cáo, phân tích hành vi hay chia sẻ cho bất kỳ bên thứ ba nào ngoài mục đích sao lưu nêu trên.

### 3.3. Dữ liệu sử dụng ứng dụng — Firebase Analytics

| Mục | Nội dung |
|---|---|
| Dữ liệu thu thập | Số liệu sử dụng ứng dụng (màn hình đã xem, thao tác trong app), thông tin thiết bị (dòng máy, phiên bản hệ điều hành), mã định danh ẩn danh của Analytics |
| Mục đích | Đo lường hiệu năng, cải thiện trải nghiệm sử dụng |
| Nơi lưu trữ | Hạ tầng Google Analytics/Firebase |
| Ai truy cập | Nhà phát triển (chỉ ở dạng số liệu tổng hợp, không định danh cá nhân); Google |
| Cam kết | Chúng tôi không gửi tên học sinh, số điện thoại phụ huynh hoặc bất kỳ thông tin định danh cá nhân nào vào hệ thống Analytics |

### 3.4. Báo cáo lỗi — Firebase Crashlytics

| Mục | Nội dung |
|---|---|
| Dữ liệu thu thập | Nhật ký lỗi (crash log), stack trace, thông tin thiết bị và phiên bản ứng dụng |
| Mục đích | Phát hiện, chẩn đoán và khắc phục lỗi kỹ thuật |
| Nơi lưu trữ | Hạ tầng Firebase/Google Cloud |
| Ai truy cập | Nhà phát triển |
| Cam kết | Báo cáo lỗi không chứa thông tin định danh cá nhân của học sinh hoặc phụ huynh |

---

## 4. Cơ sở pháp lý xử lý dữ liệu

Chúng tôi xử lý dữ liệu cá nhân dựa trên:
- **Sự đồng ý** của người dùng khi đăng ký tài khoản và nhập dữ liệu học sinh/phụ huynh;
- **Nhu cầu thực hiện chức năng cốt lõi** của ứng dụng (sao lưu, khôi phục dữ liệu).

---

## 5. Quyền của người dùng

Theo Luật Bảo vệ dữ liệu cá nhân 2025, bạn có các quyền sau đối với dữ liệu cá nhân của mình:

- **Quyền được biết** về việc xử lý dữ liệu cá nhân của mình;
- **Quyền đồng ý / rút lại sự đồng ý** đối với việc xử lý dữ liệu;
- **Quyền truy cập** để xem dữ liệu đang được lưu trữ;
- **Quyền chỉnh sửa** dữ liệu không chính xác;
- **Quyền xóa** dữ liệu cá nhân;
- **Quyền khiếu nại, tố cáo, khởi kiện** khi quyền lợi bị xâm phạm.

Để thực hiện các quyền trên, vui lòng liên hệ: **vudoanduy02@gmail.com**. Chúng tôi sẽ phản hồi trong vòng 15 ngày làm việc.

---

## 6. Bảo mật dữ liệu

- Dữ liệu được truyền tải qua kết nối mã hóa (HTTPS/TLS).
- Dữ liệu lưu trữ trên Firestore được mã hóa tại chỗ (encryption at rest) theo tiêu chuẩn mặc định của Google Cloud.
- Quyền truy cập vào dữ liệu được giới hạn thông qua Firestore Security Rules và quyền quản trị Firebase.

## 7. Thông báo khi xảy ra sự cố lộ, mất dữ liệu

Trong trường hợp xảy ra sự cố ảnh hưởng đến dữ liệu cá nhân của người dùng, chúng tôi sẽ thông báo cho người dùng bị ảnh hưởng và, nếu cần, cho cơ quan có thẩm quyền, theo quy định của pháp luật hiện hành.

## 8. Thay đổi chính sách

Chính sách này có thể được cập nhật theo thời gian. Mọi thay đổi quan trọng sẽ được thông báo trong ứng dụng hoặc qua email đăng ký.

## 9. Liên hệ

Nếu có bất kỳ câu hỏi nào về chính sách bảo mật này hoặc về dữ liệu cá nhân của bạn, vui lòng liên hệ:

**Email:** vudoanduy02@gmail.com
