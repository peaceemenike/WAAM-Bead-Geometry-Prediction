------------------------------------------------------------------------

## Dataset Description

The dataset contains WAAM process parameters and bead geometry measurements.
Columns include:

-   Voltage\
-   Wire Feed Speed (WFS)\
-   Travel Speed\
-   CTWD (Contact Tip–Workpiece Distance)\
-   AVERAGE (mean bead height)\
-   VARIANCE (variance of bead height)

The dataset is included to ensure full reproducibility.

------------------------------------------------------------------------

## **Exploratory Data Analysis (EDA)**

The notebook performs a complete EDA workflow, including:

-   Histograms of all variables\
-   Boxplots and outlier inspection\
-   Correlation heatmap\
-   Pair plots\
-   Combined scatterplot relationships\
-   Feature importance plots\
-   Model prediction plots (RF and NN)

Figures are saved inside the `figures/` directory.

------------------------------------------------------------------------

## **Machine Learning Models**

### Random Forest Regression

Used to predict: - AVERAGE bead height\
- VARIANCE of bead height

Evaluation metrics include RMSE, MAE, and R².

### Neural Network (Keras Sequential Model)

A multi-layer perceptron with:

-   Dense(64, activation = "relu")
-   Dense(32, activation = "relu")
-   Dense(16, activation = "relu")
-   Dense(2) output layer

Includes EarlyStopping and validation monitoring.

------------------------------------------------------------------------

## **Results Summary**

-   Both models perform well for AVERAGE prediction.
-   VARIANCE is more challenging due to noise and nonlinearity.
-   Random Forest generally outperforms the Neural Network for stability prediction.

A full comparison table is included in the report and notebook.

------------------------------------------------------------------------

## **Deliverables Included**

| Deliverable                | Location                             |
|----------------------------|--------------------------------------|
| Project Proposal           | `report/WAAM_Project_Proposal.pdf`   |
| Final Report (10–12 pages) | `report/WAAM_Final_Report.pdf`       |
| Dataset                    | `dataset/waam_bead_data.xlsx`        |
| Jupyter Notebook           | `notebooks/WAAM_Project.ipynb`       |
| All Figures                | `figures/`                           |
| Presentation               | `presentation/WAAM_Presentation.pdf` |

------------------------------------------------------------------------

##
