# Parking Lot System

## Overview
This project implements a **Parking Lot Service** that manages parking slots for vehicles. The system supports basic operations such as creating a parking lot, parking vehicles, unparking vehicles, querying the current status, and searching for vehicles by type or registration number.

The design is modular, extensible, and testable, providing a foundation for future features like valet parking and reserved slots.

---

## Functional Requirements

### 1. Create Parking Lot
- Initialize a parking lot with a specified number of parking slots.
- Slots are numbered from 1 to N.

### 2. Park Vehicle
- Park a vehicle (types supported: **CAR**, **BIKE**, **TRUCK**) in the nearest available slot (lowest slot number).
- If the parking lot is full, return an appropriate message indicating no slots available.

### 3. Unpark Vehicle
- Remove a vehicle from a given slot number, making the slot available for future parking.

### 4. Display Status
- Show the parking lot status with:
  - Slot number
  - Vehicle registration number
  - Vehicle type

### 5. Search Vehicles
- Search and list all vehicles of a specific type (e.g., all cars).
- Search for a vehicle by its registration number and display its slot and details.

---

## Vehicle Attributes
Each vehicle has the following properties:
- **registration_number**: Unique vehicle registration ID
- **color**: Vehicle color
- **type**: Vehicle type — one of **CAR**, **BIKE**, **TRUCK**

---

## Constraints & Considerations
- Slots are allocated on a **first-come-first-serve** basis, filling the lowest available slot number first.
- The design should be **scalable** and **open to extension**, allowing easy addition of features like valet parking and reserved parking.
- Bonus: Handle concurrency to allow multiple park/unpark requests safely (optional).
