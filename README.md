# **Mini Project 2 - ECoG Data Analysis**

## **Project Overview**
This project analyzes **Electrocorticography (ECoG) data** to compute and visualize **Event-Related Potentials (ERP)** associated with finger movements. The goal is to extract brain signals corresponding to finger movements, process them, and generate an averaged response for each finger.

## **Project Structure**
📂 mini_project2 │── 📂 mini_project_2_data # Contains the dataset files │── 📄 events_file_ordered.csv # Trial event timestamps and finger movements │── 📄 brain_data_channel_one.csv # ECoG signal data │── 📄 analysis.ipynb # Jupyter Notebook for data analysis │── 📄 README.md # Project documentation

## **Dataset Description**
- **`events_file_ordered.csv`**: Contains timestamps for trial start points, peak points, and associated finger movement (1-5).
- **`brain_data_channel_one.csv`**: A single-channel time-series dataset recording brain activity.

## **Methodology**
1. **Data Preprocessing**:
   - Read and clean trial event data (`events_file_ordered.csv`).
   - Load and format ECoG signal data (`brain_data_channel_one.csv`).

2. **ERP Computation**:
   - Extract brain signal segments around each movement event.
   - Compute the **mean ERP** for each finger by averaging across trials.

3. **Visualization**:
   - Generate ERP plots for each finger.
   - Display the final processed ERP matrix.

## **How to Run**
1. Clone this repository:
   ```bash
   git clone <https://github.com/disruptwood/miniproject2>
Open Jupyter Notebook:
jupyter notebook
Run analysis.ipynb to execute the ERP analysis.
Example ERP Output
The script generates a 5x1201 matrix, where each row represents the averaged brain response for one of the five fingers.
Libraries Used
pandas (for data manipulation)
numpy (for numerical operations)
matplotlib (for visualization)
Project Contributors
Ilya
