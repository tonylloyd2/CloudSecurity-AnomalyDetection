# CloudSecurity-AnomalyDetection

This repository contains the code and resources for a project focused on **enhancing data privacy and security in cloud computing** by integrating advanced cryptographic techniques (AES and homomorphic encryption) with **machine learning models for real-time anomaly detection**. The project uses the **BETH Dataset**, a modern cybersecurity dataset, to develop robust models capable of detecting anomalies and potential security threats in cloud environments.

## Project Overview

The primary goal of this project is to improve data privacy and security in cloud computing environments by leveraging advanced cryptographic techniques and machine learning models. The project specifically integrates:

- **AES (Advanced Encryption Standard)** for securing data at rest and in transit.
- **Homomorphic encryption** for enabling secure computations on encrypted data without needing to decrypt it.
- **Machine Learning Models** (such as SVMs and Neural Networks) to perform **real-time anomaly detection** on encrypted data.

The project will use **HPC resources**, cloud services (e.g., Google Cloud, AWS Free Tier), and Python-based frameworks for implementation.

## Key Features

- **Data Preprocessing**: Cleaning, transforming, and handling missing values in the dataset.
- **Model Training**: Developing machine learning models for anomaly detection using the BETH dataset.
- **Encryption**: Implementing AES and homomorphic encryption to secure data in cloud environments.
- **Anomaly Detection**: Real-time detection of anomalous behavior using machine learning models on encrypted data.
  
## Dataset

We are using the **BETH Dataset**—a large, real-world cybersecurity dataset containing host activity and network traffic logs. This dataset is ideal for **anomaly detection** and **cybersecurity research**.

You can find more details on the BETH dataset in the associated [GitHub Repository](https://github.com/jinxmirror13/BETH_Dataset_Analysis).

## Project Structure

```
├── data/                   # Directory containing datasets
│   ├── raw/                # Raw, unprocessed data
│   └── processed/          # Processed data ready for model training
├── src/                    # Source code for the project
│   ├── preprocessing/      # Scripts for data cleaning and preprocessing
│   ├── models/             # Machine learning models for anomaly detection
│   ├── encryption/         # AES and homomorphic encryption implementation
│   └── evaluation/         # Scripts for model evaluation and performance tracking
├── notebooks/              # Jupyter notebooks for exploratory data analysis
├── results/                # Directory for saving results (e.g., model outputs)
├── README.md               # Project documentation
└── requirements.txt        # Required Python packages
```

## Installation

To set up the project on your local machine, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/CloudSecurity-AnomalyDetection.git
   cd CloudSecurity-AnomalyDetection
   ```

2. **Create a Virtual Environment**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   Install the required Python libraries using `pip`:
   ```bash
   pip install -r requirements.txt
   ```

4. **Download the Dataset**:
   Download the BETH dataset from [BETH Dataset Repository](https://github.com/jinxmirror13/BETH_Dataset_Analysis) and place it in the `data/raw/` directory.

5. **Run Preprocessing**:
   Clean and preprocess the dataset using the following script:
   ```bash
   python src/preprocessing/clean_data.py
   ```

6. **Train the Model**:
   After preprocessing, train the machine learning model using:
   ```bash
   python src/models/train_model.py
   ```

7. **Encrypt Data**:
   Apply AES or homomorphic encryption to the processed data:
   ```bash
   python src/encryption/encrypt_data.py
   ```

8. **Anomaly Detection**:
   Run the anomaly detection model on encrypted data:
   ```bash
   python src/models/anomaly_detection.py
   ```

## Dependencies

- Python 3.8+
- NumPy
- Pandas
- Scikit-learn
- TensorFlow
- PyCryptodome (for AES)
- TenSEAL (for homomorphic encryption)
- Matplotlib (for data visualization)

You can install all dependencies using the `requirements.txt` file.

## How to Contribute

If you would like to contribute to the project:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Submit a pull request for review.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this project with attribution.
