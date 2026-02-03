# 🏪 HỆ THỐNG QUẢN LÝ MÁY BÁN HÀNG TỰ ĐỘNG

## Giải pháp SaaS toàn diện cho doanh nghiệp Vending Machine

---

## 📋 TỔNG QUAN

**CV-VMMS (Chí Vĩ Vending Machine Management System)** là nền tảng quản lý máy bán hàng tự động hiện đại, được thiết kế để giúp doanh nghiệp:

✅ **Giám sát máy 24/7** - Biết ngay khi máy gặp sự cố, hết hàng, mất kết nối
✅ **Thu tiền tự động** - Hỗ trợ QR code, tiền mặt, ví điện tử
✅ **Báo cáo thông minh** - Biết doanh thu, tồn kho ngay trên điện thoại
✅ **Giữ chân khách hàng** - Loyalty, tích điểm, khuyến mãi tự động

> 💡 **"Quản lý 100 máy như quản lý 1 máy - Mọi thứ trong tầm tay"**

---

# 📱 DANH SÁCH CHỨC NĂNG CHI TIẾT

---

## 1️⃣ GIÁM SÁT MÁY REAL-TIME

### 📍 Theo dõi trạng thái máy

| Chức năng | Mô tả chi tiết |
|-----------|----------------|
| **Trạng thái Online/Offline** | Biết máy đang hoạt động hay mất kết nối, cập nhật mỗi 5 phút |
| **Tín hiệu kết nối** | Xem cường độ tín hiệu WiFi/4G của máy (strong/weak/poor) |
| **Nhiệt độ máy** | Theo dõi nhiệt độ bên trong máy, cảnh báo khi quá nóng |
| **Health Score** | Điểm sức khỏe tổng hợp của máy (0-100), giúp ưu tiên bảo trì |
| **Thời gian online** | Thống kê uptime, downtime theo ngày/tuần/tháng |
| **Vị trí máy trên bản đồ** | Xem tất cả máy trên map, lọc theo trạng thái |

### 🔔 Cảnh báo tự động

| Loại cảnh báo | Khi nào kích hoạt |
|---------------|-------------------|
| **Máy offline** | Mất kết nối quá 10 phút |
| **Hết hàng** | Slot sản phẩm còn dưới 20% |
| **Lỗi thanh toán** | Giao dịch thất bại liên tiếp |
| **Lỗi cơ khí** | Kẹt hàng, động cơ lỗi |
| **Nhiệt độ bất thường** | Quá nóng hoặc quá lạnh |
| **Doanh thu bất thường** | Giảm đột ngột so với ngày thường |

### 📲 Nhận thông báo qua

- ✅ Push notification trên điện thoại (PWA)
- ✅ Email tự động
- ✅ Dashboard web real-time
- ✅ Báo cáo tổng hợp cuối ngày

---

## 2️⃣ THANH TOÁN ĐA DẠNG

### 💳 Các phương thức thanh toán hỗ trợ

| Phương thức | Đối tác | Phí giao dịch | Thời gian xử lý |
|-------------|---------|---------------|-----------------|
| 🏦 **VietQR** | BaoKim | Thấp | 3-5 giây |
| 💳 **Thẻ ngân hàng** | VNPay | Chuẩn | 5-10 giây |
| 📱 **Ví MoMo** | MoMo | Chuẩn | 3-5 giây |
| 💰 **OnePay** | OnePay | Chuẩn | 5-10 giây |
| 💵 **Tiền mặt** | Tích hợp sẵn | Không phí | Ngay lập tức |

### ⚡ Tính năng thanh toán

| Chức năng | Mô tả |
|-----------|-------|
| **Tạo QR trong 1 giây** | Khách quét QR, tiền về ngay |
| **Theo dõi giao dịch real-time** | Biết ngay khi khách thanh toán xong |
| **Hoàn tiền tự động** | Nếu máy lỗi, hoàn tiền về ví/tài khoản khách |
| **Đối soát tự động** | So khớp doanh thu hệ thống với ngân hàng |
| **Chống gian lận** | Xác thực chữ ký webhook từ cổng thanh toán |
| **Lịch sử giao dịch** | Tra cứu mọi giao dịch theo ngày, máy, khách hàng |
| **Xuất báo cáo ngân hàng** | Excel/PDF để đối soát với kế toán |

### 🔧 Cấu hình thanh toán

- ✅ Cấu hình cổng thanh toán riêng cho từng máy
- ✅ Cấu hình mặc định theo tổ chức
- ✅ Bật/tắt phương thức thanh toán theo nhu cầu
- ✅ Test kết nối trước khi đưa vào hoạt động

---

## 3️⃣ QUẢN LÝ SẢN PHẨM & TỒN KHO

### 📦 Quản lý danh mục sản phẩm

| Chức năng | Mô tả |
|-----------|-------|
| **Danh mục phân cấp** | Đồ uống → Nước ngọt → Coca-Cola |
| **Thông tin sản phẩm** | Tên, giá, mô tả, hình ảnh, barcode |
| **Giá theo tier** | Giá VIP, giá thường, giá khuyến mãi |
| **Mã vạch (Barcode)** | Quét barcode để nhập hàng nhanh |
| **Thuế VAT** | Cấu hình % VAT cho từng sản phẩm |
| **Sản phẩm đang hoạt động** | Bật/tắt sản phẩm không cần xóa |

### 📊 Quản lý tồn kho

| Chức năng | Mô tả |
|-----------|-------|
| **Tồn kho theo slot** | Biết từng slot máy còn bao nhiêu sản phẩm |
| **Cảnh báo hết hàng** | Thông báo khi slot còn dưới ngưỡng |
| **Nhập hàng nhanh** | Quét barcode + nhập số lượng |
| **Nhập hàng loạt** | Chọn nhiều slot, nhập cùng lúc |
| **Lịch sử nhập/xuất** | Biết ai nhập, khi nào, bao nhiêu |
| **Điều chỉnh tồn** | Ghi lý do khi điều chỉnh (hư hỏng, mất...) |
| **Báo cáo tồn kho** | Tổng hợp tồn theo máy, nhóm, sản phẩm |

### 🎰 Quản lý slot máy

| Chức năng | Mô tả |
|-----------|-------|
| **Tối đa 120 slot/máy** | Hỗ trợ máy lớn nhất thị trường |
| **Gán sản phẩm vào slot** | Kéo thả hoặc chọn từ danh sách |
| **Gán sản phẩm hàng loạt** | Chọn nhiều slot, gán cùng sản phẩm |
| **Đổi giá theo slot** | Giá khác nhau cho cùng sản phẩm ở các slot |
| **Xem tình trạng slot** | Xanh = đầy, vàng = sắp hết, đỏ = hết |
| **Đồng bộ với máy** | Cập nhật cấu hình slot xuống máy |

---

## 4️⃣ BÁO CÁO & PHÂN TÍCH

### 📈 Dashboard tổng quan

| Chỉ số | Mô tả |
|--------|-------|
| **Tổng doanh thu** | Hôm nay, tuần này, tháng này, năm nay |
| **Số giao dịch** | Tổng số giao dịch thành công/thất bại |
| **Số máy online** | Tỷ lệ máy đang hoạt động |
| **Top sản phẩm** | 10 sản phẩm bán chạy nhất |
| **Top máy** | 10 máy doanh thu cao nhất |
| **Tỷ lệ thanh toán** | % theo phương thức (QR/cash/ví) |
| **Xu hướng doanh thu** | Biểu đồ theo giờ/ngày/tuần/tháng |

### 📊 Báo cáo chi tiết

| Loại báo cáo | Nội dung |
|--------------|----------|
| **Doanh thu theo máy** | Doanh thu từng máy theo thời gian |
| **Doanh thu theo sản phẩm** | Sản phẩm nào bán chạy, lợi nhuận |
| **Doanh thu theo nhóm máy** | So sánh hiệu quả các khu vực |
| **Báo cáo tồn kho** | Tồn đầu kỳ, nhập, xuất, tồn cuối kỳ |
| **Báo cáo giao dịch** | Chi tiết từng giao dịch, lọc theo nhiều tiêu chí |
| **Báo cáo hoạt động máy** | Uptime, downtime, lỗi của máy |
| **Báo cáo nhân viên** | Ai nhập hàng, ai thao tác gì |

### 📤 Xuất báo cáo

- ✅ Xuất Excel (.xlsx) để xử lý tiếp
- ✅ Xuất PDF để in/gửi email
- ✅ Lọc theo ngày, máy, sản phẩm, nhân viên
- ✅ Lên lịch gửi báo cáo tự động qua email

---

## 5️⃣ ĐIỀU KHIỂN MÁY TỪ XA

### 🔧 Các lệnh điều khiển

| Lệnh | Chức năng | Ứng dụng |
|------|-----------|----------|
| 🔄 **Khởi động lại (Reboot)** | Reset máy không cần ra hiện trường | Máy bị đơ, lỗi phần mềm |
| 📥 **Cập nhật firmware (OTA)** | Nâng cấp phần mềm máy từ xa | Thêm tính năng, sửa lỗi |
| 💰 **Nạp tiền khuyến mãi (Topup)** | Cộng credit cho khách | Chương trình khuyến mãi, bồi thường |
| ⚙️ **Lấy cấu hình (Get Config)** | Xem cài đặt hiện tại của máy | Kiểm tra, debug |

### 🛡️ Bảo mật điều khiển

| Tính năng | Mô tả |
|-----------|-------|
| **Xác nhận 2 bước** | Lệnh quan trọng (Reboot, OTA) cần xác nhận |
| **Giới hạn tần suất** | Không gửi quá nhiều lệnh liên tục |
| **Chống lệnh trùng** | Tự động phát hiện và chặn lệnh duplicate |
| **Phân quyền** | Chỉ manager/owner mới được điều khiển |
| **Ghi log đầy đủ** | Biết ai gửi lệnh gì, lúc nào, kết quả thế nào |

---

## 6️⃣ QUẢN LÝ NGƯỜI DÙNG & PHÂN QUYỀN

### 👥 Hệ thống phân quyền 5 cấp

```
👑 Chủ sở hữu (Organization Owner)
   ├── Toàn quyền hệ thống
   ├── Quản lý tài khoản, phân quyền
   ├── Xem tất cả báo cáo
   └── Cấu hình thanh toán, hóa đơn

👔 Quản lý (Manager)
   ├── Quản lý máy, sản phẩm
   ├── Xem báo cáo doanh thu
   ├── Quản lý nhân viên cấp dưới
   └── Điều khiển máy từ xa

👷 Vận hành (Operator)
   ├── Xem trạng thái máy
   ├── Nhập hàng, điều chỉnh tồn kho
   ├── Xem lịch sử giao dịch
   └── Không thể chỉnh cấu hình

👤 Nhân viên (Staff)
   ├── Chỉ xem thông tin
   ├── Không thể thay đổi gì
   └── Phù hợp cho nhân viên mới

👁️ Khách (Guest)
   └── Quyền tối thiểu, dùng cho API
```

### 🏢 Quản lý theo nhóm máy

| Chức năng | Mô tả |
|-----------|-------|
| **Tạo nhóm máy** | VD: Khu vực HCM, Hà Nội, miền Trung |
| **Gán người dùng vào nhóm** | Nhân viên A quản lý nhóm HCM |
| **Phân quyền theo nhóm** | Quyền khác nhau ở mỗi nhóm |
| **Dữ liệu tách biệt** | Nhân viên chỉ thấy máy của nhóm mình |

### 📝 Theo dõi hoạt động nhân viên

| Thông tin được ghi lại | Mô tả |
|------------------------|-------|
| **Ai đăng nhập** | Thời gian, IP, thiết bị |
| **Ai thao tác gì** | Tạo/sửa/xóa máy, sản phẩm... |
| **Ai nhập hàng** | Slot nào, số lượng, thời gian |
| **Ai gửi lệnh điều khiển** | Reboot, OTA, Topup... |
| **Ai chỉnh phân quyền** | Thêm/bớt quyền cho ai |

---

## 7️⃣ HỆ THỐNG KHÁCH HÀNG & LOYALTY ⭐

> 💡 **Đây là điểm mạnh vượt trội so với các đối thủ trên thị trường!**

### 📱 Cổng khách hàng (Customer Portal)

| Chức năng | Mô tả |
|-----------|-------|
| **Đăng ký tài khoản** | Bằng email, số điện thoại |
| **Xem lịch sử mua hàng** | Tất cả giao dịch theo thời gian |
| **Xem chi tiết session** | Mua gì, bao nhiêu tiền, thanh toán thế nào |
| **Quản lý ví điện tử** | Nạp tiền, xem số dư, lịch sử giao dịch |
| **Đổi điểm thưởng** | Đổi lấy voucher, sản phẩm miễn phí |
| **Claim hóa đơn** | Quét QR lấy hóa đơn VAT |

### 🎁 Chương trình Loyalty 4 cấp độ

| Hạng | Điểm cần | Ưu đãi |
|------|----------|--------|
| 🥉 **Bronze** | 0+ điểm | Tích điểm cơ bản (1 điểm = 1.000đ) |
| 🥈 **Silver** | 500+ điểm | Tích điểm x1.1 (+10%), ưu đãi riêng |
| 🥇 **Gold** | 2,000+ điểm | Tích điểm x1.25 (+25%), free shipping |
| 💎 **Platinum** | 5,000+ điểm | Tích điểm x1.5 (+50%), VIP support |

### ⚡ Tính năng Loyalty nổi bật

| Chức năng | Mô tả |
|-----------|-------|
| **Tích điểm tức thì** | Điểm được cộng ngay khi thanh toán xong |
| **Tự động nâng hạng** | Đủ điểm = tự động lên tier cao hơn |
| **Điểm có hạn sử dụng** | Mặc định 365 ngày, có thể cấu hình |
| **Đổi điểm linh hoạt** | Đổi voucher, sản phẩm miễn phí, hoặc credit |
| **Lịch sử điểm chi tiết** | Biết kiếm điểm từ đâu, dùng điểm ở đâu |
| **Thông báo nhắc nhở** | Nhắc điểm sắp hết hạn |

### 🎟️ Hệ thống Promo Code nâng cao

| Chức năng | Mô tả |
|-----------|-------|
| **Tạo chiến dịch** | Đặt tên, thời gian, ngân sách |
| **Sinh mã hàng loạt** | Tạo 100, 1000 mã cùng lúc |
| **Giới hạn sử dụng** | Tối đa X lần/mã, X lần/khách |
| **Giới hạn thời gian** | Từ ngày X đến ngày Y |
| **Giới hạn theo máy** | Chỉ dùng được ở máy/nhóm máy cụ thể |
| **Giới hạn theo sản phẩm** | Chỉ áp dụng cho sản phẩm cụ thể |
| **Giới hạn theo khách hàng** | Chỉ cho nhóm khách VIP, Gold... |
| **Auto-trigger** | Tự động kích hoạt khi mua đủ X đồng |
| **Chống gian lận** | Phát hiện dùng lại, dùng quá nhanh |
| **Báo cáo hiệu quả** | Bao nhiêu mã phát, bao nhiêu mã dùng, doanh thu tăng bao nhiêu |

### 💰 Hệ thống ví điện tử

| Chức năng | Mô tả |
|-----------|-------|
| **Ví credit** | Nạp tiền trước, mua hàng không cần thanh toán lại |
| **Ví voucher** | Lưu voucher được tặng, mã khuyến mãi |
| **Nạp tiền** | QR, chuyển khoản, thẻ |
| **Chuyển tiền** | Tặng credit cho bạn bè |
| **Rút tiền** | Rút về tài khoản ngân hàng (nếu cho phép) |
| **Lịch sử giao dịch** | Chi tiết từng lần nạp/rút/dùng |

### 🆚 So sánh với đối thủ trên thị trường

| Tính năng | VMMS | Vendon (Latvia) | Dropfoods (VN) | Các hãng khác |
|-----------|------|-----------------|----------------|---------------|
| Cổng khách hàng Web | ✅ Có | ❌ App only | ❌ App only | ❌ Không |
| Đăng nhập Google/Facebook | ✅ Có | ❌ Không | ❌ Không | ❌ Không |
| Hệ thống tier 4 cấp | ✅ Có | ⚠️ Groups only | ❌ Flat | ❌ Không |
| Tự động nâng hạng | ✅ Có | ❌ Thủ công | ❌ Không | ❌ Không |
| Điểm có hạn sử dụng | ✅ Theo dõi được | ⚠️ Thủ công | ❌ Không | ❌ Không |
| Chiến dịch khuyến mãi | ✅ Đầy đủ + analytics | ⚠️ Giảm giá cơ bản | ⚠️ Hạn chế | ❌ Không |
| Chống gian lận promo | ✅ AI + rules | ❌ Không | ❌ Không | ❌ Không |
| Phân nhóm khách hàng | ✅ Tags + filters | ⚠️ Groups | ❌ Không | ❌ Không |
| Claim session lấy hóa đơn | ✅ QR + web | ❌ Không | ❌ Không | ❌ Không |
| Ví tiền + voucher | ✅ Cả 2 | ⚠️ Credit only | ⚠️ DFCoin | ❌ Không |
| Hỗ trợ doanh nghiệp B2B | ✅ Group pricing | ✅ Có | ❌ Không | ❌ Không |
| API mở để tích hợp | ✅ REST API đầy đủ | ⚠️ Hạn chế | ❌ Đóng | ❌ Không |

---

## 8️⃣ HÓA ĐƠN ĐIỆN TỬ TỰ ĐỘNG

### 🧾 Nhà cung cấp hỗ trợ

| Nhà cung cấp | Đặc điểm |
|--------------|----------|
| **HiLo** | Phổ biến, ổn định |

### ⚡ Tính năng hóa đơn

| Chức năng | Mô tả |
|-----------|-------|
| **Xuất hóa đơn tự động** | Giao dịch xong → hóa đơn tạo ngay |
| **Gom nhiều giao dịch** | 1 khách mua nhiều lần → 1 hóa đơn cuối ngày |
| **Khách claim hóa đơn** | Quét QR để lấy hóa đơn VAT |
| **Cấu hình mặc định** | Toàn tổ chức dùng chung 1 nhà cung cấp |
| **Lịch sử hóa đơn** | Tra cứu, xuất lại hóa đơn |
| **Báo cáo thuế** | Tổng hợp hóa đơn theo tháng/quý |

---

## 9️⃣ QUẢN LÝ NHÓM MÁY

### 📍 Tính năng nhóm máy

| Chức năng | Mô tả |
|-----------|-------|
| **Tạo nhóm** | Theo khu vực, theo loại, theo khách hàng |
| **Thông tin nhóm** | Tên, mô tả, địa chỉ, liên hệ |
| **Vị trí trên bản đồ** | Xem nhóm máy trên map |
| **Thêm/bớt máy** | Kéo thả hoặc chọn từ danh sách |
| **Thống kê theo nhóm** | Doanh thu, tồn kho, hoạt động |
| **So sánh nhóm** | Nhóm nào hiệu quả hơn |
| **Phân quyền theo nhóm** | Nhân viên A chỉ thấy nhóm A |

---

## 🔟 QUẢN TRỊ HỆ THỐNG (SYSADMIN)

### ⚙️ Dành cho quản trị viên cấp cao

| Chức năng | Mô tả |
|-----------|-------|
| **Quản lý tổ chức** | Xem tất cả org, thống kê, trạng thái |
| **Chuyển máy giữa org** | Transfer device không mất dữ liệu |
| **Vô hiệu hóa hàng loạt** | Tắt nhiều máy cùng lúc |
| **Cấu hình thanh toán** | Quản lý cổng thanh toán toàn hệ thống |
| **Test kết nối** | Kiểm tra cổng thanh toán,... |
| **Xem log hệ thống** | Debug, troubleshoot |
| **Audit trail đầy đủ** | Mọi thao tác admin được ghi lại |

---

## 1️⃣1️⃣ TÍNH NĂNG ĐỘC QUYỀN - CHỈ CÓ Ở VMMS 🚀

> 💡 **Các tính năng "WOW" mà không đối thủ nào có!**

---

### 🔍 SESSION TIMELINE - ĐIỀU TRA GIAO DỊCH

Xem chi tiết từng bước của 1 giao dịch để giải quyết tranh chấp:

```
⏱️ 14:30:01 - Khách nhét 50.000đ (Số dư: 50.000đ)
⏱️ 14:30:15 - Khách chọn sản phẩm A (Giá: 15.000đ)
⏱️ 14:30:18 - Máy xuất hàng thành công
⏱️ 14:30:19 - Trừ tiền: -15.000đ (Số dư: 35.000đ)
⏱️ 14:30:45 - Khách chọn sản phẩm B (Giá: 20.000đ)
⏱️ 14:30:48 - MÁY LỖI - Không xuất được hàng
⏱️ 14:30:49 - Hoàn tiền tự động: +20.000đ (Số dư: 35.000đ)
⏱️ 14:31:00 - Khách lấy tiền thừa: -35.000đ (Số dư: 0đ)
✅ Session kết thúc - Cân bằng: 0đ
```

| Tính năng | Mô tả |
|-----------|-------|
| **Timeline trực quan** | Xem từng sự kiện theo thời gian |
| **Balance tracking** | Biết số dư tại mỗi thời điểm |
| **Color-coded events** | Xanh = OK, Đỏ = Lỗi, Vàng = Cảnh báo |
| **Export PDF** | Xuất ra để gửi cho khách hàng |
| **Lọc theo loại** | Chỉ xem tiền vào, tiền ra, hoặc lỗi |

**Lợi ích:**
- 🔍 **Giải quyết tranh chấp nhanh** - Bằng chứng rõ ràng
- 📋 **Tuân thủ audit** - Ghi lại mọi thứ
- 🛡️ **Phát hiện gian lận** - Nhìn thấy pattern bất thường

---

### 🏪 TÍCH HỢP HỆ THỐNG POS (IPOS)

Đồng bộ 2 chiều với hệ thống POS cửa hàng tiện lợi:

| Hướng | Chức năng |
|-------|-----------|
| **POS → VMMS** | Đồng bộ danh mục sản phẩm, giá, tồn kho |
| **VMMS → POS** | Gửi giao dịch bán hàng về POS |

**Tính năng:**
- 📦 **Fetch sản phẩm từ POS** - Không cần nhập lại
- 💰 **Post order về POS** - Doanh thu tính chung
- 🔄 **Đồng bộ tồn kho** - Chính xác real-time
- 🏢 **Hỗ trợ multi-location** - Nhiều cửa hàng
- 🔁 **Retry tự động** - Nếu POS offline, tự retry sau

**Use case:**
- Chuỗi cửa hàng tiện lợi muốn thêm máy bán tự động
- Siêu thị mini muốn bán hàng 24/7
- F&B muốn mở rộng mà không cần nhân viên

---

### 🎫 HỆ THỐNG TICKET HỖ TRỢ

Quản lý yêu cầu hỗ trợ từ khách hàng:

| Tính năng | Mô tả |
|-----------|-------|
| **Mã ticket tự động** | TKT-20260202-0001 |
| **Phân loại** | Kỹ thuật, Thanh toán, Sản phẩm, Khác |
| **Ưu tiên** | Thấp, Trung bình, Cao, Khẩn cấp |
| **Trạng thái** | Mới → Đang xử lý → Chờ khách → Đã giải quyết |
| **Gắn file đính kèm** | Ảnh, video, log |
| **Giao cho nhân viên** | Assign cho đúng người |
| **SLA tracking** | Cảnh báo nếu xử lý chậm |
| **Lịch sử trao đổi** | Comment qua lại như chat |

**Lợi ích:**
- 📞 **Không bỏ sót request** - Mọi yêu cầu được track
- ⏱️ **Đảm bảo SLA** - Biết ngay ai chậm trễ
- 📊 **Báo cáo hiệu suất** - Support tốt hay chưa

---

### 📊 GIÁM SÁT HẠ TẦNG HỆ THỐNG

Dashboard theo dõi sức khỏe server:

| Metric | Theo dõi |
|--------|----------|
| **CPU** | % sử dụng từng core |
| **RAM** | Memory usage, swap |
| **Disk** | Dung lượng, I/O |
| **Database** | Connection pool, query time, replication lag |
| **MQTT Broker** | Connections, messages/sec |
| **Web Server** | Request/sec, error rate |

**Cảnh báo tự động khi:**
- CPU > 80% trong 5 phút
- RAM > 90%
- Disk > 85%
- Database replication lag > 10 giây
- Error rate > 1%

---

### 📈 PHÂN TÍCH XU HƯỚNG DOANH THU

Không chỉ báo cáo, mà còn phân tích:

| Phân tích | Mô tả |
|-----------|-------|
| **So sánh YoY** | So với cùng kỳ năm trước |
| **Trend prediction** | Dự đoán doanh thu tuần/tháng tới |
| **Anomaly detection** | Phát hiện bất thường (tăng/giảm đột ngột) |
| **Product mix analysis** | Sản phẩm nào nên bỏ, nên thêm |
| **Location performance** | Vị trí nào hiệu quả, vị trí nào cần cải thiện |
| **Time-of-day analysis** | Giờ nào bán chạy nhất |


### 📦 NHẬP SẢN PHẨM TỪ EXCEL

Import hàng loạt sản phẩm:

| Tính năng | Mô tả |
|-----------|-------|
| **Template sẵn** | Download file mẫu Excel |
| **Validate trước** | Kiểm tra lỗi trước khi import |
| **Báo lỗi chi tiết** | Dòng nào lỗi, lỗi gì |
| **Import hàng loạt** | 1000+ sản phẩm 1 lần |
| **Update hoặc Create** | Tự động cập nhật nếu đã có |

---

## 📲 ỨNG DỤNG WEB TIẾN BỘ (PWA)

### 📱 Hoạt động như app di động

| Chức năng | Mô tả |
|-----------|-------|
| **Cài về màn hình chính** | Nhấn "Add to Home Screen" |
| **Hoạt động offline** | Xem data đã cache khi mất mạng |
| **Thông báo đẩy** | Nhận push notification như app |
| **Tải nhanh** | Cache thông minh, mở trong 2s |
| **Không cần App Store** | Không phải publish lên store |

---

## 🏆 TẠI SAO CHỌN VMMS?

### ✅ Điểm mạnh vượt trội

| STT | Điểm mạnh | Chi tiết |
|-----|-----------|----------|
| 1 | **Tích hợp POS 2 chiều** | Đồng bộ với cửa hàng tiện lợi - chỉ VMMS có |
| 2 | **Session timeline forensic** | Điều tra giao dịch đến từng giây - bằng chứng cho tranh chấp |
| 3 | **Giám sát real-time nhất** | Cập nhật mỗi 5 giây, không phải 30 giây hay 5 phút như đối thủ |
| 4 | **Loyalty toàn diện nhất** | 4 tier, auto-upgrade, API mở - đối thủ không có hoặc rất cơ bản |
| 5 | **Hệ thống ticket support** | Quản lý yêu cầu hỗ trợ, SLA tracking |
| 6 | **Giám sát hạ tầng** | CPU, RAM, Database, MQTT - cảnh báo tự động |
| 7 | **Phân tích xu hướng** | YoY, prediction, anomaly detection |
| 8 | **Giá theo số lượng B2B** | Bán cho doanh nghiệp với giá sỉ |
| 9 | **Import Excel hàng loạt** | 1000+ sản phẩm 1 lần |
| 10 | **PWA hiện đại** | Hoạt động như app, thông báo đẩy - đối thủ không có |
| 11 | **API mở** | Dễ tích hợp với hệ thống khác - đối thủ thường đóng |

### 🆚 So sánh tổng hợp với đối thủ

| Tính năng | VMMS | Vendon | Dropfoods | Các hãng khác |
|-----------|------|--------|-----------|---------------|
| Tích hợp POS 2 chiều | ✅ | ❌ | ❌ | ❌ |
| Session timeline | ✅ | ❌ | ❌ | ❌ |
| Hệ thống ticket | ✅ | ❌ | ❌ | ❌ |
| Giám sát hạ tầng | ✅ | ⚠️ | ❌ | ❌ |
| Loyalty 4 tier | ✅ | ⚠️ | ❌ | ❌ |
| E-Invoice | ✅ | ❌ | ❌ | ❌ |
| PWA | ✅ | ❌ | ❌ | ❌ |
| API mở | ✅ | ⚠️ | ❌ | ❌ |

---

## 👥 LỢI ÍCH THEO ĐỐI TƯỢNG

### 🏢 Chủ máy bán hàng / Doanh nghiệp

| Vấn đề hiện tại | Giải pháp VMMS | Lợi ích |
|-----------------|----------------|---------|
| Không biết máy lỗi khi nào | Cảnh báo real-time về điện thoại | Giảm 80% thời gian máy chết |
| Mất thời gian kiểm tra tồn kho | Dashboard tồn kho cập nhật liên tục | Tiết kiệm 5 giờ/tuần |
| Đối soát doanh thu thủ công | Báo cáo tự động, xuất Excel | Giảm 90% sai sót kế toán |
| Quản lý nhiều nhân viên | Phân quyền 5 cấp chi tiết | Rõ ràng ai làm gì |
| Khách mua 1 lần rồi quên | Loyalty 4 tier tự động | Tăng 30% khách quay lại |
| Không có hóa đơn VAT | E-Invoice tự động 5 nhà cung cấp | Tuân thủ thuế 100% |

### 🍵 Doanh nghiệp F&B (Chuỗi café, trà sữa...)

| Vấn đề hiện tại | Giải pháp VMMS | Lợi ích |
|-----------------|----------------|---------|
| Mở rộng kênh bán khó | Máy bán tự động + API tích hợp | Triển khai nhanh 1 tuần |
| Quản lý đa chi nhánh phức tạp | Nhóm máy + multi-tenant | Dữ liệu tách biệt rõ ràng |
| Khuyến mãi khó quản lý | Promo code + analytics | Biết ngay chiến dịch nào hiệu quả |
| Hóa đơn thủ công | E-Invoice tự động | Không lo sai sót thuế |
| Không giữ được khách | Customer portal + loyalty | Khách có tài khoản, tích điểm |

### 💰 Nhà đầu tư

| Quan tâm | VMMS đáp ứng |
|----------|--------------|
| **ROI** | Dashboard doanh thu real-time, báo cáo chi tiết từng máy |
| **Rủi ro** | 99.9% uptime, backup tự động, bảo mật cao |
| **Mở rộng** | Hỗ trợ 10,000+ máy, API mở để tích hợp |
| **Tuân thủ** | E-Invoice, Audit log, GDPR-ready |
| **Kiểm soát** | Phân quyền chi tiết, biết ai làm gì |

---

## 📞 LIÊN HỆ TƯ VẤN & DEMO

Để được tư vấn chi tiết và xem demo hệ thống, vui lòng liên hệ:

- 📧 **Email:** sales@vmms.vn
- 📱 **Hotline:** 1900-xxxx
- 🌐 **Website:** https://vmms.vn
- 📍 **Địa chỉ:** [Địa chỉ công ty]

---

## 📋 TÀI LIỆU THAM KHẢO

### Tài liệu kỹ thuật (cho đội IT)
- [Tổng quan dự án](./project-overview-pdr.md)
- [Kiến trúc hệ thống](./system-architecture.md)
- [Mô tả codebase](./codebase-summary.md)
- [Hướng dẫn triển khai](./deployment-guide.md)

### API Documentation
- Swagger UI: `/docs`
- ReDoc: `/redoc`

---

**Version:** 1.3.0 | **Last Updated:** 2026-02-02

*© 2026 VMMS - Vending Machine Management System. All rights reserved.*

---

## 📚 NGUỒN THAM KHẢO THỊ TRƯỜNG

- [Vendon - Loyalty Platform](https://vendon.net/products/loyalty/)
- [Dropfoods Vietnam](https://www.dropfoods.com/en/)
- [Vietnam Vending Machine Market Research](https://www.kenresearch.com/vietnam-retail-vending-machine-market)
- [QuickPik Loyalty Features](https://vendon.net/products/loyalty-app-quickpik/)
