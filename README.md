## 📓 Notebooks Overview

| Notebook | Description |
|----------|-------------|
| **`Final_taking_day_in_July.ipynb`** | Loads and filters CSV files from selected directories. Extracts only valid rows (`1802 != -1`) and appends a `"Day"` column based on filenames (e.g., `day12.csv` → Day 12). Useful for supervised training dataset preparation. |
| **`ROI_creation_checkpoint.ipynb`** | Extracts and saves regions of interest (ROIs) from wind and pressure data per row. Also visualizes each ROI and saves the output to `extracted_region_viz/`. Ensures CNN models are trained on structured spatial sections. |
| **`CNN_Prediction_second_step.ipynb`** | Loads pre-trained CNN models to predict atmospheric classes for test samples. Generates color-coded image comparisons (real vs predicted) for each day and saves them in `cnn_predict/`. Also includes legends for clarity. |
| **`CNN_Bayesian_first_step.ipynb`** | Trains convolutional neural networks using Bayesian approaches to capture predictive uncertainty in atmospheric classifications. Includes uncertainty visualization and probabilistic output analysis to enhance model interpretability and robustness. |

## 📊 Example Visualizations

- **Classified weather patterns** using CNNs (real vs predicted).
- **Spatial ROIs** for wind and pressure extracted per row.
- **Cluster evolution** using SOMs for unsupervised analysis.

<p align="center">
  <img src="cnn_predict/example_day_12.png" width="500" alt="Real vs Predicted">
</p>

## ⚙️ Technologies Used

- **Python 3.x**
- **TensorFlow / PyTorch** – for CNN modeling
- **MiniSom / SOMPY / Custom SOMs** – for clustering atmospheric patterns
- **OpenCV / Matplotlib / Seaborn** – for image and data visualization
- **Pandas / NumPy / Scikit-learn** – for preprocessing and data handling

## 🚀 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/prakhai03/climate-change-project.git
cd climate-change-project
