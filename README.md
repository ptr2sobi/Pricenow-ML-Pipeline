# Pricenow-ML-Pipeline
Configurable ML Framework to handle complex ML pipeline workflows


#### Prerequisites
Before running/cloning the code, make sure you have the following installed on your system:

Operating System: Windows WSL/ Linux/ MacOs
Tools: An IDE, Python 3 (or above)

#### Setup:

Clone the repository on your local machine using this command:
git clone https://github.com/ptr2sobi/Pricenow-ML-Pipeline.git
 - Open a command prompt or terminal window and navigate to the directory(Pricenow-ML-Pipeline) where the code is located.
 - Set Up the project on your IDE and configure a python interpretter.
 - Navigate to the terminal:
    - Activate your virtual environment (if you're using one) by running the command: 'source venv/bin/activate' on MacOS or '.\venv\Scripts\activate' on Windows.
 - Install all the necessary libraries using the command.
 - pip install -r requirements.txt
 - Optionally, you can change the configurations of the pipline through the configs.yaml file
 - navigate to the main.py driver file, where you can execute the whole pipeline 
  


#### Code Overview

  - DataLoader.py: This script contains a DataLoader class that is responsible for loading the dataset. It supports different file types and can be easily extended to support more.

  - DataSplitter.py: This script contains a DataSplitter class that splits the provided data into train and test sets based on the provided split ratio.

  - FeatureEngineer.py: This script contains a FeatureEngineer class that is responsible for performing feature engineering operations on the dataset.

  - InitializePipeline.py: This script contains an InitializePipeline class that is responsible for initializing the pipeline with configurations from a configuration file.

  - Model.py: This script contains a Model class that is responsible for initializing the machine learning model with given hyperparameters.

  - ModelEvaluation.py: This script contains a ModelEvaluation class that evaluates the trained model using different evaluation metrics.

  - ModelTester.py: This script contains a ModelTester class that tests the trained model on the test dataset and generates predictions.

  - ModelTrainer.py: This script contains a ModelTrainer class that trains the model on the training dataset.

  - PipelineExecuter.py: This script contains a PipelineExecuter class that executes the pipeline. It makes use of the classes mentioned above to perform various steps like data loading, preprocessing, feature engineering, model training, testing, and evaluation.

  - Preprocessor.py: This script contains a Preprocessor class that is responsible for preprocessing operations on the dataset.

  - README.md: This is a markdown file that provides an overview of the project and how to set up and run the project.

  - configs.yaml: This is a configuration file in YAML format that stores various configurations like hyperparameters for the model, features list, target variable, test size etc.

  - main.py: This is the main script that is used to run the project. It uses the PipelineExecuter class to execute the pipeline.

  - requirements.txt: This file contains all the Python dependencies that are required by the project. It's used by pip to install the dependencies.
