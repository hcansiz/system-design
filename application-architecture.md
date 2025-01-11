# Application Architecture

## 1. Developer’s Perspective → Head Chef and Kitchen Setup
Developers are like the head chefs designing recipes (writing code) and managing how the kitchen operates.
The server is the kitchen, where dishes (requests) are prepared.
Persistent storage (database) is the pantry where all ingredients (data) are stored.
If the kitchen runs out of space for storage, they use a separate warehouse (external database/cloud storage).

## 2. User’s Perspective → Restaurant Customer and Waitstaff
The user is a customer who places an order (request) via a waiter (web browser/client).
The kitchen (server) prepares the dish and serves it back to the customer through the waiter.
For simple orders, the waiter brings out ready-made items (HTML/CSS/JS).

## 3. Scaling the Restaurant (Vertical & Horizontal Scaling)
**Vertical Scaling (Upgrading Equipment):**
Adding more stoves, bigger counters, or hiring more skilled chefs in the same kitchen.
Limited by the physical space of the kitchen.

**Horizontal Scaling (Opening More Kitchens):**
Opening multiple kitchen branches to handle more customers.
Customers are directed to different branches to balance the load.

## 4. Load Balancer → Restaurant Host/Manager
The load balancer is like the restaurant host who decides where to seat customers.
If one kitchen is busy, the host sends new customers to a less crowded branch.

## 5. External Services → Food Delivery Partners and Suppliers
The restaurant may rely on external services (APIs), like:
Payment systems (Stripe) → Cash register or payment terminal.
Suppliers for fresh ingredients → Third-party APIs providing data or functionality.

## 6. Logging → Kitchen CCTV & Order Notebooks
Logging is like keeping a logbook or having security cameras in the kitchen.
It tracks every step of the cooking process, showing where mistakes happen.
Logs can be stored in a safe back office (external server) for safety.

## 7. Metrics → Kitchen Thermometers and Timers
Metrics are like thermometers, timers, and inventory trackers in the kitchen.
They monitor critical stats like stove temperature (CPU usage), number of orders (network traffic), and ingredient stock (memory usage).
This helps the head chef spot bottlenecks—like a slow chef or a broken stove.

## 8. Alerts → Fire Alarms and Kitchen Buzzers
Alerts are like fire alarms or buzzers in the kitchen.
If something goes wrong (e.g., oven overheating or food burning), an alarm notifies the chefs immediately.
Developers get notifications when performance drops below a set standard (e.g., too many failed orders).

<img width="526" alt="Screenshot 2025-01-10 at 21 09 30" src="https://github.com/user-attachments/assets/3f6751df-8fbf-447e-a3a3-3e002763674a" />


