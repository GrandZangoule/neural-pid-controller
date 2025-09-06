# neural-pid-controller
🔧🎯🔁🧠 Research on advanced process control: classical PID with enhancements vs a neural controller trained with backpropagation.

## 📌 Features
- Classical PID with:
  - Setpoint weighting (β, γ)
  - Anti-windup
  - Derivative filtering
  - Output limits & rate limits
  - Bumpless transfer
- Up to **3 feedforward signals**
- Support for up to **5 disturbances**
- Neural PID (NPID):
  - Backpropagation-inspired controller
  - Gradient descent optimization of control performance
  - Learns contribution of feedforwards and components
- Plant models:
  - FOPDT
  - Flash / column dynamics

## 🚀 Run
```bash
python -m venv .venv && . .venv/Scripts/activate
pip install -r requirements.txt
python experiments/compare.py
