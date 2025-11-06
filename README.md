# Smart Microgrid Optimization with PV, Battery Storage, and Demand Response
### A Linear Programming Approach

This project presents an optimization-based framework for designing and operating behind-the-meter (BTM) and microgrid energy systems that integrate solar PV generation, battery energy storage systems (BESS), and grid interaction under multiple load types. A Mixed-Integer Linear Programming (MILP) model is developed to minimize total electricity costs while determining the optimal scheduling of appliances, battery charge–discharge cycles, and grid import/export decisions within technical and operational constraints.

The model explicitly differentiates between critical, flexible, and curtailable loads, ensuring reliable supply to essential appliances while allowing flexible ones to shift consumption in response to time-of-use (TOU) pricing and demand response (DR) events. Through this approach, the framework enhances cost-efficiency, reduces peak demand, and maintains system reliability without compromising operational flexibility.

The dataset, obtained from the Open Power System Data repository (11 German households), was preprocessed using Python for data cleaning, aggregation, and load classification.

The original dataset is available here:  
👉 [Open Power System Data – Household Data (Germany)](https://data.open-power-system-data.org/household_data/)

To run the model locally, place the dataset in `datasets/household_data_60min_singleindex.csv`.

This classification enables the MILP model to simulate realistic DR participation by automatically determining when to consume, defer, or store energy in alignment with dynamic pricing signals
