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

## How to Use

1. **Install Required Libraries**:
   - Ensure you have the necessary libraries installed. You can install them using the following commands:
     ```bash
     pip install deepface
     pip install faiss-cpu
     pip install gradio
     ```

2. **Run the Code**:
   - Load the dataset, extract embeddings, create the FAISS index, and build the Gradio interface.

3. **Upload an Image**:
   - Use the Gradio interface to upload a face image. The system will analyze the image and display the name of the most similar known individual along with the similarity score.
     -Note that the Gradio app will generate a link for accessing the interface. This link expires in 72 hours. After this period, you will need to execute the code again to generate a new link.






