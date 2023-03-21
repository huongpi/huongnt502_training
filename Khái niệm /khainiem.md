# 1. Ổ cứng là gì?

- ổ cứng là thiết bị dùng để lưu trữ dữ liệu trong máy tính của bạn. Đây là một trong những thành phần quan trọng nhất của máy tính. Hai thông số được quan trọng nhất của ổ cứng được quan tâm là: tốc độ đọc/ghi dữ liệu và dung lượng lưu trữ. 
- Ngoài đảm nhiệm việc đọc/ghi dữ liệu, ổ cứng còn liên quan đến những yếu tố như: tốc độ khởi động máy tính, độ an toàn của dữ liệu, ...
- Một số loại ổ cứng phổ biến là: HDD, SSD và NVME


# 2. So sánh các loại ổ cứng

Như đã trình bày trên, 3 loại ổ cứng phổ biến là HDD, SSD, NVME.

## 2.1 Ổ cứng HDD

### 2.1.1 Khái niệm 

- Ổ cứng HDD (Hard Disk Drive) là một thiết bị lưu trữ cơ điện, sử dụng bộ lưu trữ từ tính để lưu trữ và truy xuất dữ liệu. Nó là một thiết bị lưu trữ không bay hơi. 
- Ổ đĩa cứng được cài đặt trong hệ thống máy tính, được kết nối trực tiếp với bộ điều khiển đĩa của bo mạch chủ (mainboard). Ổ đĩa cứng là một thiết bị lưu trữ lưu trữ hệ điều hành (OS) , phần mềm đã cài đặt và các tệp máy tính khác. 

### 2.1.2 Cấu tạo 

Hình dưới đây mô tả cấu tạo của ổ cứng HDD: 

![anh1](https://user-images.githubusercontent.com/104249743/226641678-6f3c33d8-11bc-4971-98b7-a944e658aa2b.png)

Cụ thể: 

- Đĩa từ (Disk platters): là một đĩa kim loại tròn. Trong mỗi ổ cứng, nhiều đĩa từ được sếp được gắn vào một động cơ trục chính. Các đĩa từ được sắp xếp theo cấu trúc có sẵn. Cấu trúc này gồm có: track, sector, cluster. 
    - Track: trêm mỗi đĩa từ, có rất nhiều rãnh tròn đồng tâm, xếp lồng vào nhau. Đây là nơi lưu trữ toàn bộ thông tin của ổ cứng. 
    - Sector: Sector là một đơn vị nhỏ hơn của track, là đơn vị cơ bản lưu trữ dữ liệu trên ổ cứng. 
    - Cluster: đúng như tên gọi của nó, nó là cluster. Một nhóm sector gộp chung lại thì thành một cluster. 

- Đầu đọc/ghi (Read/write head): ở chế độ đọc: đầu đọc này chuyển thông tin ở dạng xung tín hiệu thành bit. Ở chế độ ghi, đầu đọc này chuyển thông tin ở dạng bit thành xung tín hiệu. 
- Sealed chamber: Dấu niêm phong băng từ.
- Bezel: vỏ bọc bên ngoài của ổ cứng
- Mouting chassis: 
- Antivibration mount: bộ phận chống rung mỗi khi ổ đĩa đọc/ghi data.
- Head electronics: đầu điện tử
- Drive electronics PCB: mạch xử lý tín hiệu. Đầu đọc liên kết với mạch này thông qua cáp ribbon. 
- Điều khiển truyền động (Head actuator) và trục truyền động (Head arm) là các thành phần điều khiển chuyển động của đầu đọc/ghi.

### 2.1.3 Ưu nhược điểm của ổ cứng HDD\

a. Ưu điểm 
- Giá thành rẻ hơn so với các ổ cứng khác. 
- Tốc độ đọc ghi nhanh hơn ổ đĩa quang.
- Dung lượng của ổ cứng HDD được nhiều hơn so vs các loại ổ cứng khác khi dùng cùng một số tiền để mua. 

b. Nhược điểm
- Tốc độ đọc ghi chậm
- Tạo ra tiếng ồn khi đọc, ghi dữ liệu 
- Tiêu thụ nhiều năng lượng điện

## 2.2 Ổ cứng SSD

### 2.2.1 Khái niệm 

- Ổ cứng SSD (Solid State Drive) là một trong những kiểu ổ đĩa cứng lưu trữ không bay hơi, viết tắt của. SSD là thiết bị lưu trữ dữ liệu trên chip nhớ flash và duy trì dữ liệu ở trạng thái vĩnh viễn, ngay cả khi tắt nguồn. 
-  SSD được xây dựng từ nhiều chip nhớ flash NOR và bộ nhớ flash NAND. Chính vì sử dụng bộ nhớ Flash nên SSD có khả năng lưu trữ dữ liệu vĩnh viễn, kể cả cho máy tính của bạn bị tắt đột ngột.
- So với ổ đĩa điện cơ, SSD có độ trễ thấp hơn và truy cập nhanh hơn. Các thiết bị lưu trữ này lưu trữ dữ liệu trong các ô bán dẫn. Không giống như ổ đĩa HDD, SSD không có bất kỳ bộ phận chuyển động nào. Đó là lý do tại sao chúng được gọi là ổ cứng thể rắn.

### 2.2.2 Kiến trúc 

Hình dưới đây mô tả kiến trúc của ổ cứng SSD: 

![anh2](https://user-images.githubusercontent.com/104249743/226641754-97f9d35b-12c7-4b9f-8438-1c0bdfdbddea.png)

Cụ thể: 

- Những con chip flash sẽ được lắp cố định trên một bo mạch chủ khoảng từ 10-60 NAND của hệ thống, trên card PCI hoặc cũng có thể là lắp vào trong một chiếc hộp có hình dạng và kích thước giống như ổ cứng nhưng nhỏ hơn.
- Ổ cứng SSD chứa: bộ điều khiển vi mô, bộ đệm, hiệu chỉnh và module giao diện flash. 
- Để gửi và nhận dữ liệu nhanh chóng, SSD sử dụng một tấm các ô điện. Những tấm này được phân chia thành từng phần, những phần này được gọi là “trang” và đây cũng chính là nơi lưu trữ dữ liệu cho máy tính của bạn. Những trang này sau khi được gộp lại sẽ tạo thành các khối. Bởi không có bộ phận chuyển động nên SSD được gọi là ổ cứng thể rắn
- Không như HDD, SDD chỉ có khả năng ghi vào một trang trống trong một khối. Điều này có nghĩa là bạn không thể ghi đè trực tiếp dữ liệu lên từng trang riêng lẻ.
- SSD xử lý việc xóa dữ liệu bằng cách xác định dữ liệu được đánh dấu là không sử dụng, sau đó dữ liệu này sẽ được chuyển vào một khối của bộ nhớ. Việc tiếp theo chính là loại bỏ toàn bộ khối đó và xác định lại dữ liệu từ bộ nhớ trở lại khối trong khi để trống các trang không sử dụng.


### 2.2.3 Ưu nhược điểm của ổ cứng HDD\

a. Ưu điểm 
- Tiêu thụ ít điện năng
- Tốc độ đọc ghi dữ liệu nhanh 
- Không tạo ra tiếng ồn 

b. Nhược điểm
- Giá thành cao 
- Khó khôi phục giữ liệu khi dữ liệu bị mật 
- Dung lượng lưu trữ ít hơn HDD

### 2.2.4 So sánh ổ cứng HDD và ổ cứng SSD

| HDD      | SSD |
|----------|-----|
|Thời gian đọc ghi nhanh |  Thời gian đọc ghi lâu   |
|Độ trễ thấp       |Độ trễ cao |
|Do không sử dụng nhiều thành phần vật lý nên trọng lượng của SSD khá nhẹ          |Trọng lượng lớn hơn SSD     |
|    Việc truyền dữ liệu không theo trình tự      | Việc truyền dữ liệu được thực hiện tuần tự    |
|Không tạo ra tiếng ồn lúc hoạt động      |Tạo ra tiếng ồn lúc hoạt động     |
|Kích thước nhỏ gọn          |Kích thước lớn hơn SSD    |
|Tạo ra ít nhiệt lượng => thiết bị bền hơn          |Tạo ra nhiều nhiệt lượng => thiết bị kém bền hơn    |
|Tiêu thụ năng lượng điện ít        |Tiêu thụ năng lượng điện nhiều   |
|Thời gian khỏi động máy tính nhanh hơn HDD          |Thời gian khởi động máy tính lâu hơn SSD    |
|Tốc độ mở tệp tin, chạy chương trình nhanh        |Tốc độ mở tệp tin,chạy chương trình chậm     |
|Không có rung động khi SSD hoạt động          |Khi HDD hoạt động, tạo ra chuyển động rung nhất định     |


### 2.2.5 ổ SSD SATA và ổ SSD NVME

Hai loại SSD này được phân biệt với nhau bằng chuẩn kết nối giữa ổ SSD và PC. 

SSD SATA: 
- Sử dụng giao diện SATA với tốc độ truyền dữ liệu tối đa là 6Gbps, thấp hơn các interface mới hơn(NVME). Đây là loại SSD có hiệu năng thấp nhất.
- SSD loại này sử dụng một connector riêng để cắm vào máy tính xách tay và một loại cap riêng để kết nối với mainboard của PC. Khi đã kết nối được rồi, ổ đĩa chưa thực sự nói chuyện với hệ thống, nó cần có một giao diện điều khiển máy chủ (host controller). Đó chính là AHCI. 
- SSD loại này có mức băng thông lớn gấp 3, 4 lần so với ổ cứng HDD. 
- Đây là loại SSD có giá cả phải chăng và kích thước cũng nhỏ gọn. 

SSD NVME: 
- Sử dụng giao thức NVME được thiết kế đặc biệt dành cho ổ SSD. Ổ SSD NVME giao tiếp trực tiếp với CPU hệ thống thông qua khe căm PCIe, giúp cho mức hiệu năng và tốc độ truyền dữ liệu là cao nhất. 

|NVME|SATA|
|-------------|---------|
|Cần cân nhắc sử dụng NVME do các thiết bị cũ có thể không tương thích với NVME vì không có các kết nối cần thiết để sử dụng khe cắm PCIe của NVMe|Không phải cân nhắc đến tính tương thích của SSD đối với máy tính|
|Giúp khởi động máy tính nhanh hơn|Khởi động máy tính không nhanh như NVME|
|Phù hợp đối với những máy tính sử dụng để chạy các trò chơi vì nó giúp tăng tốc thời gian tải trò chơi||
