🛠️ Cơ chế mô phỏng

Đoàn xe (4–6 xe)

Luôn duy trì số xe trong khoảng 4–6.

Nếu < 4 → spawn xe mới từ phía sau.

Nếu > 6 → không thêm xe.

Platooning

Xe leader đi đầu, tốc độ cố định (vd 2 px/frame).

Xe phía sau nối đuôi, giữ khoảng cách 70 px.

Xe rời đoàn

Ngẫu nhiên mỗi 8–12 giây, chọn 1 xe (không phải leader) → tăng tốc, chạy thẳng và biến mất khỏi canvas.

Nếu leader rời → xe kế tiếp thành leader mới.

Địa hình (ngẫu nhiên)

Màn hình chia thành “khu vực địa hình” dài vài trăm pixel:

Cao tốc: mạng tốt, xe chạy mượt.

Đô thị: nhiều nhiễu, jitter tăng.

Hầm: mất sóng gNB, xe chỉ còn V2V.

Sau mỗi đoạn (vd 600–1000px), chọn random 1 địa hình mới → hiển thị bằng màu nền hoặc dải màu trên canvas.

Kết nối mạng

Nếu cao tốc/đô thị → leader kết nối gNB, xe sau nối hop-by-hop.

Nếu hầm → chỉ còn V2V, log hiển thị cảnh báo “🚨 Mất kết nối gNB, fallback V2V”.

Hiển thị trực quan

Canvas: xe tải nối đuôi nhau.

Dải nền chạy ngang tượng trưng cho địa hình.

Log: sự kiện spawn, rời đoàn, đổi địa hình, kết nối mạng.
