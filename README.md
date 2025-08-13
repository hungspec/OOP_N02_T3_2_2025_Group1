# Textbook Library Management System 🎉

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=24&pause=1000&color=FF4B4B&center=true&vCenter=true&width=700&height=80&lines=Chào+mừng+đến+với+ứng+dụng+quản+lí+thư+viện+giáo+trình;Nhóm+08+OOP_N02_T3_2_2025_" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://github.com/phamkheng/OOP_N02_T3_2_2025_Group1">
    <img src="https://raw.githubusercontent.com/acervenky/animated-github-badges/master/assets/devbadge.gif" width="50" alt="Developer Badge" />
    <img src="https://raw.githubusercontent.com/acervenky/animated-github-badges/master/assets/contribbadge.gif" width="50" alt="Contributor Badge" />
  </a>
</p>

---

📋 Mục lục

1. [Giới thiệu]
2. [Thành viên] 
3. [Phân tích đối tượng] 
4. [cấu trúc thư mục]  
5. [cấu trúc lớp và phân lớp] 
6. [kiểm thử chức năng] 
7. [Các chức năng chính]  
8. [Class Diagram]
9. [Activity Diagram]  
10. [Mô tả đối tượng] 
11. [Giao diện chương trình] 
12. [Chức năng nổi bật]
13. [Công nghệ sử dụng]
14. [Hướng phát triển]
15. [Cài đặt--Chạy]
16. [Tài liệu tham khảo]


## ✨ Giới thiệu

Ứng dụng **Quản lý Thư viện giáo trình** được xây dựng theo phong cách **Lập trình Hướng đối tượng (OOP)**, giúp bạn:

- Quản lý giáo trình (`Book`)  
- Quản lý bạn đọc (`Reader`)  
- Theo dõi lịch sử mượn/trả (`Loan`)

---

## 👥 Thành viên

| Họ tên               | MSSV      | GitHub                        |
|----------------------|-----------|-------------------------------|
| Phạm Năng Khang      | 24100032  | [@phamkheng](https://github.com/phamkheng) |
| Trần Quốc Việt Hùng  | 24100015  | [@hungspec](https://github.com/hungspec)   |
| Phạm Việt Khoa       | 24100058  | [@pvkhoa](https://github.com/pvkhoa)       |
| Nguyễn Lệ Thu        |           | [@nglthu](https://github.com/nglthu)       |

---

## 🧠 Phân tích đối tượng

### 1. 👤 Người đọc (`Reader`)
- **Thuộc tính**: ID, tên, số điện thoại, email.
- **Chức năng**:
  - Đăng ký người đọc
  - Hiển thị thông tin
  - Xóa người đọc khỏi danh sách

### 2. 🧾 Giáo trình (`Book`)
- **Thuộc tính**: ID, tên, tác giả, trang thái (có sẵn/ trống), số lượng.
- **Chức năng**:
  - cập nhập giáo trình mới
  - Hiển thị danh sách giáo trình
  - Tìm kiếm giáo trình
  - Xóa giáo trình khỏi danh sách

### 3. 📦 Dịch vụ mượn/trả (`Loan`)
- **Thuộc tính**: ID, book, reader, ngày mượn, ngày trả, trạng thái
- **Chức năng**:
  - Hiển thị thông tin
  - Cập nhật sau khi mượn/trả

---
## 🗂️ Cấu trúc thư mục

```Project/
Project/
├── QuanliGiaoTrinh_springboot/       # Spring Boot
│   ├── complete/
│   │   ├── gradle/wrapper
│   │   ├── src/
│   │   │   ├── main/
│   │   │   │   ├──java/com/example/servingwebcontent/
│   │   │   │   │   ├──Component
│   │   │   │   │   ├──Controller                                              # Các controller
│   │   │   │   │   ├──Database                                                # Các service, kết nối, truy vấn cơ sở dữ liệu
│   │   │   │   │   ├──Model                                                   # Các class mô hình dữ liệu
│   │   │   │   │      ├──Book.java
│   │   │   │   │      ├──Reader.java
│   │   │   │   │      ├──Loan.java
│   │   │   │   │   ├──test                                                    # File test 
│   │   │   │   │   ├──ServingWebContentApplication.java                       # Main() để chạy ứng dụng
│   │   │   │   ├──resources/
│   │   │   │        ├── static/                                               
│   │   │   │        ├── templates/                                            # Giao diện
│   │   │   │        └── application.properties                                # File cấu hình ứng dụng
│   │   │   ├── test/java/com/example/servingwebcontent/                       # File test ứng dụng
│   │   ├── target
│   │   └── ...
│   └── ...
├── images
└── README.md                           # Tài liệu mô tả dự án
```

---

## 🧱 Cấu trúc lớp và phân lớp

### Các lớp chính:

- `Reader`: thông tin người đọc
- `Book`: thông tin của giáo trình 
- `Loan`: phiếu mượn/trả
- `Main`: lớp chạy chính của chương trình

---
## ✅ Kiểm thử chức năng

| Lớp         | Chức năng kiểm thử chính                                              |
|-------------|------------------------------------------------------------------------|
| `Reader`    | Đăng ký, xóa, chỉnh sửa, hiển thị thông tin                           |
| `Book`      | cập nhập giáo trình, xóa, hiển thị danh sách                          |
| `Loan`      | cập nhập hạn mượn/trả giáo trình, hiển thị phiếu mượn/trả             |

---
## 🛠️ Chức năng chính

- **Quản lý người đọc**:
  - Thêm / Sửa / Xóa người đọc

- **Quản lý giáo trình**:
  - Thêm / Sửa / Xóa giáo trình
  - Cập nhật số lượng giáo trình sau mỗi lần mượn/trả

- **Quản lý mượn/trả**:
  - cập nhập ngày mượn/trả
  - Hiển thị danh sách mượn

- **Lưu trữ dữ liệu**:
  - Dữ liệu được lưu vào file nhị phân 
  - Sử dụng `ObjectOutputStream`, `ObjectInputStream`
  - Áp dụng `ArrayList`, `Map`,... để quản lý dữ liệu trong bộ nhớ

---


## 📊 Class Diagram 
![Class Diagram ](../main/images/class-diagram.png)

## 📊 Activity Diagram – Mượn giáo trình
![Activity Diagram Mượn sách](../main/images/muonsach.png)
## 📊 Activity Diagram – Trả giáo trình 
![Activity Diagram ](../main/images/trasach.png)
## 📊 Activity Diagram – tìm giáo trình  
![Activity Diagram ](../main/images/timsach.png)
## 📊 Activity Diagram – đăng ký bạn đọc mới
![Activity Diagram ](../main/images/dangkybandocmoi.png)
## 📊 Activity Diagram – xóa bạn đọc
![Activity Diagram ](../main/images/xoabandoc.png)
## 📊 Activity Diagram – tìm kiếm bạn đọc
![Activity Diagram ](../main/images/timkiembandoc.png.png)


📚 Mô tả đối tượng
Book

Thuộc tính: title, author, numPages, status (Available / Unavailable)

Hành vi: checkAvailability(), markAsBorrowed(), markAsReturned(), display()

Reader

Thuộc tính: readerID, name, email, phone, borrowedBooks (List<Loan>)

Hành vi: borrowBook(Book), returnBook(Book), viewBorrowHistory()

Loan

Thuộc tính: loanID, book, reader, loanDate, returnDate, status

Hành vi: markReturned(Date), isOverdue(Date)

---

## 🖼️ Giao diện chương trình (Console)
// chưa đẩy 

---

## 🌟 Chức năng nổi bật

- **Xử lý nhập sai dữ liệu, đăng kí**
- **Tìm kiếm người đọc, giáo trình qua mã số, tên**
- **Hiển thị dữ liệu chi tiết và rõ ràng dưới giao diện console**

---
## 💡 Công nghệ sử dụng

- Ngôn ngữ lập trình: **Java**
- Mô hình hướng đối tượng (OOP)
- **Framework**: [Spring Boot](https://spring.io/projects/spring-boot)
  - Quản lý luồng xử lý, cấu trúc theo mô hình MVC
- Giao diện: Console (text-based)
- Lưu trữ: File nhị phân 
- Cấu trúc dữ liệu: `ArrayList`, `LinkedList`, `Map`,...

---

🚀 Hướng phát triển 

-Thêm giao diện đồ họa (GUI)

-Kết nối cơ sở dữ liệu (JDBC / MySQL / SQLite)

-Tích hợp RESTful API (Spring Boot)

---
## ⚙️ Cài đặt & Chạy

git clone https://github.com/phamkheng/OOP_N02_T3_2_2025_Group1.git
cd OOP_N02_T3_2_2025_Group1
Mở project bằng IDE hoặc:
- javac src/*.java
- java Main
---
## 📚 Tài liệu tham khảo

- Slide bài giảng môn Lập trình Hướng Đối Tượng – GVHD: TS.Nguyễn Lệ Thu
- Java Docs – Oracle
- Stack Overflow – Community

---










