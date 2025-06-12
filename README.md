# Cafeteria Management System (CMS)

## Project Overview
This is a Java-based Cafeteria Management System. The system automates food ordering processes, reduces fraud, and provides real-time tracking of cafeteria operations.

## Features
- User registration with role-based access (Ticketing, Server, Kitchen, IT, Head of Unit)
- Secure login authentication
- Order processing with unique order numbers
- Real-time food quantity tracking
- Role-specific dashboards
- Automated email notifications
- Reporting and analytics for management
- Webcam integration for photo capture

## Technologies Used
- **Programming Language**: Java
- **GUI Framework**: Swing
- **Database**: MySQL
- **Build Tool**: Apache Ant
- **Version Control**: Git

## Project Structure
```
CMS [main]
├── build
├── dist
├── nbproject
└── src
    └── cms
        ├── CMS.java
        ├── ChangeRole.java
        ├── HOUDashboard.java
        ├── ITdashboard.java
        ├── Icon.png
        ├── KitchenDashboard.java
        ├── Login.java
        ├── Registration.java
        ├── ResetPassword.java
        ├── ServerDashboard.java
        ├── TicketingDashboard.java
        ├── env.java
        ├── webcam.java
    └── cms.drivers
    └── test
    └──.gitignore
    └── build.xml
    └──cms.sql
    └── manifest.mf
```

## Dependencies
The project uses the following libraries (located in `cms.drivers`):
- `jakarta.activation-1.2.1.jar` (for email functionality)
- `jakarta.mail-1.6.7.jar` (for email functionality)
- `jcalendar-1.4.jar` (for date picker)
- `mysql-connector-j-8.0.31.jar` (MySQL database connectivity)
- `opencv-4110.jar` (for webcam integration)

## Installation Instructions
1. **Prerequisites**:
   - Java JDK 8 or later
   - MySQL Server
   - Apache Ant

2. **Database Setup**:
   - Run the `cms.sql` script to create the database schema

3. **Configuration**:
   - Update database credentials in `env.java`
   - Configure email settings in the appropriate classes for notification functionality

4. **Build**:
   ```bash
   ant build
   ```

5. **Run**:
   ```bash
   ant run
   ```

## Usage
1. Launch the application
2. Register users through the IT admin dashboard
3. Use role-specific dashboards for:
   - Ticketing staff: Order processing
   - Kitchen staff: Food quantity management
   - Serving staff: Order fulfillment
   - Head of Unit: Monitoring and reporting

## Contributors
- Abdul-Qoyyum Oyadeyi- Primary developer

## License
This project is licensed under the MIT License - see the LICENSE file for details.
