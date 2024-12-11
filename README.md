# Machine-Learning

## Description
This project focuses on building and saving a Machine Learning model, with the final step converting it into TFLite format. The notebook includes various stages, from data preparation to model storage.

## Project Structure
```
├── assets/                # Folder containing the images of documentation
├── dataset/               # Folder containing the dataset used for training, testing, and validation
├── saved_model/           # Folder for storing the TFLite model with and without metadata
├── README.md              # Documentation for the project
├── final_model.ipynb      # Notebook for training and converting the model into TFLite format
└── add_metadata.ipynb     # Notebook for adding metadata to the TFLite model
```

## Notebook Structure - [final_model.ipynb](https://github.com/CiMon-Capstone-Project/Machine-Learning/blob/main/final_model.ipynb)
- Installation
- Loading Dataset: Processing and loading the dataset from Google Drive. The dataset is provided as a compressed file (final_dataset.zip) and uploaded into the Colab environment.
- Data Exploration: Displaying example data for each class.
- Data Preprocessing: Converting images into their numpy array representations.
- Model Building: Creating and training the machine learning model.
- Saving the Model: Saving the trained model.
- TFLite Conversion: Converting the model into TFLite format for efficient deployment on mobile.

## Dataset
- Dataset Source: [Link to dataset](https://github.com/CiMon-Capstone-Project/Machine-Learning/blob/main/dataset/link-to-dataset.txt)

## Here’s a concise explanation of the model architecture
![image](https://github.com/CiMon-Capstone-Project/Machine-Learning/blob/main/assets/ML_Implementation.drawio.png)
- Preprocessing
  - Rescaling, adjusts the pixel values (scaling from [0, 255] to [0, 1]).
  - Normalization, ensures uniform data distribution to optimize training.
- Convolutional Layers
  - A series of convolutional layers (6 blocks of conv2d) extract hierarchical features like edges, textures, and patterns.
- Fully Connected Layers
  - GlobalAveragePooling2D to reduces the spatial dimensions, converting feature maps into vectors.
  - Dense Layers to learn complex relationships between features.
  - Dropout Layers to prevents overfitting by randomly deactivating neurons during training.
  - Softmax Layers to produces a probability distribution for classification.
- Output (5 classes of diseases)

## Tech Stack
- Google Colab for code execution
- Python as the primary programming language
- NumPy
- TensorFlow
- Matplotlib

## Contact 
If you have any questions, suggestions, or feedback, please feel free to reach out to us:
* Aprilia Wulandari [Linkedin](https://www.linkedin.com/in/aprilia-wulandari-/)
* Risma Saputri [Linkedin](https://www.linkedin.com/in/rismasaputri/)
* Tri Rambu Nugroho Prasetyo [Linkedin](https://www.linkedin.com/in/tri-rambu-nugroho-prasetyo/)
