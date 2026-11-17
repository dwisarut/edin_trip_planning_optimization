# Edinburgh Trip Planning Optimization
Optimizing one-day trip in Edinburgh with CP-SAT, GA, and NSGA-II.

Link to the [dataset](https://sites.google.com/site/limkwanhui/datacode?pli=1&authuser=0).

## Objective
1. **Single Objective** - To find the combination that achieves the highest popularity score
2. **Multi Objective** - To find the combination that achieves the highest popularity score, while minimizing walking time in accordance to tourist's interest

## Project Structure

```txt
edin_trip_planning_optimization
├── data/                                    # Raw data
│   ├── POI-edin.csv                         # Point of interests in Edinburgh
│   ├── CostProfCat-EdinPOI-all.csv          # Distance from each POI to their destination
│   └── userVisits-Edin.csv                  # Data of user visits in each POI
├── single_objective/                        
│   ├── so_cpsat.ipynb
│   ├── so_mip.ipynb
│   └── ga.ipynb
├── multi_objective/
│   ├── mo_cpsat.ipynb
│   ├── mo_mip.ipynb
│   └── nsga_ii.ipynb
└── requirements.txt                         # Dependencies
```

## Getting Started
### Prerequisites
This project used python version 3.14.7

### Installation
1. Clone this repository:

   ```
   git clone https://github.com/dwisarut/edin_trip_planning_optimization.git
   cd edin_trip_planning_optimization
   ```

2. Create a virtual environment and activate

   - Window:
     
     ```
     python -m venv .venv
     .venv\Scripts\activate.ps1
     ```
     
   - macOS:
     
     ```
     python3 -m venv .venv
     source .venv/bin/activate
     ```

3. Install essential package:
   
   ```
   pip install -r requirements.txt
   ```
