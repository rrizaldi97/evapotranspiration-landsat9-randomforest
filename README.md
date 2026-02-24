# Spatio-Temporal Integration of Landsat 9 and Meteorological Data for Evapotranspiration Prediction in Oil Palm Plantations

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Machine Learning](https://img.shields.io/badge/Algorithm-Random%20Forest-green.svg)](https://scikit-learn.org/)
[![Remote Sensing](https://img.shields.io/badge/Satellite-Landsat%209-red.svg)](https://www.usgs.gov/landsat-missions/landsat-9)

## 📌 Research Overview
Penelitian ini mengembangkan kerangka kerja otomatisasi (automated framework) untuk mengestimasi laju evapotranspirasi (ET) harian pada ekosistem perkebunan kelapa sawit di **Rancabungur, Indonesia**. Dengan menggabungkan data penginderaan jauh termal dari satelit **Landsat 9** dan observasi meteorologi permukaan, model ini mampu memberikan presisi tinggi untuk manajemen irigasi presisi.

### Key Highlights:
- **Temporal Scope:** 731 hari observasi kontinu (Januari 2023 - Desember 2024).
- **Data Fusion:** Integrasi 46 dataset temporal Landsat 9 dengan data cuaca in-situ.
- **Key Discovery:** Validasi **Land Surface Temperature (LST)** sebagai proksi utama energi panas laten permukaan.
- **Performance:** Model mencapai **RMSE 0.687 mm**, memenuhi standar akurasi agrometeorologi internasional.

## 🛠️ System Architecture
Repositori ini disusun secara modular untuk menjamin transparansi data dan reproduksibilitas riset:

```text
.
├── data/
│   ├── raw/           # Raw Climate, SHP, and SRTM data
│   └── processed/     # Result of multi-source data fusion (CSV)
├── notebook/
│   └── main_analysis.ipynb   # Full end-to-end Python workflow
├── output/
│   ├── figures/       # High-resolution (300 DPI) publication-ready plots
│   └── maps/          # Topographic and spatial AOI profiles
├── requirements.txt   # List of required Python libraries
└── README.md
