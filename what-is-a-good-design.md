# System Design Requirements

## 1. Moving Data → Delivering Ingredients and Orders
- Moving data is like how a restaurant moves **ingredients** and **orders**.  
- **Local data movement** → Kitchen staff moving ingredients from the fridge to the stove.  
- **Distributed data movement** → Shipping ingredients between different restaurant branches.  
- **Waiters (clients)** take orders from customers and deliver them to the **kitchen (servers)**.  
- **Delivery services** → External APIs or services transferring data.


## 2. Storing Data → Pantry, Freezers, and Warehouses
- Restaurants store ingredients in different ways:
  - **Fridge/Freezer** → Fast but limited storage (**RAM**).  
  - **Pantry** → Bulk storage in the kitchen (**Disk storage**).  
  - **Warehouse** → External bulk storage (**Cloud databases/blob storage**).  
- Choosing storage depends on how quickly items are needed, just like choosing the right database.


## 3. Transforming Data → Cooking the Meal
- Data transformation is like **cooking**:
  - Simple orders → Minimal transformation (e.g., making coffee).  
  - Complex orders → Multi-step processing (e.g., a 5-course meal).  
  - **Special requests** → Filtering data (e.g., gluten-free or vegan dishes).


# What is a Good Design?

## 4. Good Design → A Well-Run Restaurant
- A well-designed system is like a **smoothly operating restaurant**:
  - **Efficient kitchen layout** → Optimized system architecture.  
  - **Reliable suppliers** → Stable data sources.  
  - **Well-trained staff** → Scalable and resilient systems.


## 5. Availability → Restaurant Opening Hours
- **Availability** = When the restaurant is open for business.
  - Small café → Open **9 AM - 5 PM** (limited availability).  
  - Fast-food chain → Open **24/7** (high availability).  
- **Planned downtime** → Closing for cleaning or renovations.  
- **Unplanned downtime** → Closing unexpectedly due to power outages.  
- **99.999% availability** → Only **5 minutes** of downtime per year.


## 6. Reliability, Fault Tolerance, and Redundancy → Backup Kitchens and Staff
- **Reliability** → The kitchen consistently delivers correct orders.  
- **Fault Tolerance** → If the **head chef** is sick, a **backup chef** steps in.  
- **Redundancy** → Having extra stoves or staff as backups.
  - **Active-Passive** → Backup chef waits to be called in.  
  - **Active-Active** → Both chefs cook together, sharing the workload.


## 7. Throughput → Orders Served per Hour
- **Throughput** = Number of dishes served per hour.  
- To increase throughput:  
  - **Vertical scaling** → Hire faster chefs, get bigger ovens.  
  - **Horizontal scaling** → Open more kitchen stations or branches.

<img width="519" alt="Screenshot 2025-01-10 at 21 32 58" src="https://github.com/user-attachments/assets/b42dc6fb-262e-4e4e-9eb0-53b380473888" />


## 8. Latency → Order Preparation Time
- **Latency** = Time between placing an order and receiving the meal.  
- High latency → Slow service, long wait times.  
- Ways to reduce latency:  
  - **Prepping ingredients early** → Similar to caching.  
  - **Optimized workflows** → Faster order processing.
