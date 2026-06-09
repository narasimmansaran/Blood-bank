# Blood Bank Management System

## Project Overview

The Blood Bank Management System is a web-based application designed to automate and manage blood bank operations efficiently. The system maintains donor information, blood inventory, recipient requests, blood issuance records, and staff management. It helps reduce manual paperwork, improve data accuracy, and ensure the timely availability of blood units during emergencies.

---

## Problem Statement

### Main Objective

To develop an automated Blood Bank Management System that efficiently manages blood donation, blood storage, blood requests, and blood distribution while maintaining accurate records and improving operational efficiency.

### Specific Objectives

* Maintain donor information and donation history.
* Manage blood inventory and stock availability.
* Process blood requests from recipients and hospitals.
* Track blood collection and blood issuance.
* Monitor blood unit expiration dates.
* Generate reports for administrative purposes.
* Reduce manual errors and paperwork.
* Improve emergency blood management services.

---

## Proposed Solution

The proposed system provides a centralized platform for managing all blood bank activities digitally. It allows donors, recipients, staff, and administrators to perform their respective operations through a secure and user-friendly interface.

The system includes:

* Donor Management
* Blood Collection Management
* Blood Inventory Management
* Recipient Management
* Blood Request Processing
* Blood Issue Management
* Staff Management
* Report Generation
* User Authentication and Authorization

---

## Features

### Donor Module

* Register donor
* Update donor details
* View donation history
* Search donor information

### Blood Collection Module

* Record blood donations
* Store blood unit details
* Track collection dates

### Blood Inventory Module

* Manage blood stock
* Check blood availability
* Monitor expiry dates
* Update inventory status

### Recipient Module

* Register recipient
* Manage recipient details
* Search recipient records

### Blood Request Module

* Create blood requests
* Approve or reject requests
* Track request status

### Blood Issue Module

* Issue blood units
* Update inventory automatically
* Maintain issue history

### Staff Module

* Add staff
* Update staff information
* Assign roles and responsibilities

### Report Module

* Donor reports
* Blood stock reports
* Request reports
* Blood issue reports
* Expired blood reports

---

## System Modules

* Authentication Module
* Donor Management Module
* Blood Collection Module
* Blood Inventory Module
* Recipient Management Module
* Blood Request Module
* Blood Issue Module
* Staff Management Module
* Report Management Module

---

## Database Tables

### donor

| Field Name         | Description        |
| ------------------ | ------------------ |
| donor_id           | Primary Key        |
| donor_name         | Donor Name         |
| gender             | Gender             |
| blood_group        | Blood Group        |
| phone              | Contact Number     |
| email              | Email Address      |
| address            | Address            |
| last_donation_date | Last Donation Date |

### blood_bank

| Field Name | Description     |
| ---------- | --------------- |
| bank_id    | Primary Key     |
| bank_name  | Blood Bank Name |
| location   | Location        |
| contact_no | Contact Number  |
| email      | Email Address   |

### blood_unit

| Field Name      | Description                    |
| --------------- | ------------------------------ |
| blood_unit_id   | Primary Key                    |
| donor_id        | Foreign Key                    |
| bank_id         | Foreign Key                    |
| blood_group     | Blood Group                    |
| quantity        | Quantity                       |
| collection_date | Collection Date                |
| expiry_date     | Expiry Date                    |
| status          | Available / Issued / Discarded |

### recipient

| Field Name     | Description    |
| -------------- | -------------- |
| recipient_id   | Primary Key    |
| recipient_name | Recipient Name |
| blood_group    | Blood Group    |
| phone          | Contact Number |
| address        | Address        |
| hospital_name  | Hospital Name  |

### blood_request

| Field Name        | Description                               |
| ----------------- | ----------------------------------------- |
| request_id        | Primary Key                               |
| recipient_id      | Foreign Key                               |
| blood_group       | Blood Group                               |
| quantity_required | Quantity Required                         |
| request_date      | Request Date                              |
| status            | Pending / Approved / Rejected / Completed |

### blood_issue

| Field Name      | Description     |
| --------------- | --------------- |
| issue_id        | Primary Key     |
| request_id      | Foreign Key     |
| blood_unit_id   | Foreign Key     |
| issue_date      | Issue Date      |
| quantity_issued | Quantity Issued |

### staff

| Field Name | Description    |
| ---------- | -------------- |
| staff_id   | Primary Key    |
| bank_id    | Foreign Key    |
| staff_name | Staff Name     |
| role       | Staff Role     |
| phone      | Contact Number |
| email      | Email Address  |

### users

| Field Name | Description           |
| ---------- | --------------------- |
| user_id    | Primary Key           |
| username   | Login Username        |
| password   | Encrypted Password    |
| role       | Admin / Staff / Donor |

---

## ER Diagram

Place your ER Diagram image inside the `docs` folder.

```text
docs/
└── ER_Diagram.png
```

---

## Use Case Diagram

Place your Use Case Diagram image inside the `docs` folder.

```text
docs/
└── UseCase_Diagram.png
```

---

## Hardware Requirements

### Minimum Requirements

* Intel Core i3 Processor
* 4 GB RAM
* 250 GB Hard Disk
* Keyboard and Mouse
* Monitor

### Recommended Requirements

* Intel Core i5 or Higher
* 8 GB RAM
* SSD Storage
* Stable Internet Connection

---

## Software Requirements

### Frontend

* HTML5
* CSS3
* JavaScript
* Bootstrap

### Backend

* PHP / Python Django / Node.js

### Database

* MySQL

### Development Tools

* Visual Studio Code
* XAMPP
* Git
* GitHub

---

## System Workflow

### Donor Workflow

Donor Registration

↓

Login

↓

Blood Donation

↓

Blood Collection

↓

Inventory Update

---

### Recipient Workflow

Recipient Registration

↓

Search Blood Availability

↓

Submit Request

↓

Request Verification

↓

Blood Approval

↓

Blood Issue

---

### Staff Workflow

Login

↓

Manage Donors

↓

Manage Inventory

↓

Process Requests

↓

Issue Blood

↓

Generate Reports

---

### Admin Workflow

Login

↓

Manage Staff

↓

Manage Settings

↓

View Logs

↓

Generate Reports

---

## Project Structure

```text
Blood-Bank-Management-System/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── docs/
│   ├── ER_Diagram.png
│   └── UseCase_Diagram.png
│
├── database/
│   └── blood_bank.sql
│
├── frontend/
│   ├── index.html
│   ├── login.html
│   ├── donor.html
│   ├── recipient.html
│   ├── inventory.html
│   └── reports.html
│
├── backend/
│   ├── config/
│   ├── models/
│   ├── controllers/
│   ├── routes/
│   └── middleware/
│
├── screenshots/
│
└── tests/
    └── test_cases.md
```

---

## Expected Outcomes

* Efficient blood inventory management
* Faster request processing
* Improved donor record maintenance
* Accurate blood stock monitoring
* Reduced paperwork
* Better emergency response
* Secure and centralized database management

---

## Future Enhancements

* Mobile Application Support
* SMS Notifications
* Email Notifications
* QR Code-Based Blood Tracking
* Cloud Deployment
* AI-Based Blood Demand Prediction
* Hospital Integration
* Real-Time Blood Availability Monitoring
* Biometric Authentication

---

## Conclusion

The Blood Bank Management System provides an efficient and reliable solution for managing blood donation and distribution activities. The system improves operational efficiency, ensures accurate record keeping, and helps save lives through better blood availability management.
