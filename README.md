# Document-Classification-and-Data-Extraction
We put out a model that can recognise the collection of papers contained in a pdf or image made up of numerous documents. To accomplish this, the input PDF is divided into individual pages. The CNN model is used to categorise each page into the appropriate document category. After that, each document's data is extracted using OCR (optical character recognition). This is being recommended for five documents: voter identification, driver's licence, PAN, and Aadhar.
Except for the front and back of the same document, the input pdf must include a single document on a single page.
Our data classification model obtained 0.7342 accuracy on the training set and 0.7736 accuracy on the validation set, with gains of 0.6923 and losses of 0.8340.
