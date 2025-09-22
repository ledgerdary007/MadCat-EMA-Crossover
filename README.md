# **MadCat EMA Crossover Indicator for TradingView**

A versatile and highly customizable EMA (Exponential Moving Average) crossover indicator for TradingView, written in Pine Script. This indicator is designed to provide clear buy and sell signals based on EMA crossovers and can be tailored to specific assets and timeframes through a powerful profiling system.

## **Overview**

The MadCat EMA Crossover indicator plots fast and slow EMAs on your chart and generates buy/sell signals when they cross. What sets it apart is its ability to automatically switch between up to 20 different pre-configured profiles based on the ticker and timeframe you are currently viewing. This allows traders to apply optimized settings for various assets without manual adjustments.

The script also includes longer-term EMAs (50, 100, 200\) for trend analysis and provides advanced alert conditions that can be used for automated trading strategies.

## **Key Features**

* **Dynamic EMA Profiles:** Configure up to 20 unique profiles, each with its own ticker, timeframe, and EMA settings. The script automatically applies the correct profile.  
* **Customizable Crossover EMAs:** Set default fast and slow EMA periods for general use.  
* **Trend-Confirming EMAs:** Includes optional 50, 100, and 200 EMAs to help gauge the longer-term trend.  
* **Visual Signals:** Clear, customizable buy (uptriangle) and sell (downtriangle) signals plotted directly on the chart.  
* **Advanced Alert System:** Create alerts for both pure EMA crossovers and filtered signals (e.g., "only trigger buy alerts if the price is below the 200 EMA").  
* **Information Table:** An on-screen table displays which profile is currently active and its corresponding EMA values, ensuring you always know what settings are being used.  
* **Clean, Organized Code:** The Pine Script code is well-commented and structured for easy modification.

## **How to Use**

1. **Copy the Code:** Open the MadCat\_EMA\_Crossover.pine script file and copy its entire contents.  
2. **Open Pine Editor in TradingView:** On your TradingView chart, click on the "Pine Editor" tab at the bottom.  
3. **Paste and Save:** Paste the copied code into the Pine Editor, replacing any default text. Click "Save", give it a name (e.g., "MadCat EMA Crossover"), and then click "Add to chart".

### **Configuration**

The indicator's settings allow for deep customization:

#### **EMA Profile Configuration**

* **Enable Ticker/Timeframe Profiles:** Toggle this on to use the profile system. If it's off, the script will use the Default Fast EMA and Default Slow EMA values on all charts.  
* **Profiles (1-20):**  
  * **Enabled:** Check this box to activate a specific profile.  
  * **Ticker:** Enter the exact ticker name (e.g., BITSTAMP:BTCUSD or NASDAQ:AAPL).  
  * **Timeframe:** Select the timeframe for this profile (e.g., 5, 15, 60, D).  
  * **Fast & Slow EMA:** Set the EMA periods for this specific profile.

#### **Display Table**

* **Show Info Table:** Toggles the visibility of the on-screen display.  
* **Table Position:** Choose where the table appears on your chart.

#### **Alert Settings**

You can create alerts based on several conditions within TradingView's "Create Alert" menu.

* **Buy/Sell EMA (Pure):** Triggers an alert on any crossover, regardless of other conditions.  
* **Buy/Sell EMA (Filtered):** Triggers an alert only if the crossover meets the conditions you set in the indicator's settings, such as:  
  * **Short Buy EMA Condition:** e.g., Below 200 EMA. A buy signal will only trigger an alert if the fast EMA is below the 200 EMA at the time of the cross.  
  * **Short Sell EMA Condition:** e.g., Above 200 EMA. A sell signal will only trigger an alert if the fast EMA is above the 200 EMA at the time of the cross.

## **License**

This project is licensed under the MIT License. See the LICENSE.md file for details.

