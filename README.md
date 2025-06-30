# XEMPLA-AI-OM-PLATFORM



# Xempla AI O&M Platform (Simple Version)

> A basic project that shows how AI can help in maintenance work using simple tools like Python and a web page.

---

##  What This Project Does

- Shows 4 steps: Discover, Investigate, Implement, Verify (called DIIV)
- Helps users know if a machine might fail based on temperature and runtime
- Uses basic rules (you can upgrade to real machine learning later)
- Simple form where you type in data and get a prediction

---

##  Files in the Project

```
├── app.py                # Main Python program using Flask
├── model.py              # Simple logic to check for machine problems
├── templates/
│   └── index.html        # Web page form
├── static/
│   └── style.css         # Page design (colors, fonts, etc)
├── data/
│   └── sensor_data.csv   # Example input data
```

---

## 🚀 How to Run It

### What You Need First:
- Python installed
- pip (Python's installer)

### Steps:

```bash
# Download the project
git clone https://github.com/yourusername/xempla-ai-om-platform.git
cd xempla-ai-om-platform

# (Optional) Create a Python environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install Flask
pip install flask
```

### Start the App:

```bash
python app.py
```

Then open a browser and go to: `http://127.0.0.1:5000`

---

##  Example Data to Test
Input:
```json
{
  "temperature": 85,
  "runtime": 120
}
```
Output:
```json
{
  "alert": true,
  "message": "High risk of equipment failure!"
}
```

---

##  What Can Be Improved Later
- Use real machine learning for smarter predictions
- Store user data in a real database (like Firebase)
- Add login system and admin panel
- Connect with real devices or sensors (IoT)



