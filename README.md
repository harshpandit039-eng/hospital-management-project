# Smart Hospital Management System (SHMS)

## Overview

Smart Hospital Management System (SHMS) is a Python-based Hospital Management application developed using Object-Oriented Programming principles and advanced Python concepts. The project simulates real-world hospital operations and manages patients, doctors, nurses, appointments, medical records, billing, pharmacy inventory, and laboratory reports.

The system is designed to demonstrate both software engineering practices and Python programming concepts in a single integrated project.

---

## Features

### Patient Management

* Register new patients
* Update patient information
* Search patients by ID or name
* View patient history
* Track appointments and medical records

### Doctor Management

* Add doctors
* Update doctor information
* Manage consultation fees
* Maintain available appointment slots
* Sort doctors based on fees

### Nurse Management

* Add nurses
* Assign departments and shifts
* Update nurse shifts
* Group nurses by department

### Appointment Management

* Book appointments
* Cancel appointments
* Reschedule appointments
* Prevent appointment conflicts
* Track appointment status

### Pharmacy Management

* Add medicines
* Update medicine stock
* Dispense medicines
* Monitor medicine expiry dates
* Sort medicines by price

### Medical Records

* Store diagnosis details
* Add prescriptions
* Maintain treatment notes
* Retrieve patient records

### Laboratory Reports

* Generate reports
* Store test results
* View laboratory history

### Billing Management

* Generate bills
* Calculate charges automatically
* Create receipts
* Store billing records

### Report Generation

* Appointment report generation
* Billing report generation
* Lab report generation
* CSV export support

### Data Persistence

* Save data using JSON files
* Load data automatically from storage

---

## Python Concepts Used

This project demonstrates multiple advanced Python concepts:

### Object-Oriented Programming

* Abstraction
* Encapsulation
* Inheritance
* Polymorphism
* Composition

### Advanced Python Features

* Abstract Classes
* Static Methods
* Class Methods
* Magic Methods
* Decorators
* Lambda Functions
* Generators
* Recursive Functions
* List Comprehensions
* Exception Handling

### Data Structures

* Lists
* Dictionaries
* Tuples
* Sets

### File Handling

* JSON File Handling
* CSV Report Generation

### Additional Modules Used

* datetime
* functools
* json
* csv
* os
* abc

---

## Project Structure

```text
Smart-Hospital-Management-System/
│
├── SHMS PROJECT.py
│
├── data/
│   ├── patients.json
│   ├── doctors.json
│   ├── nurses.json
│   ├── appointments.json
│   ├── medicines.json
│   ├── medical_records.json
│   ├── lab_reports.json
│   └── bills.json
│
├── reports/
│   ├── appointment_report.csv
│   ├── billing_report.csv
│   └── lab_report.csv
│
└── README.md
```

---

## Classes Implemented

### Base Class

**Person**

* Abstract base class
* Parent of Patient, Doctor, and Nurse

### Derived Classes

#### Patient

Attributes:

* Patient ID
* Name
* Age
* Gender
* Phone Number
* Blood Group

#### Doctor

Attributes:

* Doctor ID
* Specialization
* Consultation Fee
* Available Slots

#### Nurse

Attributes:

* Nurse ID
* Department
* Shift

#### Appointment

Attributes:

* Appointment ID
* Patient ID
* Doctor ID
* Date
* Slot
* Status

#### Medicine

Attributes:

* Medicine ID
* Name
* Stock
* Price
* Expiry Date

#### MedicalRecord

Attributes:

* Record ID
* Diagnosis
* Prescription
* Notes

#### LabReport

Attributes:

* Report ID
* Test Name
* Result

#### Bill

Attributes:

* Bill ID
* Consultation Charges
* Medicine Charges
* Laboratory Charges
* Total Amount

#### Hospital

Central class responsible for:

* Managing all records
* Saving and loading data
* Report generation
* Statistics management

---

## Exception Handling

Custom exceptions implemented:

* InvalidPatientIDError
* InvalidDoctorIDError
* InvalidNurseIDError
* AppointmentConflictError
* InsufficientStockError
* InvalidBillAmountError
* MissingFileError
* InvalidInputError
* MedicineExpiredError
* SlotNotAvailableError

---

## Installation

### Clone Repository

```bash
git clone https://github.com/your-username/Smart-Hospital-Management-System.git
```

### Navigate to Project

```bash
cd Smart-Hospital-Management-System
```

### Run Project

```bash
python "SHMS PROJECT.py"
```

---

## Example Workflow

### Register Patient

```python
hospital.register_patient(
    "John Doe",
    24,
    "Male",
    "9876543210",
    "O+"
)
```

### Add Doctor

```python
hospital.add_doctor(
    "Dr Smith",
    45,
    "Male",
    "9876543210",
    "Cardiology",
    500
)
```

### Book Appointment

```python
hospital.book_appointment(
    "P001",
    "D001",
    "2026-07-10",
    "10:00"
)
```

### Generate Bill

```python
hospital.generate_bill(
    "P001",
    500,
    300,
    200
)
```

---

## Future Enhancements

* GUI using Tkinter or PyQt
* Database integration (MySQL/MongoDB)
* User authentication system
* Admin dashboard
* Web application version
* Online appointment booking
* Email and SMS notifications
* PDF report generation

---

## Learning Outcomes

This project helps understand:

* Practical implementation of OOP concepts
* Large-scale Python application structure
* Exception handling strategies
* File management systems
* Data persistence
* Modular coding practices
* Real-world project development

---

## Author

Harshit Shukla

Smart Hospital Management System — Python OOP Project
