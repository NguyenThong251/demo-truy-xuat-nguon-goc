# Demo: Truy xuất nguồn gốc bằng mã QR

Bản online: https://nguyenthong251.github.io/demo-truy-xuat-nguon-goc/ (repo riêng NguyenThong251/demo-truy-xuat-nguon-goc)
Chạy thử trên máy: `python3 -m http.server 8790` trong thư mục này → http://localhost:8790/
(Thương hiệu "Nông trại Lá Xanh" và mọi số liệu đều là MẪU, trang có ghi rõ "BẢN DEMO".)

## Có gì trong demo
- **Trang khách quét** (`#/sp/<mã>`): báo hàng chính hãng / mã đã bị quét nhiều lần (nghi sao chép tem) / mã không tồn tại (nghi hàng giả);
  thông tin lô, vùng trồng, mã vùng trồng, bản đồ, hành trình sản phẩm, chứng nhận, kiểm nghiệm; chuyển tiếng Việt / tiếng Anh (cho khách xuất khẩu).
- **Niêm phong dữ liệu SHA-256**: nút "Thử sửa ngày thu hoạch" cho thấy dữ liệu bị sửa là lộ ngay. Bản thật có thể ghi dấu vân tay lên blockchain công khai.
- **Trang quản lý** (`#/quan-ly`): tạo lô, sinh mã ngẫu nhiên không trùng (tối đa 60/lô), in tem QR (trang in A4), thống kê lượt quét, cảnh báo mã nghi sao chép.

## Giới hạn của bản demo (nói rõ với khách)
- Dữ liệu và lượt quét lưu trên trình duyệt đang mở. Bản thật: máy chủ + cơ sở dữ liệu, đếm quét từ mọi điện thoại, có đăng nhập cho nhà sản xuất.
- QR của lô tạo mới chỉ mở được trên máy đã tạo; QR mẫu có sẵn mở được ở mọi máy khi demo đã đưa lên mạng.

## Gói bán (giá đề xuất 4–6 triệu, theo số sản phẩm/tính năng)
- Cơ bản ~4tr: trang quản lý, tạo lô, in tem, trang khách quét, 2 ngôn ngữ, chống sao chép tem.
- Nâng cao ~6tr: thêm nhiều tài khoản nhân viên, nhập nhật ký từ điện thoại, xuất báo cáo cho đối tác/siêu thị, ghi dấu vân tay lên blockchain.
- Hosting/tên miền khách trả; có thể kèm gói chăm sóc website 300k–600k/tháng.
- Khách mục tiêu: HTX, nông trại sầu riêng/cà phê/trái cây xuất khẩu, sản phẩm OCOP, xưởng thực phẩm, mật ong, trà.
