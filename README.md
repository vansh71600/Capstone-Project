Brief overview: The Dynamic Pricing for Urban Parking Lots project is a real-time analytics project. I build a smart pricing engine for 14 parking lots using real-time data and custom models in Python, Pandas, Numpy, and Pathway. The data includes parking occupancy, vehicle types, queue lengths, traffic conditions, and event indicators over 73 days. The goal is to dynamically adjust parking prices based on demand, starting from a base price of $10. Three models are to be built: a baseline linear model, a demand-based model using key features, and an optional competitive model that factors in nearby parking lots. Final outputs include real-time price predictions, Bokeh visualizations, and a report explaining the logic and results.


Tech stacks used: Language:-Python
                  Libraries:- pandas, numpy, bokeh
                  Streaming & Real-Time Framework:-Pathway
                  Environmet:-Visual studio code

                  
![arch](https://github.com/user-attachments/assets/829f6f29-1d46-49ec-beb4-3a219b70e03b)

                  
Workflow: it starts by loading the file by using pandas, filling the missing values and then followed by sorting the data by lot_id or timestamp for the sequential processing of the data. then we define a base price and set weight parameter and then we added important columns.
In model 1: For each time step and parking lot: Price_next = Price_current + α * (Occupancy / Capacity) and update the price column over the time.
In model 2: Define a demand function using features: Occupancy Rate, Queue Length, Traffic Level, Special Day Indicator, Vehicle Type (with weights)
Normalize the demand using MinMaxScaler: Calculate price: Price = BasePrice * (1 + λ * NormalizedDemand)
Ensure price stays between 0.5× and 2× base
following this comes real time integration with pathway, visualisation by bokeh and then by saving the results.














