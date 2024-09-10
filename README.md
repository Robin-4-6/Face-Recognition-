# Face Recognition System

## Project Overview

This project is a face recognition system that uses the Labeled Faces in the Wild (LFW) dataset. The system compares a given face image against a dataset of known faces to identify the most similar matches. It uses the FaceNet model for embedding extraction and FAISS for similarity search. The project includes a user interface built with Gradio for easy face image uploads and recognition.

## How It Works

1. **Dataset Loading**:
   - The LFW dataset is loaded, containing images and labels for known individuals.

2. **Face Embedding Extraction**:
   - Each face image is processed to extract facial embeddings using the FaceNet model.

3. **FAISS Indexing**:
   - The extracted embeddings are indexed using FAISS to enable fast similarity searches.

4. **Face Recognition**:
   - Upon uploading a new face image, the system finds the most similar faces from the dataset and returns the closest match along with a similarity score.

5. **User Interface**:
   - The Gradio interface allows users to upload a face image and receive recognition results.


## Files Included
- `Project.py`: Contains the entire code for the project.
- `requirements.txt`: Lists the libraries required to run the project.
- `Project.ipynb`: A Jupyter Notebook version of the project for interactive use.

## How to Use
1. **Set Up Your Environment**
   - Install the necessary libraries using the `requirements.txt` file:
     ```bash
     pip install -r requirements.txt
     ```

2. **Run the Script**
   - Execute the `Project.py` script to start the Gradio interface:
     ```bash
     python Project.py
     ```
   - The script will generate a link for the Gradio interface. This link will expire in 72 hours. You need to run the script again to generate a new link if needed.

3. **Using the Interface**
   - Upload any image, and the system will analyze it to find its closest match from the famous individuals. 
   - The system generates all necessary data during execution, including embeddings and FAISS index, so no pre-uploaded model or dataset is needed.

## Note
The project was developed and tested using Google Colab, which is why the code is contained in a single file. 







