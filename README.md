cat > README.md <<EOF
# National Geo-AI Hackathon - Theme 1 (SVAMITVA Scheme)

**Objective:** Automatically extract features from drone-based orthophotos using AI/ML.

## 📂 Repository Structure
The source code is located in the \`Theme1/\` folder.
**Note:** Large datasets (training images, shapefiles) and processed tiles are **not included** in this repository to maintain lightweight version control.

## 🚀 Setup Instructions

### 1. Clone the Repository
\`\`\`bash
git clone https://github.com/YOUR_USERNAME/National-Geo-AI-Hackathon.git
cd National-Geo-AI-Hackathon
\`\`\`

### 2. ⚠️ Data Setup (Crucial)
Since the dataset is not uploaded, you must set up the data locally for the code to run.
Download the data from this link: https://docs.google.com/spreadsheets/d/1PNDSmS6M63XH-0ed6OYVYLRHc_CgtZMy/edit?gid=2013070920#gid=2013070920
Create folders in the root folder (Theme 1) as follows, along with the cloned files:

\`\`\`text
Theme 1/
├── Final Model Training + Predictions/
│   ├── test_predictions/
│   ├── test_predictions_overlap/
│   ├── test_predictions_report/
├── processed_tiles/    #leave empty until you run chhattisgarh_tiling_masking.ipynb and punjab_tiling_masking.ipynb
│   ├── images/
│   │   ├── chhattisgarh/
│   │   └── punjab/
│   └── masks/
│       ├── chhattisgarh/
│       └── punjab/
├── raw_images/
│   ├── chhattisgarh/    #upload 5 .tif files for chhattisgarh training villages (Convert any .ecw to .tifs if needed)
│   └── punjab/          #upload 5 .tif files for punjab training villages (Convert any .ecw to .tifs if needed)
├── raw_shapes/
│   ├── chhattisgarh/    #upload shp folder package for chhattisgarh training villages
│   └── punjab/          #upload shp folder package for punjab training villages
├── test_data/
│   ├── chhattisgarh/    #upload 5 test .tif files for chhattisgarh training villages (Convert any .ecw to .tifs if needed)
│   └── punjab/          #upload 5 test .tif files for punjab training villages (Convert any .ecw to .tifs if needed)

\`\`\`

## 🏃‍♂️ How to Run

1.  Navigate to the source folder:
    \`\`\`bash
    cd Theme1
    \`\`\`
2.  Run chhattisgarh_tiling_masking.ipynb and punjab_tiling_masking.ipynb
3.  Run Final Model Training + Predictions/model_training+predictions_ipynb
    

EOF