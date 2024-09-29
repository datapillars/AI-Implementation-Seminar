# AI-Implementation-Seminar
Courier Assignment Model with Environmental Impact

System Requirements for Training and Working with the Data 

Program Requirements
Python Version: 3.11.9
The model was trained in Jupyter Notebooks, but the code can also run directly as a .py file without any modification.
Note: For future Python versions, the “append” method is depreciated. If a newer Python version is used, the “concat” method should be used for putting the final data in a data frame. 

Datasets Used:
all_waybill_info_meituan.csv
2021_Cars_Aggregated.csv
Data Link: https://drive.google.com/drive/folders/1LoDZXG93EYtUYOBlhiHwfzfzddSDX-sm?usp=sharing

Memory Usage:
Single Courier Training: 600 MB of RAM is required for training each model—both the fastest car model and the environmentally friendly model.
Multiprocessing: Since the model trains each day separately, the required memory increases with the number of days. For 8 days, the recommended RAM is 4.8 GB.
CPU Requirements: To run both models in parallel for 8 days of data, a total of 8 GB of CPU is required for safe execution. If data with different days will be used for the model, consider using a different approach for multiprocessing. 

Training Time:
Training each of the two models (fastest car and environmentally friendly model) for 100,000 orders with 20,000 available couriers over an average of 4 days (with 8 hours of availability) will take approximately 8 hours per model.
In total, training both models will take approximately 16 hours.

Required Libraries:
pandas (for data manipulation)
numpy (for numerical operations)
datetime (for handling date and time data)
psutil (for tracking memory usage)
multiprocessing (for parallel execution of the training process)
math (for mathematical calculations)

Extra Note for Data Loading 
You need to update the code to load data to the model. The data loading part is the second cell in the jupyter notebook. 
