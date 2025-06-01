🅿️ Parking Lot System – Machine Coding Round
❓ Problem Statement:
Design and implement a Parking Lot Service that manages parking slots for vehicles. The system should support basic operations like parking a vehicle, un-parking it, and querying current status. The design should be modular, extensible, and testable.

📘 Functional Requirements:
Create Parking Lot:

Create a parking lot with a given number of slots.

Park Vehicle:

Park a vehicle (car, bike, truck) in the nearest available slot.

If the parking lot is full, return an appropriate message.

Unpark Vehicle:

Remove a vehicle from a given slot.

Display Status:

Show slot number, vehicle number, and vehicle type for all parked vehicles.

Search Vehicles:

Search for vehicles by type (e.g., all cars).

Search for vehicle by registration number.

🛠️ Constraints & Considerations:
Each vehicle has: registration_number, color, and type (CAR, BIKE, TRUCK).

Slots are filled in the order from 1 to N (lowest available).

Slot assignment is first-come-first-serve.

Design should be scalable and open to extension (e.g., support valet slots, reserved parking, etc.).

Console-based I/O or API-based interface — your choice.

Bonus if you handle concurrency (optional).