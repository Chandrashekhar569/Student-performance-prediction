# Student Performance Prediction

This project aims to predict student performance based on various factors. It uses machine learning techniques to analyze and predict the scores of students.

## Project Structure

The project is organized into the following main directories:

- `artifacts/`: Contains the data and model artifacts.
  - `data.csv`: Combined dataset used for training and testing.
  - `test.csv`: Testing dataset.
  - `train.csv`: Training dataset.
  - `model.pkl`: Trained model file.
  - `preprocessor.pkl`: Data preprocessing object.

- `notebook/`: Contains the dataset used for exploration and analysis.
  - `exams.csv`: Raw data file containing student exam scores.

- `src/`: Contains the source code for the project.
  - `components/`: Contains modules for data ingestion, data transformation, and model training.
    - `data_ingestion.py`: Module for ingesting data.
    - `data_transformation.py`: Module for transforming data.
    - `model_trainer.py`: Module for training the model.
  - `pipeline/`: Contains scripts for training and prediction pipelines.
    - `train_pipeline.py`: Script to run the training pipeline.
    - `predict_pipeline.py`: Script to run the prediction pipeline.
  - `logger.py`: Module for logging.
  - `exception.py`: Module for handling exceptions.
  - `utils.py`: Utility functions.

- `templates/`: Contains HTML templates for the web interface.
  - `home.html`
  - `index.html`

- `static/`: Contains static files for the web interface.
  - `styles.css`

## Getting Started

### Prerequisites

- Python 3.11
- Required Python packages (listed in `requirements.txt`)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Chandrashekhar569/Student-performance-prediction.git
    cd Student-performance-prediction
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

### Usage

1. **Data Ingestion**:
    Run the data ingestion module to load the data.
    ```bash
    python src/components/data_ingestion.py
    ```

2. **Data Transformation**:
    Transform the data using the data transformation module.
    ```bash
    python src/components/data_transformation.py
    ```

3. **Model Training**:
    Train the model using the training pipeline.
    ```bash
    python src/pipeline/train_pipeline.py
    ```

4. **Prediction**:
    Run the prediction pipeline to make predictions on new data.
    ```bash
    python src/pipeline/predict_pipeline.py
    ```

### Web Interface

To run the web interface, use a web framework like Flask (if Flask is used in your project):
1. Set the environment variable for Flask (if needed):
    ```bash
    export FLASK_APP=app.py
    export FLASK_ENV=development
    ```

2. Run the Flask application:
    ```bash
    flask run
    ```

Open your browser and go to `http://127.0.0.1:5000/predict` to see the web interface.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes.

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.
