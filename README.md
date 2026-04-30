# OC_P6_text_and_image_to_vector, classification of consumer goods
TF-idf vectorizer, NLP, CNN, Doc2Vec, VGG16, Transfer Learning, Keras (Tensorflow)

You are a data scientist at a company that wants to launch an e-commerce marketplace: sellers offer items to buyers by posting a photo and a description. Currently, sellers manually assign categories to items, which makes the process unreliable. Additionally, the volume of items is currently very small. To make the user experience as seamless as possible for both sellers (by making it easier to list new items) and buyers (by making it easier to search for products), and with a view to scaling up, it has become necessary to automate this task.

You are asked to study the feasibility of a system for classifying items into different categories with a sufficient level of accuracy. Your task is to conduct, in an initial iteration, a feasibility study for an article classification engine, based on an image and a description, to automate the assignment of article categories.

You must analyze the textual descriptions and images of the products through the following steps: 
Preprocessing of text or image data, as applicable;
Feature extraction;
Reduction to two dimensions, in order to plot the products on a 2D graph as points whose color corresponds to the actual category;
Analysis of the graph to determine, using the descriptions or images, whether it is feasible to automatically group products of the same category;
Conducting a measurement to confirm your visual analysis by calculating the similarity between the actual categories and the categories resulting from cluster segmentation.
Demonstrate, using this approach, the feasibility of automatically grouping products of the same category

To extract text features, you will need to implement: 
two “bag-of-words” approaches: simple word counting and TF-IDF;
a classic word/sentence embedding approach using Word2Vec (or Glove or FastText);
a word/sentence embedding approach using BERT;
a word/sentence embedding approach using USE (Universal Sentence Encoder). 

To extract image features, you will need to implement:
a SIFT/ORB/SURF-type algorithm;
a CNN Transfer Learning-type algorithm.

Data is provided by the university.
There are no intellectual property restrictions on the data or images.

## Assessment Criteria
### Preprocess text data to obtain a usable dataset.
Clean the text fields (removing punctuation and filler words, converting to lowercase).
Write a function to “tokenize” a sentence.
Write a function to “stem” a sentence.
Write a function to “lemmatize” a sentence.
Build bag-of-words features (standard bag-of-words: word counting and TF-IDF), with additional cleaning steps: word frequency threshold, word normalization.
Test a sentence or a short example text to demonstrate the successful completion of the previous 5 steps.
In addition to the “bag-of-words” approach, implement 3 word/sentence embedding methods: Word2Vec (or Doc2Vec or Glove or FastText), BERT, and USE (Universal Sentence Encoder).
Ensure that the processed text does not constitute intellectual property whose use or modification is prohibited.

### Preprocess image data to obtain a usable dataset.
Use specialized libraries for initial contrast processing (e.g., OpenCV). 
Demonstrate image post-processing operations (e.g., grayscaling, noise filtering, equalization, blurring) on one or more examples. 
Develop a function to extract “bag-of-images” features via descriptor generation (ORB, SIFT, or SURF algorithms). 
Develop and execute a function to extract features (“feature engineering”) using a transfer learning algorithm based on neural networks, such as CNN. 
Ensure that the images used do not infringe on any intellectual property rights.

### Apply dimension reduction techniques.
Justify the need for dimension reduction. 
Apply a dimension reduction method appropriate to the problem (e.g., PCA). 
Justify the choice of parameter values in the selected dimension reduction method (e.g., the number of dimensions retained for PCA).

### Visually represent high-dimensional data.
Implement at least one dimension reduction technique (using LDA, PCA, T-SNE, UMAP, or another technique).
Create at least one graph representing the data reduced to 2D (for example, displaying the two components of T-SNE).
Conduct and document an analysis of the 2D graph.

### Evaluate the performance of deep learning models based on various criteria (scores, training time, etc.) in order to select the model that performs best for the business problem.
Select a metric appropriate for the business problem, which is used to evaluate the performance of the models 
Explain the choice of evaluation metric 
Evaluate the performance of a baseline model and used it as a benchmark to assess the performance of more complex models 
In addition to the chosen metric, you calculate at least one other indicator to compare the models (for example: the time required to train the model) 
Optimize at least one of the hyperparameters of the chosen model (e.g., choice of loss function, batch size, number of epochs) 
Present a comparative summary of the different models, for example in the form of a table. 

### Use data augmentation techniques to improve model performance.
Use several data augmentation techniques (e.g., for images: rotation, scaling, adding noise, etc.). 
Present a comparative summary of performance improvements achieved through the various data augmentation techniques used (control of overfitting, better score).
