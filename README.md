# 🌱 NAMA'A | Smart Agricultural Monitoring Platform

**Smart Agricultural Monitoring & Field Transformation using NASA Data in Jazan, Saudi Arabia**[span_0](start_span)[span_0](end_span).  
*Submitted to: NASA Space Apps Challenge*

---

## 🎯 Overview & Problem Statement
Farms in Jazan face growing climate pressures, while farmers need earlier warnings to prevent unexpected losses[span_1](start_span)[span_1](end_span). **NAMA'A** addresses key regional challenges:
* **Rising Heat:** Extreme temperatures strain crops and reduce productivity[span_2](start_span)[span_2](end_span).
* **Scarce Water:** Limited water availability makes irrigation increasingly challenging[span_3](start_span)[span_3](end_span).
* **Shifting Vegetation Health:** Changes in plant health signal deeper ecosystem stress[span_4](start_span)[span_4](end_span).
* **Unpredictable Rainfall:** Erratic rains disrupt planning and increase risk for farmers[span_5](start_span)[span_5](end_span).

---

## 💡 The Solution: NAMA'A
NAMA'A bridges the gap between satellite data and field decisions by providing smart monitoring, early risk detection, and actionable agricultural recommendations[span_6](start_span)[span_6](end_span)[span_7](start_span)[span_7](end_span):
* **Vegetation Health Tracking:** Monitors crop conditions from `Excellent` to `Very Poor`[span_8](start_span)[span_8](end_span).
* **Early Risk Identification:** Detects elevated heat and water stress before crop damage occurs[span_9](start_span)[span_9](end_span).
* **Actionable Guidance:** Suggests optimized irrigation scheduling and monitoring for vulnerable fields[span_10](start_span)[span_10](end_span).

---

## 🛰️ NASA Data Sources & Tech Stack
NAMA'A integrates multi-source Earth observation data and machine learning[span_11](start_span)[span_11](end_span):
* **Landsat 8 & 9 (OLI / OLI-2):** 30m resolution for Vegetation Index calculation ($NDVI = \frac{NIR - Red}{NIR + Red}$)[span_12](start_span)[span_12](end_span).
* **MODIS MOD13Q1:** 250m resolution (16-day observations) for seasonal vegetation tracking[span_13](start_span)[span_13](end_span).
* **GPM IMERG:** Near-real-time global precipitation and rainfall tracking[span_14](start_span)[span_14](end_span).
* **NASA POWER API:** Meteorological data for surface temperature ($T2M$) and humidity ($RH2M$).
* **SRTM DEM:** Topography, elevation, and land slope analysis.
* **Artificial Intelligence:** **Isolation Forest** (`scikit-learn`) for automated anomaly and early crop stress detection.

---

## 🚀 How to Run the AI & NASA Data Model

```bash
# 1. Clone the repository
git clone [https://github.com/jana99-cloud/midad-agricultural-platform.git](https://github.com/jana99-cloud/midad-agricultural-platform.git)
cd midad-agricultural-platform/model

# 2. Install required dependencies
pip install -r requirements.txt

# 3. Run the analysis model (Pilot Farm: Al-Wadi Farm, Sabya - Jazan)
python namaa_model.py
