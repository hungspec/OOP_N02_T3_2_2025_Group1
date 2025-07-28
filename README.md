# Library Management System 🎉

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=24&pause=1000&color=FF4B4B&center=true&vCenter=true&width=500&height=50&lines=Chào+mừng+đến+với+ứng+dụng+thư+viện;Nhóm+01+OOP_N02_T3_2_2025_" alt="Typing SVG" />
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
3. [Ứng dụng] 
4. [Yêu cầu]  
5. [Cài đặt & Chạy] 
6. [Activity Diagram – Mượn sách] 
7. [Activity Diagram – Trả sách]  
8. [Cấu trúc thư mục]
9. [Mô tả đối tượng]  
10. [Ví dụ sử dụng] 
11. [Hướng phát triển] 
12. [Bản quyền]
Cài đặt--Chạy


## ✨ Giới thiệu

Ứng dụng **Quản lý Thư viện** được xây dựng theo phong cách **Lập trình Hướng đối tượng (OOP)**, giúp bạn:

- Quản lý sách (`Book`)  
- Quản lý bạn đọc (`Reader`)  
- Theo dõi lịch sử mượn/trả (`Loan`)

---

## 👥 Thành viên

| Họ tên               | MSSV      | GitHub                        |
|----------------------|-----------|-------------------------------|
| Phạm Năng Khang      | 24100032  | [@phamkheng](https://github.com/phamkheng) |
| Trần Quốc Việt Hùng  | 24100015  | [@hungspec](https://github.com/hungspec)   |
| Phạm Việt Khoa       | 24100058  | [@pvkhoa](https://github.com/pvkhoa)       |

---

## 🌐 Ứng dụng

- Thêm / sửa / xóa sách và bạn đọc  
- Cho mượn / trả sách, xem lịch sử giao dịch  
- Kiểm tra trạng thái sách (Available / Unavailable)

---

## 📆 Yêu cầu

- Java 11 hoặc cao hơn  
- Maven hoặc IDE Java (IntelliJ IDEA, Eclipse…)

---

## 📊 Class Diagram 
![Class Diagram ](../main/images/class-diagram.png)

## 📊 Activity Diagram – Mượn sách
![Activity Diagram Mượn sách](../main/images/muonsach.png)
## 📊 Activity Diagram – Trả sách  
![Activity Diagram ](../main/images/trasach.png)
## 📊 Activity Diagram – tìm sách  
![Activity Diagram ](../main/images/timsach.png)
## 📊 Activity Diagram – đăng ký bạn đọc mới
![Activity Diagram ](../main/images/dangkybandocmoi.png)
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

🚀 Hướng phát triển
Thêm giao diện đồ họa (GUI)

Kết nối cơ sở dữ liệu (JDBC / MySQL / SQLite)

Tích hợp RESTful API (Spring Boot)

## ⚙️ Cài đặt & Chạy

```bash
git clone https://github.com/phamkheng/OOP_N02_T3_2_2025_Group1.git
cd OOP_N02_T3_2_2025_Group1
# Mở project bằng IDE hoặc:
# javac src/*.java
# java Main











