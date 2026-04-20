<p align="center">
  <img src="https://github.com/user-attachments/assets/9db5d1e9-8d26-4ba4-ba56-8c65076f0c0b" 
       alt="ARPS Zenith Ichimoku Framework"
       width="60%" />
</p>


# ARPS Zenith Ichimoku Framework
**Originally created: November 11, 2020**
*(Note: This script was created in 2020 but is being shared on GitHub on 2025-04-25)*

---

# ARPS Zenith Ichimoku Framework

The **ARPS Zenith Ichimoku Framework** is an advanced TradingView script powered by Pine Script developed to provide traders with an all-in-one trading indicator that combines Ichimoku-based strategies, moving average systems, volume-weighted metrics, trend lines, Williams fractals, and Stochastic RSI analysis. This script is designed to enhance trading efficiency with its comprehensive visualization of market trends and signals via customizable parameters and alerts.

---

## Features Overview

### General
- **Multiple Customizable Parameters**:
  - Set values for Ichimoku components, ZEMA periods, stochastic RSI smoothing, and others.
- **Dynamic Visualization**:
  - Colored components and arrows for enhanced readability.
- **Event-Driven Alerts**:
  - Real-time alert notifications for key trading events.
  
---

### Core Functionalities

#### 1. **Enhanced Ichimoku Cloud**
The script includes an Ichimoku cloud implementation with custom periods for:
- **Tenkan-Sen (Turning Line)**: Optionally offset for additional clarity.
- **Kijun-Sen (Standard Line)**: With period flexibility and enhanced styling.
- **Senkou Span A/B (Leading Spans)**: Colored cloud representation for bullish and bearish trends.
- **Chikou Span (Lagging Line)**: Combined with user-defined offsets for backtesting.
- **Crossovers and Arrows**:
  - Visual markers on Tenkan-Kijun crossovers (bullish/bearish entries).

#### 2. **Zero-Lag Exponential Moving Average (ZEMA)**
Calculate and display the Zero-Lag EMA with parameters for:
- **Timeframe**: Multiple resolutions.
- **Custom Calculations**: Using nested EMAs for smoothing.
- **Trend-Based Coloring**: Differentiates upward and downward market conditions.

#### 3. **Moving Average System**
- **T3 Moving Average**: Configurable length and volume factor.
  - Color-coded to highlight rising or falling conditions.
- **Stoploss Lines**:
  - Calculated using ATR for dynamic trailing stops.
- **Trend Direction Highlighting**:
  - Marks uptrend or downtrend regions based on ZEMA and price relationships.

#### 4. **Williams Fractals**
- Automatic detection and plotting of fractals for trend reversals:
  - **Upward Fractals**: Displayed below candles.
  - **Downward Fractals**: Displayed above candles.
  
#### 5. **Stochastic RSI Overlay**
- Visual representation of stochastic RSI conditions.
- Includes specific shapes to highlight bullish (upward crossover) and bearish (downward crossover) signals.

#### 6. **Alerts**
- Configure alerts for critical events such as:
  - **T3 Buy/Sell Signals**: Alerts triggered by T3 direction changes.
  - **Crossover Events**: Stochastic RSI and other indicators' crossovers.

---

## How to Use

1. **Add to TradingView**:
   - Copy the script provided and paste it into your TradingView Pine Script editor.
   - Click "Add to Chart" to apply the indicator to your trading chart.
   
2. **Set Custom Parameters**:
   - Use input fields to set thresholds and parameters for Ichimoku cloud, ZEMA, Stochastic RSI, T3, and other components.

3. **Enable/Disable Features**:
   - Turn on or off specific features like Williams fractals, alerts, MAs, and more.

4. **Interpret Visualizations**:
   - Leverage Ichimoku clouds, T3 overlays, and fractal points to analyze market conditions and identify potential entries/exits.

5. **Configure Alerts**:
   - Go to the TradingView "Alerts" tab and set automated alerts based on predefined conditions in the script.

---

## Parameters

### Ichimoku Cloud
| Parameter               | Default | Description                                      |
|-------------------------|---------|--------------------------------------------------|
| Tenkan-Sen Periods      | 20      | Period for the turning line.                    |
| Kijun-Sen Periods       | 60      | Period for the baseline.                        |
| Senkou Span B Periods   | 120     | Period for the leading span B line.             |
| Displacement            | 30      | Offset for leading/lagging spans.               |
| Show Tenkan-Sen         | `True`  | Toggle visibility of Tenkan-Sen.                |

### ZEMA
| Parameter          | Default | Description                                      |
|--------------------|---------|--------------------------------------------------|
| ZEMA Timeframe     | 60m     | Timeframe used for ZEMA calculations.            |
| ZEMA Period        | 42      | The length for ZEMA smoothing.                   |

### Moving Average System
| Parameter          | Default | Description                                      |
|--------------------|---------|--------------------------------------------------|
| T3 Length          | 21      | Length of the T3 moving average.                 |
| Volume Factor      | 0.98    | Sensitivity control for T3 calculations.         |

### Williams Fractals
| Parameter               | Default | Description                                      |
|-------------------------|---------|--------------------------------------------------|
| Show Upward Fractals    | `False` | Toggle visibility of upward fractals.           |
| Show Downward Fractals  | `False` | Toggle visibility of downward fractals.         |

---

## Alerts

### Types of Alerts
1. **T3 Buy/Sell Notifications**:
   - Alerts at bullish/bearish T3 crossovers.
2. **Stochastic RSI Signals**:
   - Notifications generated during upward or downward crossovers.

---

## Sample Use Cases
1. **Trend Confirmation**:
   - Combine Ichimoku cloud with ZEMA direction and T3 movements for multi-layered trend validation.
   
2. **Reversal Detection**:
   - Use Williams fractals and Stochastic RSI to identify reversal points.
   
3. **Risk Management**:
   - Configure dynamic stop-loss levels using ATR and Stoploss Lines.

---

## Contribution and Support
This indicator is designed and developed by **Ali Rajabpour-Sanati**.
For questions or support, feel free to contact me at **ali.poursanati@gmail.com**.

Enjoy trading with confidence! 💹
