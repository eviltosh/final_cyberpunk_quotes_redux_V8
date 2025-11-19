# Cyberpunk Quotes Redux — V8

A high‑performance, neon‑infused Streamlit application that displays real‑time stock quotes in a fully custom cyberpunk UI. This project merges fast financial data handling with a highly stylized interface featuring animated backgrounds, custom typography, and precision‑aligned UI components.

---

## 🚀 Features

### **🔹 Real‑Time Financial Data**
- Fetches and displays up‑to‑date stock price information
- Includes percentage change, daily change, and other key metrics
- Automatically retries data sources to ensure reliability

### **🔹 Cyberpunk UI Theme**
- Fully customized CSS with neon effects
- Embedded pixel‑perfect fonts
- Animated cyberpunk background imagery
- Glowing highlights and precise typography tuning

### **🔹 Clean Metric Layout**
- Optimized 2x2 metric grid
- Cyan labels & values for readability
- Restored red/green delta colors for positive/negative moves

### **🔹 Modular Code Structure**
- `app_core.py` handles data and logic
- `app_render.py` manages UI layout and visuals
- `cyberpunk_style_embedded.css` contains all custom styling
- Easy to extend or modify without breaking the design

---

## 📁 Project Structure

```
/project_root
│
├── app_core.py                  # Main app controller + data fetching
├── app_render.py                # All UI components + layout
├── cyberpunk_style_embedded.css # Full theme + animations
└── README.md                    # You are here
```

---

## 🧩 How It Works

### **1. Data Layer** (`app_core.py`)
- Handles ticker input and retrieval
- Caches data for performance
- Normalizes results to keep the UI consistent

### **2. UI Layer** (`app_render.py`)
- Builds the Streamlit view
- Applies CSS via safe_markdown
- Renders metrics, logos, titles, and layout blocks

### **3. Styling Layer** (`cyberpunk_style_embedded.css`)
- Adds embedded fonts
- Defines neon glow
- Animates backgrounds
- Ensures responsive layout

---

## 📦 Installation

### **Requirements**
- Python 3.10+
- pip

### **Installation Steps**

```bash
git clone https://github.com/eviltosh/final_cyberpunk_quotes_redux_V8.git
cd final_cyberpunk_quotes_redux_V8
pip install -r requirements.txt
```

---

## ▶️ Running the App
```bash
streamlit run app_core.py
```
The app will launch in your browser.

---

## 🎨 Customization

You can safely modify:
- Background images
- Typography
- Neon intensities
- Metric alignment
- Color schemes

All theme changes live in:
```
cyberpunk_style_embedded.css
```

Metric-specific overrides can be injected through small `<style>` blocks in:
```
app_render.py
```

---

## 🛠 Troubleshooting

### Metrics all appear white
You may be overriding delta colors accidentally. Use the correct delta selector based on your DOM version.

### Logo not appearing
Ensure correct path and MIME-safe filenames.

### White flash during load
Check splash sequence and Streamlit container layering.

---

## 🤝 Contributing
Pull requests are welcome. Stick to the modular file structure and keep the theme consistent.

---

## 💬 Support
If you need help with customization, styling, or performance improvements, open an issue or contact the maintainer.

---

## 🧠 Credits
Developed by **eviltosh** with collaboration and iterative engineering powered by **Q (AI assistant)**.

Cyberpunk aesthetic inspired by classic neon sci‑fi visuals.

---

Enjoy the neon glow ⚡

