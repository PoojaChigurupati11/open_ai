This code demonstrates how to use CLIP (Contrastive Language-Image Pre-training) to calculate cosine similarity scores between images and their associated captions. It also utilizes the zero-shot classification capability of the Hugging Face Transformers library to predict labels for the images based on their captions.

Prerequisites
Python 3.x

Install required libraries using the following commands:
pip install sentence_transformers
pip install torch
pip install transformers
pip install tqdm
pip install matplotlib

Usage
1. Set up the Environment
Update the image_folder_path variable to the path of the folder containing your images.
Update the caption_file_path variable to the path of the file containing image captions. The file should be in CSV format with the first column being the image names and the second column being the corresponding captions.
2. Extract Image and Text Embeddings
The code uses the CLIP model to encode images and captions into embeddings.
Run the first code block to obtain cosine similarity scores between images and their captions.
3. Predict Labels Using Zero-Shot Classification
The second code block utilizes the Hugging Face Transformers library for zero-shot classification.
The model facebook/bart-large-mnli is used for zero-shot classification.
The code predicts labels for each image based on its associated captions and displays the results.
4. Visualize Results
The results are visualized using Matplotlib. For each image, the predicted label and confidence score are displayed.
