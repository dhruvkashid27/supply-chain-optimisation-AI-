Supply Chain Optimization AI

Purpose
Demonstrate how AI + Optimization can solve supply chain problems:
- Forecast demand (LSTM).
- Optimize transport (Linear Programming).

Outcomes
- **Forecasts**: 14-day rolling demand predictions (MAPE ~10–15%).  
- **Optimization**: DC→Store shipment plan with cost & CO₂ KPIs.  

Quickstart (Colab)
```python
!pip install pulp tensorflow pandas numpy
.
├── src/
│   ├── dl_forecasting.py
│   ├── transport_lp.py
├── data/
└── README.md

Forecast (next 14 days)
2025-01-01    240
2025-01-02    255
...

Shipment Plan (LP Optimal)
          Store1  Store2  Store3
DC_East     300     250     200
DC_West     150     200     180
