# Work_shifts
This repository contains the data and model to help developing work shifts for operational workers in a dark kitchen company.

# Data
The data file contains the upper tolerance limit of orders for both kitchens and retail operations, covering 90% of orders with 95% confidence.<br>
This file also has the minimum of workers for each hour and weekday in each unit, calculated by the UTLs of orders and rounded to the next higher integer.<br>
It also contains the results produced by the model for each unit, with numbers of workers in each regime and total cost.

# Model
The model file contains the restrictions, decision variables and objective function (total cost) used by the model, which is the extension OpenSolver in GoogleSheets.<br>
The yellow cells in the upper part of the sheet should be completed with the minimum of workers for each unit in the data file.<br>
The OpenSolver sidebar should be completed as the following image:

<img width="257" height="757" alt="image" src="https://github.com/user-attachments/assets/e21c26a3-5b7c-43c6-9959-d4b46fe993d7" />

After running the model, the optimal solution should appear in the bottom, with the number of workers in each regime and the total monthly cost for the unit.
