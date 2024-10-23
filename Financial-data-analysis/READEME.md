# **Stock Price Analysis and Probability Distribution**

## **Project Overview**
This project involves analyzing stock price data to evaluate whether stock returns follow a normal distribution. The stock data for NASDAQ:GOOG was fetched using the Google Finance function in Google Sheets. The analysis focuses on calculating daily logarithmic returns and examining the distribution of these returns through histograms to identify normality.

**Objective**: To determine if stock returns are normally distributed, helping in assessing risks and making better financial decisions.

## **Dataset**
The dataset includes stock price data for NASDAQ:GOOG, spanning from **January 1, 1998** to **October 22, 2024**, with 2,662 rows and 3 columns:
- **Date**: The date of each trading day.
- **Close**: The stock's closing price for the day.
- **Return**: The calculated logarithmic return using the formula `Return = LN(Price_t / Price_t-1)`.

The data was collected using the Google Finance function in Google Sheets:
```plaintext
=GOOGLEFINANCE("NASDAQ:GOOG", "price", DATE(1998, 1, 1), TODAY(), "DAILY")
```

More details on the Google Finance function can be found [here](https://support.google.com/docs/answer/3093281?hl=en).

## **Project Structure**
The project is structured as follows:
- **Data Collection**: Stock price data is fetched using the `GOOGLEFINANCE` function in Google Sheets.
- **Logarithmic Return Calculation**: The daily logarithmic return is calculated using the formula `LN(Price_t / Price_t-1)`.
- **Normality Test**: A histogram is plotted to visualize the distribution of returns and assess whether it follows a normal distribution.
  
## **Installation**
To run this project locally, follow these steps:
1. Download or clone the repository:
    ```bash
    git clone https://github.com/Maha0001/guided-project.git
    cd guided-project
    ```
2. Use spreadsheet software (e.g., Excel or Google Sheets) to analyze the data or export the data to your preferred analysis tool like Python for further processing.

## **Key Findings**
- The calculated logarithmic returns were plotted in a histogram to check for normality.
- Visual analysis indicated that the stock returns follow a near-normal distribution, with minor deviations during market volatility.

## **Conclusion**
The findings suggest that stock returns for NASDAQ:GOOG exhibit characteristics of a normal distribution, which can be useful for financial modeling and risk assessment.
