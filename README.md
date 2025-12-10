A console-based Bus Ticket Booking System written in C using file handling, user authentication, seat reservation, and ticket generation.
This project demonstrates structured programming, modular design, and a simple real-world booking workflow.
🔐 Login Interface

User can sign up and log in using a simple console UI.

🚌 Main Menu
📸 Screenshots
<img width="536" height="215" alt="Screenshot 2025-12-09 222012" src="https://github.com/user-attachments/assets/9011093b-9995-43fa-a79a-55ad85544cc8" />


After login, users can:

Buy Tickets

View Booking Info

Change Password

Log Out

📸 Screenshots
<img width="581" height="434" alt="Screenshot 2025-12-10 223930" src="https://github.com/user-attachments/assets/87dfd2e8-7473-4905-9292-516f199a8948" />


🎟 Ticket Booking
User selects a date, number of seats, and seat numbers from a visual seat map.


✨ Features
👥 User Authentication

Sign‐up with username & password

Secure login with password masking

Change password anytime

Stores user info in simple text files
📸 Screenshots
<img width="698" height="270" alt="Screenshot 2025-12-10 223842" src="https://github.com/user-attachments/assets/1aaabdd3-ebc6-4e77-a132-7c84ff190669" />


🎫 Ticket Booking

Choose journey date (supports 2025–2030)

Shows available seats in a visual grid

Prevents booking already-reserved seats

Saves booking info per user

💺 Seat Management

Maintains a simple “Booked list”

Visual seat map 

Supports booking multiple seats at once
<img width="942" height="593" alt="Screenshot 2025-12-10 224154" src="https://github.com/user-attachments/assets/f6093b04-d078-47e1-9650-f8b071a4582a" />

📄 File Handling

The system uses multiple files:

users.txt → stores all user accounts

password.txt → temporary password storage

<username>_booking.txt → booking history

<username>_seat.txt → user-specific seat numbers

Date-wise global seat files

Additional utility files used internally

🧹 Additional Functionalities

Resetting seats

Printing & reviewing old bookings

Displaying user data

Logout & return to main menu


🗂 Project Structure
📁 BusTicketSystem
│
├── bus.c               # Main source code
├── users.txt           # Registered users
├── password.txt        # Password temp file
├── <seat files>        # Auto-generated per date
├── <username>_booking.txt
├── <username>_seat.txt
└── README.md


(Seat files are automatically created based on the date of journey.)

🧾 How It Works
1️⃣ Sign Up

User enters:

First Name

Last Name

Username

Password

Email

Phone Number

2️⃣ Login

Username + Password

Three failed attempts → access denied

Password masking enabled (*)

3️⃣ Book Ticket

Enter date (DD/MM/YYYY)

Enter number of seats

Choose seat numbers from the seat map

Confirm booking

System saves info into files

4️⃣ View Booking Info

Shows:

Journey date

Number of seats

Seat numbers

📦 Compilation & Run
Linux / MacOS
gcc bus.c -o bus
./bus

Windows (MinGW)
gcc bus.c -o bus.exe
bus.exe

🛠 Technologies Used

C Programming Language

File Handling (fopen, fgets, fputs, fprintf)

Console UI (ASCII Based)

Structs & Modular Programming

Date Validation

Seat Reservation Logic

🚀 Future Improvements (Optional Ideas)


🔐 Encrypted password storage

🚌 Multiple buses & routes

📱 More modern UI

📤 Export ticket as PDF

🔎 Search booking

🌐 Online database support
