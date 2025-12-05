# Smart Greenhouse – IoT Monitoring System
### Group Members: **Aaron Paul & Eunice Shaji**

This project is a Smart Greenhouse Monitoring System built using **.NET MAUI**, **SQLite**, and **IoT sensor data simulation**.  
The application displays real-time temperature, humidity, and soil moisture values, and allows the user to control greenhouse devices such as the **fan** and **water pump**.

---

## 📌 Features

- Real-time dashboard for:
  - Temperature  
  - Humidity  
  - Soil Moisture  
- Device control:
  - Fan ON/OFF  
  - Pump ON/OFF  
- Local SQLite database for:
  - Saving sensor readings  
  - Storing device settings  
  - Viewing history  
- Login page (simple authentication)
- Clean UI with multiple pages:
  - Login Page  
  - Dashboard Page  
  - Control Page  
  - History Page  
  - QR Page  

---

## 🛠 Technologies Used

- **C# / .NET MAUI**
- **SQLite Database**
- **XAML UI**
- **MVVM Pattern (simplified)**
- **Async data handling**
- **Simulated IoT sensor values**


## 📂 Project Structure


🏗️ Project Architecture
SmartGreenHouse/
│
├── Models/
│ ├── SensorReading.cs
│ └── DeviceSettings.cs
│
├── Services/
│ ├── DatabaseService.cs
│ └── AuthService.cs
│
├── Pages/
│ ├── LoginPage.xaml
│ ├── DashboardPage.xaml
│ ├── ControlPage.xaml
│ ├── HistoryPage.xaml
│ └── QRPage.xaml
│
├── App.xaml
├── App.xaml.cs
└── MauiProgram.cs

🧩 Features
✓ Real-Time Sensor Simulation

Generates Temperature, Humidity, and Soil Moisture values every 3 seconds

Auto-updates dashboard UI

Saves all readings to SQLite

✓ Device Control

Toggle and save:

Fan

Pump

✓ Login System

Default credentials:

Username: admin
Password: password

✓ QR Scanner

Integrated QR code scanner page for future expansion.

✓ SQLite-Based Data Persistence

Saves sensor readings

Saves fan/pump states

✓ Navigation Shell

Smooth page transitions using .NET MAUI Shell.

🔧 Technologies Used
Technology	Purpose
.NET MAUI	Cross-platform UI
SQLite-net PCL	Embedded database
C#	Application logic
XAML	UI page layout
ZXing / MAUI Essentials	QR Scanner
MVVM (Partial)	App structure
📦 Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/yourusername/SmartGreenHouse.git

2️⃣ Install MAUI Workload
dotnet workload install maui

3️⃣ Restore Dependencies
dotnet restore

4️⃣ Run Project

Open with Visual Studio → Run on:

Android Emulator

Windows Machine

Physical Android device

🗄️ Database Structure
SensorReading Table
Field	Type
Temperature	float
Humidity	float
SoilMoisture	float
Timestamp	DateTime
DeviceSettings Table
Field	Type
FanOn	bool
PumpOn	bool

Database auto-creates at:

/AppData/Local/smartgreen.db3

🔐 Login

To access the app use:

Username: admin
Password: greenhouse123

🧪 Future Enhancements

MQTT IoT device integration

Real sensor hardware support

Cloud synchronization (Azure / Firebase)

AI plant health prediction

Push notifications for alerts

📝 License

This project is for academic use.
Feel free to extend or modify.

👩‍💻 Author

Eunice Bethesda Shaji
Computer Programming – IoT
Cambrian College
