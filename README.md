This project implements a **medium-frequency mean-reversion strategy** on the **BankNifty-Nifty spread**  

Models Overview  

### **1. Baseline Z-Score Model** 
The baseline model uses the **z-score** of the spread between **BankNifty** and **Nifty** to identify trading signals:  

- **Spread** = BankNifty - Nifty  
- **Z-score** = (Spread - Rolling Mean) / Rolling Std Dev  


### **2. Machine Learning Approach** 
A **feature-rich ML model** was tested to predict spread direction:  
- Features: Time-based, momentum-based, z-scores of different timeframes 
- Model: LightGBM  

