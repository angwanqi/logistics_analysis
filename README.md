# Logistics Analysis
This is one of the challenges attempted in Shopee's Code League 2020. 

## Logistics Performance
The performance of these third-party logistics providers are monitored regularly and each provider is held accountable based on the Service Level Agreements (SLA). Late deliveries are flagged out and penalties are imposed on the providers to ensure they perform their utmost.

## Task
The task is to identify all the orders that are considered late depending on the Service Level Agreements (SLA) with the Logistics Provider.

## Notes
- Each orderid represents a distinct transaction. 
- SLA can vary across each route according to the SLA Matrix
- Working Days are defined as Mon - Sat, Excluding Public Holidays.
- Assume the following Public Holidays: 
  - 2020-03-08 (Sunday);
  - 2020-03-25 (Wednesday);
  - 2020-03-30 (Monday)
  - 2020-03-31 (Tuesday)
- SLA calculation begins from the next day after pickup (Day 0 = Day of Pickup; Day 1 = Next Day after Pickup)
- 2nd Attempt must be no later than 3 working days after the 1st Attempt, regardless of origin to destination route
- Only consider the date when determining if the order is late; ignore the time.

## Data
- SLA Matrix.xlsx - This contains the SLA for each pickup-destination pair
- delivery_orders_march.csv - This contains the all devlivery orders data to be used in the exercise
