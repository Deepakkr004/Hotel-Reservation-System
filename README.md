# 🏨 Hotel Reservation System  

A simple **Java console-based hotel management system** built using **JDBC and MySQL**.  
Designed for hotel receptionists to manage guest reservations efficiently with full **CRUD functionality** (Create, Read, Update, Delete).  

---

## 🚀 Features  
- ✅ **Reserve a Room** – Add new reservations with guest details  
- ✅ **View Reservations** – Display all reservations in a clean tabular format  
- ✅ **Get Room Number** – Retrieve a guest’s room number using reservation ID & name  
- ✅ **Update Reservation** – Modify guest details, room number, or contact info  
- ✅ **Delete Reservation** – Cancel reservations by ID  
- ✅ **Exit System** – Graceful exit with countdown  

---

## 🛠️ Tech Stack  
- **Language:** Java  
- **Database:** MySQL  
- **Libraries/Tools:** JDBC, Scanner, SQL  
- **IDE:** IntelliJ IDEA  

---

## 📂 Project Structure  
Hotel-Reservation-System/
│── src/
│ └── Main.java # Main program file
│── .gitignore # Ignore IDE & build files
│── README.md # Project documentation


---

## 🗄️ Database Schema  
Table: **reservations**  
```sql
CREATE TABLE reservations (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(100) NOT NULL,
    room_number INT NOT NULL,
    contact_number VARCHAR(15) NOT NULL,
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);


▶️ How to Run
Clone the repository:

git clone https://github.com/your-username/Hotel-Reservation-System.git
Open project in IntelliJ IDEA (or any Java IDE).

Update database credentials in Main.java:

private static final String url = "jdbc:mysql://localhost:3306/hotel_db";
private static final String username = "root";
private static final String password = "your_password";


Run the program.
Use the console menu to manage hotel reservations 🎉.

📸 Sample Console Output

HOTEL MANAGEMENT SYSTEM
1. Reserve a room
2. View Reservations
3. Get Room Number
4. Update Reservations
5. Delete Reservations
0. Exit
Choose an option:

🌟 Future Improvements
Web-based front-end using Spring Boot or Flask

Authentication for staff login

Payment & billing module

Room availability tracking

👨‍💻 Author
Developed by Deepak Kumar

