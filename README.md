# Tour Management System

This is a simple C++ console-based application for managing tours. The system allows users to perform the following operations:

- Add new tours with destination, duration, and price.
- Remove tours by destination, duration, and price.
- Display all available tours sorted by price.

## Features

- **Add Tour**: Allows users to add a new tour with details such as destination, duration (in days), and price.
- **Remove Tour**: Allows users to remove a tour by providing its destination, duration, and price.
- **Display Tours**: Displays all available tours sorted by price in ascending order.
- **Exit**: Exits the application.

## Class Design

### 1. `Tour` Class
The `Tour` class represents a single tour's details. It includes attributes like:
- `destination`: The destination of the tour.
- `duration`: The duration of the tour in days.
- `price`: The price of the tour.
- `next`: A pointer to the next `Tour` object in the linked list.

### 2. `TourList` Class
The `TourList` class manages a linked list of `Tour` objects. It provides the following functions:
- `addTour()`: Adds a new tour to the list.
- `removeTour()`: Removes a specific tour from the list.
- `displayTours()`: Displays all tours, sorted by price.

### 3. `TourManager` Class
The `TourManager` class acts as an interface between the user and the `TourList` class. It includes:
- `addTour()`: Adds a tour using the `TourList` class.
- `removeTour()`: Removes a tour using the `TourList` class.
- `displayTours()`: Displays tours using the `TourList` class.

## Usage

### 1. Add Tour
- Users can add a tour by specifying the destination, duration (in days), and price.
  
### 2. Remove Tour
- Users can remove a tour by specifying the destination, duration (in days), and price.

### 3. Display Tours
- Displays a list of all tours sorted by price in ascending order.

### 4. Exit
- Exits the application.

## Example Interaction

```plaintext
Menu:
1. Add Tour
2. Remove Tour
3. Display Tours
4. Exit
Enter your choice: 1

Enter destination: Paris
Enter duration (in days): 7
Enter price: /-5000
Tour added.

Menu:
1. Add Tour
2. Remove Tour
3. Display Tours
4. Exit
Enter your choice: 3

Available Tours (Sorted by Price):
Destination: Paris
Duration: 7 days
Price: /-5000
----------------------
