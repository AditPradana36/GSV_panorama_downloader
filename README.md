# GSV Batch Downloader

This repository contains a Jupyter Notebook (`GSV_batch_downloader.ipynb`) for downloading multiple Google Street View (GSV) images in batch using the Google Street View Static API. It is designed for researchers, GIS practitioners, and developers who need to collect GSV imagery for spatial analysis, computer vision, or urban studies.

---

## 📌 Features

- Download Street View images in bulk from a CSV or shapefile containing coordinates.
- Customizable parameters:
  - Image size
  - Field of view (FOV)
  - Heading & pitch
  - Output folder
- Supports API key authentication via Google Cloud.
- Progress tracking and error handling.

---

## 📂 Requirements

Make sure you have the following installed:

- Python 3.8+
- Jupyter Notebook
- Required libraries:
  ```bash
  pip install pandas requests tqdm geopandas shapely
  ```

---

## 🔑 API Key Setup

1. Go to **Google Cloud Console** → [Google Street View Static API](https://developers.google.com/maps/documentation/streetview/overview).
2. Create or select a project.
3. Enable **Street View Static API**.
4. Create an **API key**.
5. Copy the API key and paste it into the notebook’s `API_KEY` variable.

---

## 📥 How to Use

1. Open the notebook:
   ```bash
   jupyter notebook GSV_batch_downloader.ipynb
   ```
2. Load your coordinate file:
   - CSV with columns: `latitude`, `longitude`
   - or a shapefile containing point geometries
3. Set the output directory and API parameters in the notebook.
4. Run the notebook cells to start the download.
5. Images will be saved to your specified folder.

---

## 📄 Example CSV Format

```csv
id,latitude,longitude
1,-6.175392,106.827153
2,-6.208763,106.845599
```

---

## ⚠️ Notes & Limitations

- **Quota limits**: Google Street View Static API may have daily request quotas.  
- **Usage cost**: Downloads beyond free tier are billed according to Google Cloud pricing.
- **Legal**: Ensure you comply with [Google Maps Platform Terms of Service](https://cloud.google.com/maps-platform/terms).
- Images are for personal/research use unless otherwise permitted.

---

## 📜 License

This project is provided **as-is** for research and educational purposes.  
Ensure compliance with Google’s licensing before using the images commercially.

---

## ✨ Mohammad Raditia Pradana @2025

Developed by *[Your Name]* — inspired by the need to automate large-scale Street View imagery collection for spatial research.
