# Top AI Stock Performance Analysis (Posit Table Contest 2024)

This repository contains code for an R script that analyzes the stock performance of the top 14 AI companies (May 2024) according to [Stash](https://www.stash.com/learn/top-ai-companies/) and presents the results in a visually appealing table using the `gt` and `gtExtras` packages.


**Note: In case you are using R Posit Cloud, please note that lines 199 to 209 of the code in the `Codes.R` script should be commented out, and line 212 should be uncommented to ensure proper execution.** 

## Functionality

The script performs the following tasks:

1.  **Data Acquisition:** Retrieves stock data for the past 52 weeks using the `quantmod` package.

2.  **Data Processing:** Calculates various metrics like current price, percentage change, 52-week high/low, and volume.

3.  **Table Creation:** Generates a table using `gt` and `gtExtras` packages. The table includes:

    -   Company logo

    -   Company name

    -   Ticker symbol

    -   Current price

    -   Percentage change in price (daily)

    -   Weekly percentage change in price (chart)

    -   52-week high

    -   52-week low

    -   Price Trend (chart)

    -   Current volume

    -   Percentage change in volume (daily)

    -   Volume trend (chart)


## Usage

1.  **Prerequisites:**

    -   R environment with required packages: `quantmod`, `lubridate`, `tidyverse`, `htmltools`, `purrr`, `plotly`, `gt`, `gtExtras`

    -   A working internet connection to download stock data.

2.  **Instructions:**

    -   Clone or download this repository.

    -   Ensure you have the required R packages installed (instructions provided in the code).

    -   Replace `"AI_Company_Data.csv"` with the path to your actual CSV file containing AI Company Data (optional, for reference).

    -   Run the script (`source('your_script_name.R')`). This will generate a table object named `table_final`.

    -   Use the `print(table_final)` command to view the table in the R console.

**Note:** This script retrieves data directly from Yahoo Finance.

## Additional Information

-   The script dynamically adjusts table width based on user screen resolution.

-   Logos for the companies are assumed to be placed in a folder named "Logos" within the project directory (modify the script for a different path).

-   The script includes comments and explanations for better understanding.
