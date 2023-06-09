# Instagram-image-color-tone-classification
* Developed a CNN model based on the AlexNet architecture to classify instagram images of hospitality brands into 4 different classification label based on the color tone used on the image. These includes: *warm tone, cool tone, low-key tone, high-key tone*
* This is an application of color tone in marketing field. Through the deep_learning model, I explored how hospitality brands use the concept of  color psychology in their Instagram images. 


## Code and Resources Used 
**Python**  
**Packages:** pandas, numpy, pytorch, sklearn, matplotlib, OS, time 

## Dataset
Datasets were downloaded from flickr. classified as the following:
*	Warm tone
*	Cool tone
*	High-key tone
*	Low-key tone 

<img src="https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/1ea36546-3ecf-4404-970c-e7614e2132b2" alt="warm tone image" width="200" height="200">
<img src="https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/b9463d9d-3ce0-46d0-8919-2beb8176a1c6" alt="warm tone image" width="200" height="200">
<img src="https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/751963a4-a00d-4f47-96fc-c0c07ccc7ff4" alt="warm tone image" width="200" height="200">
<img src="https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/73c12259-7196-4f45-aa97-782a7c90f042" width="200" height="200">

## CNN Model Architecture
Implementation of the AlexNet architecture

<img src="https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/42ce56e3-0946-4069-bb1f-2e842ed9945a" alt="model architecture" width="950" height="350">

## Model Training 
* Transfer Learning --> AlexNet pre-trained model and its learned parameters
* learned parameter values --> initial values and then fine-tuned to train the model
* learning rate set at **0.0001**. 


## Model performance
The Random Forest model far outperformed the other approaches on the test and validation sets. 
*	**Prediction Accuracy** = 0.92
*	**F1-Score** = 0.92
*	**AUC-score** = 0.99

<img src="https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/f4ec7b7d-555b-48b4-884a-d0bc5cbbd012" width="200" height="200">
<img src="https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/a16c4e48-f46e-4418-a105-635ad266097c" width="200" height="200">
<img src="https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/97aca562-b4d3-4d35-a739-bdf5adc75fe9" width="200" height="200">

