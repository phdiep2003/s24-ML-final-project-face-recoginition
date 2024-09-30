# s24-ML-final-project-face-recoginition
# Nationality Face Recoginition in Images using Machine Learning  
**By Phat Diep (phdiep) and Sangyoon Lim (sangyoon)**  

## Abstract/Problem Specification  
This project aims to explore the feasibility and accuracy of classifying individuals' nationalities using Machine Learning models (such as convolutional neural networks). The prevailing models for facial recognition are dominated by Westerners, while Asians are underrepresented, resulting in lesser accuracy in recognizing people of Asian heritage than their Western counterparts (Xiong et al., 2019). Moreover, Asian people represented in such datasets are not distinguished by nationality, which leads to a great loss of data for the development and deployment of country-related applications for Asians.  
The purpose of this research is to provide answers to issues about the efficacy of machine learning models in this kind of categorization work, the morality of putting such a system in place, and the possible uses and consequences of this technology.

**Keywords**: CNN, Classification, Asian face dataset, Racial bias.

## Project Idea  
Our project will involve building a Query Analysis Model (QuAM) that utilizes a classification approach to identify the nationality of individuals in images, especially differentiating between Asians. The model will be designed to recognize and analyze specific, non-sensitive features that can be associated with different nationalities. The interface will allow users to upload an image, and the system will then provide a prediction of the nationality or nationalities represented, along with a confidence score for each prediction.

## Dataset Overview (Preliminary)  
- A `.zip` of female Asian images, each nationality represented by over 700 images.
- A `.csv` file to record the label of the image based on nationality.

**Figure 1**: Image data for classification (left: Korean 026.jpg, right: Chinese 006.jpg).

## Methodology  

### Data Collection  
- **Use serpapi** (Google search API) to scrape the data from Google Images.  
  *Phat* (to be completed by Apr 5).

### Data Preprocessing  
- Use a short CNN classification to filter out AI-generated or inappropriate images (only ID-type, face-only, no body, no obstacles, etc.).
- Resize images to build convolutional layers.  
  *Sangyoon* (Apr 10).

### Model Development  
We will develop machine learning models: K-NN and CNN neural networks, inspect and visualize the activations from the layers, and relate them to feature extraction (epochs, softmax).  
- X ~ Image Features (grayscale, HOC, Laplacian, SIFT, etc.)  
  *Phat* (Apr 14), *Sangyoon* (Apr 16) extracting features and visualizations.  
- Y ~ Nationality: 1. Korean (collected), 2. Chinese (collected), 3. Vietnamese (NaN), etc.

### Model Training and Evaluation  
- Train models on a subset of the dataset and evaluate using cross-validation techniques to ensure generalization to unseen data.
- Assess performance using evaluation metrics (confusion matrix, accuracy, precision, f1-score).  
  *Phat and Sangyoon* (Apr 17) to sit together and reassess and improve the process.

### Model Optimization  
- Fine-tune features to improve performance using gradient descent to detect subtle facial differences.  
  *Phat* (improve feature extraction), *Sangyoon* (model training).

## Thank you  
Thank you for considering our project proposal. We look forward to contributing to the advancement of neural networks for face recognition.

### Image Data  
[Data Link](https://drive.google.com/file/d/1hVRjKoA8KjtTNNMhFgI0c80fYA8Aw-AM/view?usp=sharing)

### Reference  
Xiong, Z., Wang, Z., Du, C., Zhu, R., Xiao, J., & Lu, T. (2018). An Asian face dataset and how race influences face recognition. In *Advances in Multimedia Information Processing–PCM 2018: 19th Pacific-Rim Conference on Multimedia, Hefei, China, September 21-22, 2018, Proceedings, Part II 19* (pp. 372-383). Springer International Publishing.
