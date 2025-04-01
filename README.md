# Hotel-Reservatoin-System
A simple Java-based hotel reservation management system using MySQL. This application allows users to reserve rooms, view reservations, retrieve room numbers, update, and delete reservations.

Features:
1.Reserve a room
2.View all reservations
3.Retrieve room number based on reservation ID
4.Update an existing reservation
5.Delete a reservation

Technologies Used:
1.Java
2.MySQL
3.JDBC

Database Setup
Create a MySQL database named hoteldb.
Create a reservations table using the following SQL query:

sql
Copy
Edit
CREATE TABLE reservations (
    res_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(255) NOT NULL,
    room_number INT NOT NULL,
    contact_number VARCHAR(20) NOT NULL,
    res_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
Update database credentials in the HotelReservationSystem.java file:

java
Copy
Edit
private static final String url = "jdbc:mysql://localhost:3306/hoteldb";
private static final String username = "root";
private static final String password = "your_password";
How to Run
Clone the repository:


Copy
Edit
git clone https://github.com/yourusername/hotel-reservation-system.git
Navigate to the project directory:


Copy
Edit
cd hotel-reservation-system
Compile and run the Java program:


Copy
Edit
javac HotelReservationSystem.java
java HotelReservationSystem
Usage
Select an option from the menu to interact with the reservation system.

Follow the prompts to enter details for reservation, update, or delete operations.

License
This project is open-source and available under the MIT License.
