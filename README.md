# Simple Parking Lot Management System

This project is a simple parking lot management application that allows you to park and unpark vehicles, track available slots, and generate parking tickets.

## Features

- Manage a parking lot with multiple floors and slots.
- Each slot is designated for a specific vehicle type: **car**, **bike**, or **truck**.
- Assign slots to vehicles based on availability and floor order (lowest floor, earliest slot).
- Generate tickets in the format `PARKINGLOTID_FLOOR_SLOT` (e.g., `PR123_2_5`).
- Unpark vehicles using a valid ticket.
- Display the number of available slots per vehicle type.
- List available and occupied slots for a specific vehicle type.

## Parking Lot Structure

- **Parking Lot ID**: Unique identifier for the parking lot.
- **Number of Floors**: Total floors in the parking lot.
- **Slots per Floor**: Number of slots on each floor.
- **Slot Assignment**:
    - First slot on each floor → Truck
    - Next two slots → Bikes
    - Remaining slots → Cars

## Vehicle Details

When parking a vehicle, the following details are recorded:

- Vehicle type (car, bike, truck)
- Registration number
- Color
- Optional: Vehicle name, driver’s name, etc.

## Parking Strategy

- Vehicles are parked on the **lowest available floor** and the **earliest available slot**.
- The app generates a **ticket** upon parking.

## Unparking

- Users must present a **valid ticket** to unpark the vehicle.
- The vehicle is removed from the slot, and the slot becomes available.

## Usage

1. Initialize the parking lot with a given ID, number of floors, and slots per floor.
2. Park vehicles by providing required vehicle details.
3. Unpark vehicles using the generated ticket.
4. Query for available or occupied slots by vehicle type.

## Example Ticket

This ticket represents a vehicle parked in **floor 2, slot 5** of parking lot `PR123`.

## Future Improvements

- Add support for reservation of slots.
- Track parking duration and generate billing.
- Add user authentication for drivers.
- Extend vehicle types as needed.

This is a simple Java command-line application for a parking lot system.
