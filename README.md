## Document-Classification-and-Data-Extraction


   
<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
       <li>
      <a href="#salient-features">Salient Features</a></li>
      <li>
      <a href="#description">Description</a>
      <li>
      <a href="#data-preprocessing">Data Preprocessing</a></li>
      <li>
      <a href="#Document Classification Model">Document Classification Model</a></li>
      <li>
      <a href="#results">Results</a>
      <li>
      <a href="#Information extraction model">Information extraction model</a>
      <li>
      <a href="#team">Team</a>
    </li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About the project
We put out a model that can recognise the collection of papers contained in a pdf or image made up of numerous documents. To accomplish this, the input PDF is divided into individual pages. The CNN model is used to categorise each page into the appropriate document category. After that, each document's data is extracted using OCR (optical character recognition). This is being recommended for five documents: voter identification, driver's licence, PAN, and Aadhar.
Except for the front and back of the same document, the input pdf must include a single document on a single page.
Our data classification model obtained 0.7342 accuracy on the training set and 0.7736 accuracy on the validation set, with gains of 0.6923 and losses of 0.8340.


### Salient Features
Hyperparameter tuning, regularization(early stopping), document split 
### Tech stack used
* models: CNN and OCR
* Framework-Keras 

### Methodology
<img width="500" alt="image" src="https://user-images.githubusercontent.com/87893594/224972918-d1e9f755-02e0-40c0-8725-ac5c4824d49a.png">

### Data Description 
When we began searching for an appropriate dataset, we observed that there is no publicly available dataset of identity documents as they hold sensitive and personal information. But we came across a dataset on Kaggle that consisted of six folders, i.e., Aadhar Card, PAN Card, Voter ID, single-page Gas Bill, Passport, and Driver's License.  We added a few more images to each folder. These were our own documents that we manually scanned, with the rest coming from Google Images.
Thus, these are the five documents we are classifying and extracting information from.



### Data Preprocessing
Before model training, we applied horizontal and vertical data augmentation using random flips. This further increased the size and diversity of the dataset. The categorical values of the labels column were converted to numerical values using one-hot encoding.


### Document Classification Model
<img width="555" alt="image" src="https://user-images.githubusercontent.com/87893594/224973161-2513f1f7-0291-41ed-9b79-c14ef2578882.png">

Various hyperparameters like the number of layers, neurons in each layer, number of filters, kernel size, value of p in dropout layers, number of epochs, batch size, etc. were changed until satisfactory training and validation accuracy was achieved.

<img width="500" alt="image" src="https://user-images.githubusercontent.com/87893594/224972235-be7435d0-1f11-4c38-8ab6-6958fcb3bb83.png">

<img width="500" alt="image" src="https://user-images.githubusercontent.com/87893594/224972374-4244b1b6-418d-4364-8fea-77a05450ca19.png">


### The final Model and results
<img width="500" alt="image" src="https://user-images.githubusercontent.com/87893594/224972133-8bf9642b-d16e-4880-b017-161c61d8f247.png">
<img width="500" alt="image" src="https://user-images.githubusercontent.com/87893594/224972187-cd7f5c48-95d7-42fa-a187-bfd84344e903.png">


### Information extraction model
Following are the steps of OCR done on images:

<img width="650" alt="image" src="https://user-images.githubusercontent.com/87893594/224973268-06a235f9-6657-4970-befc-78cf665bfb65.png">

<img width="650" alt="image" src="https://user-images.githubusercontent.com/87893594/224973311-0b5c26d3-46d4-4df8-96a3-c4287072637a.png">



### Team
- Kanika Kanojia [GitHub](https://github.com)        [Linkedin](https://www.linkedin.com/in/kanika-kanojia-348620207/) 
- Deepali Thakur [GitHub](https://github.com/deepalii05) [Linkedin](https://www.linkedin.com/in/deepali-thakur/)
- Princy Singhal [GitHub](https://github.com/PrincySinghal) [Linkedin](https://www.linkedin.com/in/princy-singhal-047414224/)
