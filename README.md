# Hardware Warehouse Management System

## 📌 Overview
The Hardware Warehouse Management System is a console application designed to manage the inventory of hardware items in a warehouse. The system allows for real-time updates and processing of items as they are added to the inventory.

## 🛠️ Technologies Used

- **C# 13.0**
- **.NET 9**


## 🚀 Features

- **Real-time Inventory Updates**: The system provides real-time updates on the inventory as items are added.
- **Batch Processing**: Items are processed in batches of a specified size.
- **Custom Queue Implementation**: The system uses a custom queue to manage the hardware items.


## 🏗️ How It Works

1. **Initialization**: The application initializes a `CustomQueue` of `HardwareItem` objects and subscribes to the `CustomQueueEvent`.
2. **Adding Items**: Hardware items (e.g., drills, ladders, hammers, paint brushes) are added to the queue with simulated delays to mimic real-world scenarios.
3. **Event Handling**: When an item is added to the queue, the `CustomQueueEvent` is triggered, which updates the console display with the current state of the queue.
4. **Batch Processing**: When the queue reaches a specified batch size (5 items), the `ProcessItems` method is called to process the items in the queue.
5. **Real-time Updates**: The console is cleared and updated in real-time to show the current items in the queue and their details.

