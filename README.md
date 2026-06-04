# 🚨 Chicago Crime Advanced Geospatial Analytics Dashboard

## 🎨 Interface & Dashboard Overview

The dashboard breaks away from traditional jarring page reloads by using a single-page layout. Smooth scroll action selectors automatically glide the browser pane into focus, flashing distinct animated light themes custom-engineered for each analytic module:

1. **🔥 Crime Hotspot Heatmap (Soft Red/Rose Theme):** Uses Kernel Density Estimation (KDE) over a Folium map script layer to seamlessly isolate high-intensity crime density clusters without marker clutter.
2. **🛡️ District Hazard Profiles (Soft Teal Theme):** Aggregates total criminal volume per administrative police unit, serving a high-resolution static bar chart beside an interactive centroid map tracking the Top 5 peak hazards.
3. **🤖 K-Means Spatial Clusters (Soft Cream Theme):** Applies unsupervised machine learning ($K$-Means Clustering) to mathematically group geographic observation coordinate matrices into 5 distinct localized quadrants.

---

## 🛠️ Architecture & Technical Stack

The technical design relies on Python backend script vectors and standard frontend presentation scripts:

* **Backend Web Core:** Flask (WSGI Engine)
* **Geospatial Rendering:** Folium & Leaflet.js
* **Machine Learning Engine:** Scikit-Learn ($K$-Means Model)
* **Data Aggregation:** Pandas & NumPy
* **Visualizations:** Matplotlib & Seaborn
* **UI Layout:** Bootstrap 5 Framework (CSS Grid & Utilities)
* **Production Server:** Gunicorn

---

## 📂 Project Structure

```text
chicago-crime-dashboard/
│
├── app.py                      # Core Flask deployment backend script
├── cleaned_chicago_crimes.csv   # Geospatial dataset (Optimized sample matrix)
├── requirements.txt            # Python server production package locks
├── Procfile                    # Render/Heroku environment process instruction
└── templates/
    └── dashboard.html          # Frontend structural markup with embedded CSS animations






