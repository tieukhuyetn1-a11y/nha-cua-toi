# THIÊN QUANG — NGỌC QUANG | Quyết định nghiên cứu cuối
26/11/2026. Bản nghiên cứu, không dùng gia công/thi công. Kế thừa R15 cb867f1d3a78ddb6b574feb938bf2eb1e350a63a; R16 diễn họa chưa xác nhận commit.

## Quyết định có điều kiện
Ưu tiên khảo sát C: kính 1600×2350, dịch Tây 275 mm so với phương án cân giữa ô mái. Tọa độ x cục bộ từ mép Tây ô mái 2800: kính [325,1925]; lõi [250,2000], y=[800,1550]. Dải đặc Tây 325, Đông 875. Lõi giao kính 1,20/1,3125 m² = 91,43%, trước 1,05 m² = 80%. Không thay đổi cầu thang 8–4–9, 21 cổ, cao 3200; nhà lọt lòng 3900; vế 800, mặt xây/hoàn thiện 250/270; hành lang 1350/1100. Không khóa vị trí kính thi công trước khảo sát dầm, khung và thoát nước. A là đối chứng/dự phòng nếu C vướng kết cấu.

## Mô hình có thể tái lập
Chạy node solar-model.js. 525 điểm 50 mm; 12 ngày đại diện, 17 giờ mặt trời lấy mẫu mỗi ngày (8–16h, bước 0,5h). Vĩ độ 10,9°, Bắc lệch +5°, mái dốc 7° về Nam; cao độ mép thấp 6500 giả định. Tia nắng qua mái, kiểm tra thêm lõi +3200 khi xét điểm z=0. Chỉ số có trọng số sin cao độ mặt trời (giả định DNI không đổi). Khuếch tán: tích phân số bầu trời đồng đều qua kính, có lọc lõi cho tầng trệt. Không phải lux, dữ liệu thời tiết năm, render vật lý, CFD hay mô phỏng đầy đủ vật cản/phản xạ. Các ngày không có tia trực tiếp không có nghĩa là tối.

|Phương án|x Tây mm|Rộng kính mm|Bao phủ lõi|Chỉ số trực tiếp +3200|Chỉ số trực tiếp z=0|
|---|---:|---:|---:|---:|---:|
|A|600|1600|80,00%|0,149944|0,029426|
|B|400|1600|91,43%|0,153021|0,029826|
|C|325|1600|91,43%|0,153596|0,030002|
|D|250|1600|91,43%|0,152669|0,029943|
|E|150|1600|85,71%|0,150501|0,030064|
|F|250|1750|100%|0,167052|0,032597|
|G|400|2000|91,43%|0,186727|0,036679|

C so với A: trực tiếp +3200 tăng 2,44%, z=0 tăng 1,96%; khuếch tán lý tưởng +3200 tăng 0,97%, z=0 tăng 1,40%. E có chỉ số z=0 nhỉnh hơn C rất ít nhưng dải Tây chỉ 150, bao phủ lõi và chỉ số tầng trên thấp hơn. Các khác biệt nhỏ chưa đủ kết luận thống kê. Ưu tiên C do cân tâm lõi, không tăng diện tích và còn phương án A dự phòng. Không tuyên bố C tối ưu tuyệt đối.

## Nhiệt, gió, nước, chi phí
Diện tích kính nghiêng 3,788 m²; Qsolar=A*G*SHGC: 909–1212 W tại G=800 W/m² và SHGC=.30–.40. Dịch kính không thay đổi tải thu qua kính khi bỏ qua che bóng. F/G tăng diện tích 9,375%/25%. Dự toán tham chiếu R12: 17,586 triệu A/C trước phát sinh khung; F khoảng 18,12; G khoảng 19,01 theo chênh kính/mái đặc (2,3/0,8 triệu/m² nghiêng). Không phải báo giá.
Thông gió: giữ khe thoáng hữu hiệu mục tiêu R12 0,28 m² nếu có đường cấp và thoát thật; không suy ra ACH. Dịch kính không tự tăng lưu lượng. Thoát nước: thử tính 15m²×400mm/h=1,667 L/s, chưa có IDF và diện tích hứng khảo sát. Cần máng, tràn độc lập, chống ngưng tụ và kiểm tra mưa tạt; không cắt dầm. Dải Tây 325 mm chưa chứng minh đủ neo/khung/chống thấm.

## Điều kiện HOLD
H01 khảo sát; H02 kết cấu kính/khung/neo/tải gió; H03 thông thủy/lan can/cháy/bảo trì; H04 thông số kính và sơn; H05 mô hình có vật cản và kiểm tra lux; H06 IDF/thoát nước/chống thấm; H07 cấp thoát khí; H08 điện và độ rọi; H09 báo giá; H10 phê duyệt. Tất cả mở. Đề xuất kết thúc nghiên cứu hình thức, chuyển khảo sát kỹ thuật và nghiệm thu. Không dùng ảnh AI để xác nhận hình học. Không tuyên bố website đã cập nhật nếu chưa có bằng chứng deploy.
