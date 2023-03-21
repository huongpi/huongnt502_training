# 1. Object storage

link tham khảo: https://www.scality.com/topics/object-storage/

- Hiểu một cách đơn giản, với loại lưu trữ này, dữ liệu được tổ chức thành từng object. Mỗi tập hợp dữ liệu sẽ có một ID và một metadata tương ứng. (Object storage organizes information into containers of flexible sizes, referred to as objects.)
- 3 thành phần cơ bản trong Object storage là: dữ liệu, ID và Metadata
## 1.1 ID 

Mỗi khi dữ liệu được thêm vào Object storage, dữ liệu đấy sẽ nhận được một ID, thường là UUID hay GUID. Các ID này là một số nguyên 128 bit.

## 1.2 Metadata

- Để truy cập vào một dữ liệu được lưu trong Object storage, ngoài ID, cần có thêm metadata. Metadata được sử dụng để phân loại dữ liệu trong một Object. 

- Metadata có thể là tên của một địa điểm vật lí, tên một người, ...

- Hiểu một cách đơn giản, metadate như là nhãn, được gán cho dữ liệu. Dựa vào nhãn đấy, ta phân loại, tìm kiếm và sắp xếp dữ liệu dễ dàng hơn.


## 1.3 Dữ liệu 

Dữ liệu để lưu trữ bằng Object storage là tất cả những gì cần lưu trữ. VD như nội dung một cuốn sách, một video hát hò ăn uống, ...

## 1.4 Ưu điểm của Object storage 

- Để làm nồi bật phần này, thì đáng ra OS (Object Storage) nên được giới thiệu cuối cùng,, do nó có những đặc điểm của FS và BL, nên cũng kế thừa ưu và nhược điểm của 2 loại lưu trữ này. 
- Nhìn chung ưu điểm của loại này là giúp lưu trữ những dữ liệu không có cấu trúc (unstructured) nhưng vẫn cho phép truy cập vào dữ liệu này một cách dễ dàng (sử dụng ID và metadata). 
- Khả năng mở rộng OS vô hạn. Mở rộng ra bao nhiêu cũng được, do tính phẳng của loại lưu trữ này. 
- Dễ dàng sao lưu.

## 1.5 Công dụng chính của OS

- lưu trữ dữ liệu không cấu trúc
- lưu trữ tập hợp data lớn
- lưu trữ số lượng lớn dữ liệu nhưng yêu cầu tốc độ truy cập nhanh. 

## 1.6 Giao thức để giao tiếp với OS
- Restful/HTTP protocols ( the same language as the Internet)

# 2. File Storage (FS)

- Hãy nghĩ đến cách các tệp tin, dữ liệu được lưu trữ ở máy tính của bạn. Trong FS, dữ liệu cũng được tổ chức và lưu trữ theo cách tổ chức phân cấp đấy. 
- Khác với OS, để truy cập vào dữ liệu, cần có tên của file và đường dẫn đến file đấy. 
- giao thức để truy nhập đến dữ liệu của FS là: NFS (LInux) và SMB (windows)

## 2.1 Ưu điểm của FS

- File storage có dung lượng chứa lớn và có thể lưu trữ bất cứ thứ gì. Nó rất tốt để lưu trữ các file phức tạp và nhanh chóng cho users điều chỉnh.
- Nhược điểm: do tính chất phân cấp của dữ liệu được lưu trữ, nên khi mở ộng dữ liệu sẽ gây ra khó khăn trong việc phân cấp lại hệ thống tệp tin cùng với quyền truy cập của từng tệp tin đấy. 

## 2.2 Use case 

- Lưu trữ dữ liệu có cấu trúc. 
- Dữ liệu yêu cầu được bảo vệ (data protection, chỗ này em không biết nên dịch sao cho hợp lý) và dễ triển khai.

# 3. Block storage (BS)

- Block storage chia nhỏ dữ liệu thành các khối, và lưu trữ chúng thành các phần riêng biệt. Mỗi khối dữ liệu được cung cấp một mã định danh duy nhất.
- Đây được xem là loại storage giúp chúng ta truy cập dữ liệu nhanh nhất. 
- Giao thức để truy cập dữ liệu của BS: iCSI, FC, và FCoE. 

## 3.2 Ưu điểm của BS

- tốc độ truy xuất dữ liệu nhanh. 
- Khối lưu trữ tách dữ liệu khỏi môi trường người dùng, cho phép dữ liệu đó được trải rộng trên nhiều môi trường. Điều này tạo ra nhiều đường dẫn đến dữ liệu và cho phép người dùng truy xuất nó một cách nhanh chóng. Khi người dùng hoặc ứng dụng yêu cầu dữ liệu từ BS, hệ thống lưu trữ bên dưới sẽ lắp ráp lại các khối dữ liệu và trình bày dữ liệu cho người dùng hoặc ứng dụng.
- Nhược điểm: không có metadata, nên việc lưu trữ dữ liệu không linh hoạt. Loại lưu trữ này phức tạp và có giá thành cao so vs hai loại còn lại. 

## 3.3 Use Case

- Lưu trữ cơ sở dữ liệu 
- Lưu trữ cho RAID volume
- Lưu trữ dữ liệu cho các hệ thống quan trọng ảnh hưởng đến hoạt động kinh doanh
- Storage of data as file systems for operating systems for virtualization software vendors (lưu trữ dữ liệu dưới dạng file system cho ccas nhà cung cấp phần mềm ảo hóa)