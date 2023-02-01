# flightaware-analysis
 A Jupyter notebook to easily analyze travel times for a flight.

## What does it do?
This notebook helps analyze the duration of any given flight. It provides key statistics, a histogram, and plot of duration vs. date.

| Statistic | Description |
| --- | --- |
| `std` | Sample standard deviation. |
| `median` | Sample median. |
| `mean` | Sample mean. |
| `min` | Lowest value in sample. |
| `max` | Greatest value in sample. |
| `n` | Number of flights in sample. |

## How do I use it?

### Configure Repository
Clone this repository and run the following command to install dependencies:

```pip3 install -r requirements.txt```

You will need Jupyter notebook installed.  I use VSCode's built-in option ([ref](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)).

### Get Data
Go to [FlightAware](https://flightaware.com) and input your flight number. Select `flight schedule` and keep hitting `View More` until you've reached the limit (free accounts usually get 3 months of history).

Use [this](https://chrome.google.com/webstore/detail/download-table-as-csv/jgeonblahchgiadgojdjilffklaihalj) Chrome Extension to download flight data as a CSV.

Put the `.csv` in `./data`. Do **not** modify the raw output—this notebook contains code that cleans the data.

In `main.ipynb` (after starting the Jupyter kernel), modify the `DATA_SOURCE` variable to point to your flight's CSV.