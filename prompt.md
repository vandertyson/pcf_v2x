Tạo một mô phỏng trực quan bằng HTML + JS (canvas) về truck platooning với các yêu cầu sau:

1. Platoon xe tải:
   - Số lượng xe ngẫu nhiên 4–6 xe.
   - Leader luôn ở đầu (bên phải nhất), chạy hướng trái → phải trên làn ngoài cùng.
   - Xe rời đoàn: chuyển làn, tăng tốc vượt leader, biến mất khỏi mô phỏng.
   - Xe nhập đoàn: di chuyển từ từ vào platoon, chuyển kết nối V2I → V2V.
   - Xe có hình dạng khác nhau: xe tải dài đỏ, xe con ngắn xanh, xe bus dài xanh lá.

2. Xe ngoài platoon:
   - Chạy các làn khác, luôn kết nối với trạm gNodeB (V2I).
   - Số lượng xe tùy địa hình: City 7–10 xe, Highway/Tunnel 4–5 xe.

3. Địa hình & trạm gNodeB:
   - City: trạm cách nhau 100m, nhiều xe ngoài platoon.
   - Tunnel: không có trạm, ít xe ngoài platoon.
   - Highway: ít trạm, 4–5 xe ngoài platoon.
   - Cảnh vật và trạm thay đổi liên tục khi xe chạy qua.
   - Nền canvas thay đổi theo địa hình (city, highway, tunnel).

4. Hiển thị trạng thái & kết nối:
   - Vẽ dây kết nối từ xe platoon đến leader (V2V) hoặc đến gNodeB (V2I), V2V màu cam, V2I màu vàng.
   - Hiển thị bảng theo dõi tất cả xe: ID, loại xe, kết nối, tốc độ, độ trễ.
   - Leader luôn ở đầu, hướng trái → phải.

5. Animation mượt & liên tục:
   - Xe chạy vòng lặp, cảnh vật thay đổi liên tục.
   - Xe tách đoàn, nhập đoàn mượt mà.
   - Các xe ngoài platoon chạy bình thường.

6. Controls:
   - Nút bấm kích hoạt xe rời/nhập đoàn (1–2 xe ngẫu nhiên).
   - Bảng trạng thái cập nhật tự động.

7. Yêu cầu:
   - File HTML + JS hoàn chỉnh, chạy trực tiếp trên trình duyệt.
   - Mô phỏng đầy đủ animation, cảnh vật, xe platoon, xe ngoài platoon, kết nối và bảng theo dõi.
