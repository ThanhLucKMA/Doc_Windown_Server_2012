# Tocpic Win Server 2012 
### I. Thực hiện allow port, allow ip trên window fw
#### 1.1. Allow Port
#### Bước 1 : Vào `Server Manager` -> `Local Server` -> Tại Properties có thuộc tính Windowsn Firewall click vào `Public:On` để mở cửa sổ quản lý firewall 
![text](./Images/Screenshot%20from%202025-04-08%2015-10-17.png)
#### Bước 2 : Vào `Advanced Setting`
![text](./Images/Screenshot%20from%202025-04-08%2015-15-49.png)
#### Bước 3 : Chọn `Inbound Rules` -> chọn `New Rule` để tạo rule
![text](./Images/Screenshot%20from%202025-04-08%2015-21-40.png)
#### Bước 4 : Chọn loại Rule là Port -> `Next`
![text](./Images/Screenshot%20from%202025-04-08%2015-24-21.png)
#### Bước 5 : Chọn giao thức là TCP và điền port -> `Next`
![text](./Images/Screenshot%20from%202025-04-08%2015-26-27.png)
#### Bước 6 : Action chọn `Allow Connect`
![text](./Images/Screenshot%20from%202025-04-08%2015-33-00.png)
#### Bước 7 : Chọn Profile 
![text](./Images/Screenshot%20from%202025-04-08%2015-35-09.png)
#### Bước 8 : Đặt tên cho port 
![text](./Images/Screenshot%20from%202025-04-08%2015-35-59.png)

---
#### 1.2. Allow IP
#### Bước 1 : Vào `Server Manager` -> `Local Server` -> Tại Properties có thuộc tính Windowsn Firewall click vào `Public:On` để mở cửa sổ quản lý firewall 
![text](./Images/Screenshot%20from%202025-04-08%2015-10-17.png)
#### Bước 2 : Vào `Advanced Setting`
![text](./Images/Screenshot%20from%202025-04-08%2015-15-49.png)
#### Bước 3 : Chọn `Inbound Rules` -> chọn `New Rule` để tạo rule
![text](./Images/Screenshot%20from%202025-04-08%2015-21-40.png)
#### Bước 4 : Rule type chọn `Custom`
![text](./Images/Screenshot%20from%202025-04-08%2015-44-48.png)
#### Bước 5 : Progaram chọn `All Program`
![text](./Images/Screenshot%20from%202025-04-08%2015-45-54.png)
#### Bước 6 : Chọn các options của Protocol and Port 
![text](./Images/Screenshot%20from%202025-04-08%2015-48-08.png)
#### Bước 7 : Ở Scope phần Remote IP Address chọn `These IP addresses` -> `Add` -> Nhập địa chỉ IP cho phép -> `Next`
![text](./Images/Screenshot%20from%202025-04-08%2015-51-31.png)
#### Bước 8 : Ở bước Action chọn `Allow the connection`
![text](./Images/Screenshot%20from%202025-04-08%2015-54-28.png)
#### Bước 9 : Chọn các options ở Profile 
![text](./Images/Screenshot%20from%202025-04-08%2015-55-28.png)
#### Bước 10 : Đặt tên cho rule ->`Finish`  
![text](./Images/Screenshot%20from%202025-04-08%2015-56-33.png)

---
### II. Thực hiện block port, block ip trên window fw
#### 2.1. Block port 
#### Bước 1 : Vào `Server Manager` -> `Local Server` -> Tại Properties có thuộc tính Windowsn Firewall click vào `Public:On` để mở cửa sổ quản lý firewall 
![text](./Images/Screenshot%20from%202025-04-08%2015-10-17.png)
#### Bước 2 : Vào `Advanced Setting`
![text](./Images/Screenshot%20from%202025-04-08%2015-15-49.png)
#### Bước 3 : Chọn `Inbound Rules` -> chọn `New Rule` để tạo rule
![text](./Images/Screenshot%20from%202025-04-08%2015-21-40.png)
#### Bước 4 : Chọn loại Rule là Port -> `Next`
![text](./Images/Screenshot%20from%202025-04-08%2015-24-21.png)
#### Bước 5 : Chọn Protocol and Port 
![text](./Images/Screenshot%20from%202025-04-08%2016-08-29.png)
#### Bước 6 : Actions chọn `Block the Connection`
![text](./Images/Screenshot%20from%202025-04-08%2016-03-23.png)
#### Bước 7 : Chọn options của profile 
![text](./Images/Screenshot%20from%202025-04-08%2015-55-28.png)
#### Bước 10 : Đặt tên cho rule
---
#### 2.2. Block IP
#### Bước 1 : Vào `Server Manager` -> `Local Server` -> Tại Properties có thuộc tính Windowsn Firewall click vào `Public:On` để mở cửa sổ quản lý firewall 
![text](./Images/Screenshot%20from%202025-04-08%2015-10-17.png)
#### Bước 2 : Vào `Advanced Setting`
![text](./Images/Screenshot%20from%202025-04-08%2015-15-49.png)
#### Bước 3 : Chọn `Inbound Rules` -> chọn `New Rule` để tạo rule
![text](./Images/Screenshot%20from%202025-04-08%2015-21-40.png)
#### Bước 4 : Rule type chọn `Custom`
![text](./Images/Screenshot%20from%202025-04-08%2015-44-48.png)
#### Bước 5 : Progaram chọn `All Program`
![text](./Images/Screenshot%20from%202025-04-08%2015-45-54.png)
#### Bước 6 : Chọn các options của Protocol and Port 
![text](./Images/Screenshot%20from%202025-04-08%2015-48-08.png)
#### Bước 7 : Ở Scope phần Remote IP Address chọn `These IP addresses` -> `Add` -> Nhập địa chỉ IP cho phép -> `Next`
![text](./Images/Screenshot%20from%202025-04-08%2015-51-31.png)
#### Bước 8 : Action chọn `Block the Connection`
![text](./Images/Screenshot%20from%202025-04-08%2016-03-23.png)
#### Bước 9 : Chọn options của profile 
![text](./Images/Screenshot%20from%202025-04-08%2015-55-28.png)
#### Bước 10 : Đặt tên cho rule

---

### III . Thực hiện giới hạn port, giới hạn ip trên window fw chỉ cho phép ip chỉ định truy cập
### Ví dụ:
### * Chỉ cho IP 203.113.130.5 truy cập port 3306 (MySQL)
### * Mọi IP khác đều bị chặn không được vào port này.
#### Bước 1 : Chọn Inbound Rules -> New Rule
#### Bước 2 : Chọn Port -> Next
#### Bước 3 : Chọn TCP (hoặc UDP nếu dùng). Nhập số port: 3306 -> Next
#### Bước 4 : Chọn Allow the connection -> Next
#### Bước 5 : Tick chọn các profile: Domain, Private, Public -> Next
#### Bước 6 : Đặt tên rule `Allow MySQL 3306 from 203.113.130.5` -> Finish
#### Bước 7 : Double click vào rule bạn vừa tạo -> Chọn tab Scope -> Ở mục Remote IP address, chọn: `These IP addresses` -> Nhấn Add → nhập IP: 203.113.130.5 -> OK
---
### IV. Thực hành cài đặt Webserver IIS, trên Webserver IIS
- Cài đặt website wordpress mặc định
- Cài đặt SSL
### Phần 1 : Cài Web Server IIS 
#### Bước 1 : `Server Manager` -> `Add roles and features`
![text](./Images/Screenshot%20from%202025-04-08%2016-42-36.png)
#### Bước 2 : Nhấn Next cho đến khi tới bước Server Roles
![text](./Images/Screenshot%20from%202025-04-08%2016-50-03.png)
####
![text](./Images/Screenshot%20from%202025-04-08%2016-54-34.png)
#### Bước 3 : Cứ `next` -> `Install` -> Đợi quá trình cài sau khi cài xong restart lại win server và truy cập trang defaul để kiểm tra 
![text](./Images/Screenshot%20from%202025-04-08%2022-07-15.png)
### Phần 2 : Cài Wordpress 
#### Bước 1 : Tải wordpress : `https://wordpress.org/latest.zip`
#### Bước 2 : Giải nén vào `C:\inetpub\wwwroot\wordpress`
#### Buocs 3 : Trong IIS
- Add Website 
  + Site name: wordpress.local
  + Physical path: C:\inetpub\wwwroot\wordpress
  + Binding: Port 80, Hostname: wordpress.local
####
![text](./Images/Screenshot%20from%202025-04-08%2022-21-16.png)
- Trỏ DNS:
  + Mở file C:\Windows\System32\drivers\etc\hosts
  + Thêm dòng: `127.0.0.1 wordpress.local`
####
![text](./Images/Screenshot%20from%202025-04-08%2022-23-58.png)
#### Bước 4 : Cài Php Manager sau đó cài phiên bản php, cài Mysql 

####
![text](./Images/Screenshot%20from%202025-04-09%2009-30-16.png)

#### Bước 5 : Kiểm tra kết quả 
- Kết quả truy cập vaò domain để kiểm tra
![text](./Images/Screenshot%20from%202025-04-09%2010-31-47.png)
#### 
![text](./Images/Screenshot%20from%202025-04-09%2011-01-26.png)


### Phần 3 : Cài SSL 
#### Bước 1 : Lấy cert và key trên ZeroSSL (Bước này tạo .well-know/pki-validation để xác thực domain)
#### Bước 2 : Tạo file pem `type ten_file.crt ten_file_ca.crt > fulkchain.crt` 
![text](./Images/Screenshot%20from%202025-04-09%2011-41-28.png)
#### Bước 3 : Xuất file PFX tại `https://www.sslshopper.com/ssl-converter.html`
![text](./Images/Screenshot%20from%202025-04-09%2012-00-23.png)
#### Bước 4 : Import PFX 
#### 
![text](./Images/Screenshot%20from%202025-04-09%2012-02-58.png)
#### 
![text](./Images/Screenshot%20from%202025-04-09%2012-04-27.png)
####
![text](./Images/Screenshot%20from%202025-04-09%2012-05-37.png)
####
![text](./Images/Screenshot%20from%202025-04-09%2012-06-36.png)
#### Bước 5 : Cấu hình website với SSL
#### Trên màn hình Internet Information Services (IIS) Manager, chọn `Site`, sau đó chuột phải vào trang web và chọn `Edit Binding…`
![text](./Images/Screenshot%20from%202025-04-09%2012-09-07.png)
#### Chọn `Add`
![text](./Images/Screenshot%20from%202025-04-09%2012-10-06.png)
####
![text](./Images/Screenshot%20from%202025-04-09%2012-12-52.png)
#### Kết quả 
![text](./Images/Screenshot%20from%202025-04-09%2012-21-11.png)
---
### Phần 4 : Cài SQL Server 
![text](./Images/Screenshot%20from%202025-04-09%2012-52-24.png)