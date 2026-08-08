## Problem Statement

In modern airline reservation systems, thousands of flight bookings are processed every minute across different regions and time zones. Each booking contains important attributes such as passenger details, flight number, departure time, and priority level (e.g., VIP passengers, emergency bookings, or frequent flyers).

To ensure efficient operations, the system must continuously **sort flight bookings** based on:

- **Primary Key:** Departure Time  
- **Secondary Key:** Passenger Priority  

This sorting helps in proper scheduling, boarding management, and resource allocation.

However, several challenges arise in this scenario:

- **Large Data Volume:** Airline systems handle massive numbers of booking records, making sorting computationally intensive.
- **Real-Time Updates:** New bookings, cancellations, and modifications occur frequently, requiring continuous re-sorting.
- **Stability Requirement:** When two bookings have the same departure time, their relative order (based on priority) must be preserved.
- **System Performance:** The sorting algorithm must guarantee consistent performance regardless of input size.

To address these challenges, the **Merge Sort algorithm** is applied. Merge Sort follows the **Divide and Conquer strategy**, where the dataset is recursively divided into smaller sublists, sorted individually, and then merged to produce a fully sorted list.

The objective of this case study is to:

- Analyze how Merge Sort ensures **stable and efficient sorting** of airline bookings.
- Explain its working using the **Divide and Conquer approach**.
- Evaluate its **time complexity (O(n log n))** under different scenarios.
- Identify limitations such as additional memory usage.
- Design an optimized solution suitable for large-scale, real-time airline reservation systems and justify its effectiveness.
