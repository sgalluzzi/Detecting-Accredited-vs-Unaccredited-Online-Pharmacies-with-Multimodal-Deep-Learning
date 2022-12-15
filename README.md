## Detecting Accredited & Non-Accredited Online Pharmacies with Deep Learning

### Abstract
The objective of this study was to harness neural networks to solve the rampant problem of non-accredited online pharmacies performing unapproved sales of drugs. A BERT model and MobileNetV2 model were used to classify the text and images of online pharmacies as accredited and non-accredited. Both models achieved moderately high accuracy on the validation datasets, with the BERT model at 90% and the MobileNetV2 model at 87% accuracy. Future work using a MultiModal model is recommended to combine the image and text models for improved overall accuracy.

### Motivation
The National Association of Boards of Pharmacy claims that 96% of all online pharmacies are illegitimate. Currently, the process of verifying legitimacy is manual and slow. In order to flag suspicious online pharmacies that may be selling unsafe medications, it is necessary to create an automated process that can detect whether an online pharmacy is accredited or not. There has yet to be a Deep Learning study that identifies non-accredited pharmaceutical websites. Our study is the first to train complex neural networks to detect accredited and non-accredited pharmaceutical websites.

### Methodology
Our custom dataset includes web-scraped content from the home pages of 72 known accredited and non-accredited pharmacies. 

Below are the notebooks, datasets, models, and results:

* [Webscraping online pharmacies, parsing data, & building datasets](https://github.com/HaleyEgan/Detecting-Accredited-vs-Unaccredited-Online-Pharmacies-with-Multimodal-Deep-Learning/blob/main/WebScrape_ToDatafame_AllPharmacies.ipynb)

* [Datasets](https://github.com/HaleyEgan/Detecting-Accredited-vs-Unaccredited-Online-Pharmacies-with-Multimodal-Deep-Learning/tree/main/Datasets)

* [Text preprocessing & BERT model](https://github.com/HaleyEgan/Detecting-Accredited-vs-Unaccredited-Online-Pharmacies-with-Multimodal-Deep-Learning/blob/main/BERTModel_Final.ipynb)

* [Image preprocessing & MobileNetV2 model](https://github.com/HaleyEgan/Detecting-Accredited-vs-Unaccredited-Online-Pharmacies-with-Multimodal-Deep-Learning/blob/main/mobilenetv2-img-classification.ipynb)
    * [Testing & Selecting the best image model](https://github.com/HaleyEgan/Detecting-Accredited-vs-Unaccredited-Online-Pharmacies-with-Multimodal-Deep-Learning/blob/main/IMG_classification_model.ipynb)

* Literature & Reporting:
    * [Project Proposal & Literature Review](https://github.com/HaleyEgan/Detecting-Accredited-vs-Unaccredited-Online-Pharmacies-with-Multimodal-Deep-Learning/blob/main/Reports/Detecting%20Accredited%20vs%20Non-accredited%20Online%20Pharmacies%20with%20Multimodal%20Deep%20Learning.pdf) 
    * [Model Design & Implementation](https://github.com/HaleyEgan/Detecting-Accredited-vs-Unaccredited-Online-Pharmacies-with-Multimodal-Deep-Learning/blob/main/Reports/DS%206050%20Milestone%202%20-%20Model%20Design%20and%20Implementation%20-%20Group%2013.pdf)
    * [Final Report & Results](https://github.com/HaleyEgan/Detecting-Accredited-vs-Unaccredited-Online-Pharmacies-with-Multimodal-Deep-Learning/blob/main/Reports/DS%206050_Group%2013_Final%20Paper.pdf)

### Model Performance
BERT Model Performance
![BERTModel](https://github.com/HaleyEgan/Detecting-Accredited-vs-Unaccredited-Online-Pharmacies-with-Multimodal-Deep-Learning/blob/main/plots/BERTModelResults.png)

MobileNetV2 Model Performance

<img src="https://github.com/HaleyEgan/Detecting-Accredited-vs-Unaccredited-Online-Pharmacies-with-Multimodal-Deep-Learning/blob/main/plots/MobileNetResults.png" width="300" height="300" />

### Future Work
We recommend concatenating the image and text models with a MultliModal Model for a more comprehensive approach to classifying pharmacy website content as a whole. 
