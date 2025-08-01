# Hospital Management System

A comprehensive Flutter application for managing hospital operations including patient management, doctor scheduling, appointment booking, and room management.

## Features

### 🏥 Core Modules
- **Patient Management**: Register, view, edit, and manage patient records
- **Doctor Management**: Manage doctor profiles, specializations, and availability
- **Appointment Scheduling**: Book, reschedule, and track appointments
- **Room Management**: Monitor bed availability and room status
- **Dashboard Analytics**: Overview of hospital statistics and recent activities

### 📊 Key Features
- **Modern UI/UX**: Clean, intuitive interface with Material Design 3
- **Local Database**: SQLite database for persistent data storage
- **State Management**: Provider pattern for efficient state management
- **Responsive Design**: Works across different screen sizes
- **Sample Data**: Pre-populated with sample data for demonstration

### 🎯 Functionality
- **Patient Records**: Complete patient information including medical history, allergies, and medications
- **Doctor Profiles**: Detailed doctor information with specializations and availability status
- **Appointment System**: Comprehensive appointment management with status tracking
- **Room Monitoring**: Real-time room and bed availability tracking
- **Search & Filter**: Easy navigation and data filtering capabilities

## Screenshots

The application includes the following main screens:
- **Dashboard**: Overview with statistics and quick actions
- **Patients**: List and manage patient records
- **Doctors**: View and manage doctor profiles
- **Appointments**: Schedule and track appointments
- **Rooms**: Monitor room and bed availability

## Getting Started

### Prerequisites
- Flutter SDK (3.8.1 or higher)
- Dart SDK
- Android Studio / VS Code
- Android Emulator or Physical Device

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd flutter_application_1
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the application**
   ```bash
   flutter run
   ```

### Project Structure

```
lib/
├── models/           # Data models
│   ├── patient.dart
│   ├── doctor.dart
│   ├── appointment.dart
│   └── room.dart
├── screens/          # UI screens
│   ├── dashboard_screen.dart
│   ├── patients_screen.dart
│   ├── doctors_screen.dart
│   ├── appointments_screen.dart
│   └── rooms_screen.dart
├── widgets/          # Reusable widgets
│   ├── dashboard_card.dart
│   └── stats_card.dart
├── providers/        # State management
│   └── hospital_provider.dart
├── services/         # Business logic
│   ├── database_service.dart
│   └── sample_data_service.dart
├── utils/            # Utilities
│   └── helpers.dart
└── main.dart         # App entry point
```

## Dependencies

The application uses the following key dependencies:

- **provider**: State management
- **sqflite**: Local database
- **path**: File path utilities
- **uuid**: Unique ID generation
- **intl**: Internationalization
- **fl_chart**: Charts and graphs
- **table_calendar**: Calendar widget
- **go_router**: Navigation

## Database Schema

### Patients Table
- id, name, email, phone, address
- dateOfBirth, gender, bloodGroup
- emergencyContact, emergencyPhone
- registrationDate, medicalHistory, allergies, currentMedications

### Doctors Table
- id, name, email, phone, specialization, department
- licenseNumber, dateOfBirth, gender, address
- joiningDate, qualification, experience, bio, isAvailable

### Appointments Table
- id, patientId, doctorId, appointmentDate, timeSlot
- status, type, notes, symptoms, diagnosis, prescription, fee, createdAt

### Rooms Table
- id, roomNumber, type, floor, capacity, occupiedBeds
- pricePerDay, status, description

## Usage

### Adding Patients
1. Navigate to the Patients screen
2. Tap the "+" button to add a new patient
3. Fill in the required information
4. Save the patient record

### Managing Doctors
1. Go to the Doctors screen
2. View doctor profiles and availability
3. Add new doctors or edit existing ones
4. Update availability status

### Scheduling Appointments
1. Access the Appointments screen
2. Select patient and doctor
3. Choose date and time slot
4. Add appointment details and save

### Room Management
1. Visit the Rooms screen
2. Monitor bed availability
3. Update room status
4. Track occupancy rates

## Features in Detail

### Dashboard
- **Statistics Cards**: Real-time counts of patients, doctors, appointments, and rooms
- **Quick Actions**: Easy access to common tasks
- **Recent Activity**: Latest updates and notifications
- **Navigation**: Seamless navigation to all modules

### Patient Management
- **Complete Records**: Comprehensive patient information
- **Medical History**: Track patient medical background
- **Allergies & Medications**: Important health information
- **Emergency Contacts**: Quick access to emergency information

### Doctor Management
- **Professional Profiles**: Detailed doctor information
- **Specializations**: Track medical specializations
- **Availability Status**: Real-time availability updates
- **Experience & Qualifications**: Professional credentials

### Appointment System
- **Scheduling**: Easy appointment booking
- **Status Tracking**: Monitor appointment status
- **Patient-Doctor Linking**: Connect patients with doctors
- **Medical Notes**: Detailed appointment records

### Room Management
- **Bed Availability**: Real-time bed tracking
- **Room Types**: Different room categories (General, Private, ICU, Emergency)
- **Pricing**: Room cost management
- **Occupancy Monitoring**: Track room utilization

## Future Enhancements

- **User Authentication**: Secure login system
- **Role-based Access**: Different access levels for staff
- **Billing System**: Integrated billing and payment
- **Lab Reports**: Laboratory test management
- **Pharmacy Module**: Medication and inventory management
- **Reports & Analytics**: Advanced reporting features
- **Notifications**: Push notifications for appointments
- **Multi-language Support**: Internationalization
- **Cloud Sync**: Data synchronization across devices

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support and questions, please open an issue in the repository.

---

**Note**: This is a demonstration application with sample data. For production use, additional security measures, data validation, and proper error handling should be implemented.
