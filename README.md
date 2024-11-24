# Efficient Data Stream Anomaly Detection
---

## Project Overview

The **Efficient Data Stream Anomaly Detection** project focuses on developing a Python script that detects anomalies in a continuous data stream. The stream simulates real-time sequences of floating-point numbers, representing various metrics such as financial transactions or system performance. The goal is to identify unusual patterns, such as high deviations from the norm, efficiently and accurately.

## Features

- **Algorithm Selection**: Utilizes the **Isolation Forest** algorithm to detect anomalies in real-time data streams, known for its robustness in high-dimensional data.
- **Data Stream Simulation**: Incorporates multiple datasets to emulate different types of data streams, including seasonal trends, regular patterns, and random noise.
- **Anomaly Detection**: Flags and visualizes anomalies in real time, enabling immediate detection of deviations from expected patterns.
- **Optimization**: The Isolation Forest algorithm is tuned for speed and efficiency to handle large data streams in real time.
- **Visualization**: Real-time graphing of the data stream with anomalies highlighted for easy identification.
- **CSV Export**: Detected anomalies can be exported to a CSV file for further analysis or reporting.

## Datasets Used

- **CPU Utilization Dataset**: Represents real-time CPU usage on Amazon EC2.
- **Temperature Data**: Simulates temperature variations in a system, including potential failures due to extreme conditions.
- **NYC Taxi Demand**: Tracks demand for taxi services in New York City over time.

All datasets are sourced from Kaggle (see **Data Sources** below).

## How to Use

1. **Installation**:

   Clone the repository and install the required packages:

   ```bash
   git clone https://github.com/zsh28/Efficient-Data-Stream-Anomaly-Detection
   cd Efficient-Data-Stream-Anomaly-Detection
   ```

   1.1 **Create a Virtual Environment**:

   Create and activate a virtual environment for an isolated environment:

   **On Windows**:
   ```bash
   python -m venv venv
   .\venv\Scripts\activate
   ```

   **On macOS/Linux**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

   1.2 **Install Dependencies**:

   Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. **Running the Project**:
   
   Execute the main script to start the anomaly detection process:

   ```bash
   python main.py
   ```

   The script will load the CPU Utilization dataset by default. You can switch between datasets and export detected anomalies to a CSV file using the provided controls.

3. **Controls**:
   - **Switch Dataset**: Switch between the provided datasets (CPU Utilization, Temperature Data, NYC Taxi Demand).
   - **Export CSV**: Export the detected anomalies to a CSV file with timestamp, value, mean, and standard deviation.

4. **Customization**:
   
   Adjust parameters like the contamination level (defining the percentage of anomalies) in the `process_full_data()` function for fine-tuning.

## Dependencies

- Python 3.x
- `matplotlib`: For real-time visualization.
- `pandas`: For data handling and manipulation.
- `sklearn`: For implementing the Isolation Forest algorithm.

Install dependencies using:

```bash
pip install -r requirements.txt
```

## Credits

### Data Sources:
- [Kaggle Dataset](https://www.kaggle.com/code/joshuaswords/time-series-anomaly-detection/input)

### Research:
- Isolation Forest-based anomaly detection inspired by:
  - [Anomaly Detection Techniques Summary](https://www.kaggle.com/code/praxitelisk/anomaly-detection-techniques-summary/notebook#Z-Score-anomalies-(Statistical-Method))
  - [Practical Approach to Z-Score Anomalies](https://medium.com/@akashsri306/detecting-anomalies-with-z-scores-a-practical-approach-2f9a0f27458d)

# Efficient-Data-Stream-Anomaly-Detection
