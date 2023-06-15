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
*	Low-key tone
*	High-key tone 

![warm_tone](https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/1ea36546-3ecf-4404-970c-e7614e2132b2)
![cool_tone](https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/b9463d9d-3ce0-46d0-8919-2beb8176a1c6)
![high_key](https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/751963a4-a00d-4f47-96fc-c0c07ccc7ff4)
![low_key](https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/73c12259-7196-4f45-aa97-782a7c90f042)

<img src="https://github.com/Khlement/Instagram-image-color-tone-classification/assets/87413037/1ea36546-3ecf-4404-970c-e7614e2132b2" alt="warm tone image" width="250" height="250">
## Model Building 

First, I transformed the categorical variables into dummy variables. I also split the data into train and tests sets with a test size of 20%.   

I tried three different models and evaluated them using Mean Absolute Error. I chose MAE because it is relatively easy to interpret and outliers aren’t particularly bad in for this type of model.   

I tried three different models:
*	**Multiple Linear Regression** – Baseline for the model
*	**Lasso Regression** – Because of the sparse data from the many categorical variables, I thought a normalized regression like lasso would be effective.
*	**Random Forest** – Again, with the sparsity associated with the data, I thought that this would be a good fit. 

## Model performance
The Random Forest model far outperformed the other approaches on the test and validation sets. 
*	**Random Forest** : MAE = 11.22
*	**Linear Regression**: MAE = 18.86
*	**Ridge Regression**: MAE = 19.67

## Productionization 
In this step, I built a flask API endpoint that was hosted on a local webserver by following along with the TDS tutorial in the reference section above. The API endpoint takes in a request with a list of values from a job listing and returns an estimated salary.
