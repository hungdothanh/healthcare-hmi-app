# Healthcare HMI App

This repository contains a Human-Machine Interface (HMI) healthcare application prototype created using **Axure RP**. The application allows doctors and patients to interact through a simulated interface for managing health data, viewing prescriptions, and connecting with medical professionals.

# Table of Contents
- [Introduction](#introduction)
- [Key Features](#key-features)
- [Design Diagrams](#design-diagrams)
- [Use Case Scenarios](#use-case-scenarios)
- [Activity Diagram](#activity-diagram)
- [State Diagrams](#state-diagrams)
- [Design Considerations](#design-considerations)
- [Testing Considerations](#testing-considerations)
- [Demo](#demo)

## Introduction
This project demonstrates a functional prototype for a healthcare app that showcases interactions between doctors and patients. It incorporates login/logout functionality, doctor search, connection management, viewing health information, and managing prescriptions.

## Key Features
- **Doctor-Patient Connection**: Allows patients to search and connect with available doctors.
- **Prescription Management**: Doctors can create and view prescriptions, while patients can view prescriptions issued to them.
- **Health Status Monitoring**: Doctors can view a patient's current health status metrics (heartbeat, SpO2).
- **Profile Management**: Both patients and doctors can view and manage their profile information.

## Design Diagrams
### Use Case Diagram
The use case diagram describes the various interactions between the user roles (Doctor, Patient) and the system. It outlines key functionalities like login, viewing profiles, connecting with doctors, and managing prescriptions.

![Use Case Diagram](diagrams/use_case_diagram.png)

---

### State Diagrams
The following state diagrams represent system behavior for different user roles.

#### State Diagram for Patient
The patient’s state diagram illustrates transitions between states like login, menu navigation, doctor search, and viewing prescriptions.

![State Diagram - Patient](diagrams/state_diagram_patient.png)

#### State Diagram for Doctor
The doctor’s state diagram shows state transitions for actions like viewing patients, creating prescriptions, and logging out.

![State Diagram - Doctor](diagrams/state_diagram_doctor.png)

---

### Activity Diagram
The activity diagram describes the sequence of actions performed by users during typical usage of the app, starting from logging in to viewing prescriptions or managing connected doctors.

![Activity Diagram](diagrams/activity_diagram.png)

---

### Testing Considerations
The test diagram describes various test scenarios implemented to ensure the app works as intended. These include login validation, prescription management, and data fetching tests.

![Test Diagram](diagrams/test_diagram.png)

---

### Demo
A demo video showcasing the healthcare app functionality:
- **[Watch Demo](demo/healthcare_app_demo.mp4)**

---

## Design Considerations
The design of this healthcare app was guided by key considerations to optimize usability and functionality. Refer to [design_considerations.md](design_considerations.md) for detailed explanations of:
- Interface Design Elements
- Input and Output Expectations
- Mockup Implementations for Core Use Cases

---

## Use Case Scenarios and Implementations
| Use Case ID | Description | Implementation | Interface Components |
|-------------|-------------|----------------|---------------------|
| UC-01       | Login to Account | Allows user to input email and password. Checks for validity. | Text fields, login button |
| UC-02       | Logout of Account | Provides a logout option for both user roles. | Logout button |
| UC-03       | View Profile | Users can view their profile information. | Profile sub-menu |
| UC-04       | Search Doctor | Patients can search and filter doctors by symptom. | Search field, filter function |
| UC-05       | Connect Doctor | Patients select and connect to doctors. | Checkboxes, icons, global variables |
| UC-06       | Disconnect Doctor | Patients can disconnect from doctors. | Toggle icons, global variables |
| UC-07       | View Prescriptions | Patients view a list of prescriptions. | Repeater, server request |

---

## Mockup and Feasibility
Functionality in mock-ups was designed using Axure RP features like filters, global variables, and repeaters. The feasibility and real-world implementation were considered when creating components for managing doctor connections, health metrics, and prescription handling.
