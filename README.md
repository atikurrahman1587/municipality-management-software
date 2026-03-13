# Smart Municipal Management System

![Laravel](https://img.shields.io/badge/Laravel-10.x-red)
![PHP](https://img.shields.io/badge/PHP-8.x-blue)
![MySQL](https://img.shields.io/badge/Database-MySQL-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Production-success)

A **Smart Municipal Management System** designed to digitize municipal services and create a **fully online and cashless municipality platform**.

This system allows citizens to access municipal services remotely through a **Citizen Portal**, while municipal authorities manage operations through a **centralized Admin Dashboard**.

The platform integrates **bKash, Nagad, and EkPay payment gateways** and provides **SMS notifications** for real-time service updates.

---

# 🌐 Live Projects

### Municipality Websites

- https://baraigrampaurashava.com  
- https://gurudaspurpaurashava.com  
- https://bonparapaurashava.com
- https://kazipurpourashova.com

---

# 🚀 Features

## 👨‍💻 Citizen Portal

Citizens can access municipal services online:

- Apply for certificates online
- Track application status
- Submit documents digitally
- Pay municipal fees online
- Receive SMS notifications
- Download approved certificates

---

## 🏛 Municipal Services

The system supports multiple municipal services including:

- Citizenship Certificate
- Family Certificate
- Inheritance Certificate
- Character Certificate
- Death Certificate
- Trade License
- Disability Certificate
- Landless Certificate
- Holding Tax
- Water Bill

---

## 💰 Cashless Payment System

Integrated digital payment gateways:

- **bKash**
- **Nagad**
- **EkPay**

This allows citizens to pay municipal fees securely online.

---

## 📊 Admin Dashboard

The Admin Dashboard provides full system management:

- Citizen Management
- Certificate Application Management
- Trade License Management
- Holding Tax Management
- Water Bill Management
- Financial & Revenue Tracking
- Notice & Announcement System
- Reports & Analytics Dashboard

---

## 📩 SMS Notification System

Automated SMS notifications are sent for:

- Application submission
- Payment confirmation
- Service approval or rejection
- Important municipal announcements

---

## ⚙ Background Processing

The system uses **Laravel Queue & Scheduler** for:

- SMS processing
- Payment verification
- Scheduled tasks
- System maintenance jobs
- Automated reports

---

## Author

Atikur Rahman  
Laravel Developer

GitHub: https://github.com/atikurrahman1587

---

# 🏗 System Architecture

```mermaid
graph TD

Citizen -->|Apply Service| Portal
Portal --> LaravelApp
LaravelApp --> MySQL

Citizen -->|Online Payment| PaymentGateway
PaymentGateway --> LaravelApp

LaravelApp --> SMSGateway
LaravelApp --> QueueSystem
QueueSystem --> BackgroundJobs

Admin --> AdminDashboard
AdminDashboard --> LaravelApp

