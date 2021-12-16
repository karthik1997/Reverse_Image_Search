# Reverse_Image_Search
Ever wondered how the Google Image Search works…………………..? Well, It ain't any rocket science. The procedure Behind the screen is Reverse Image Search Algorithm. 
I have implemented a miniature version of the same with the help of classical ML and Deep Learning Techniques.
Tried the results with some real world data to check the robustness 

Picked up a  a pre-trained deep learning model (Resnet), remove the top layers, and extract the convolutional features for the images in our dataset. 
We used PCA to reduce the dimensionality of the extracted features so that we have a grip in the output.
Then we will use these feature vectors to find similar images by using sklearn nearest neighbor algorithm. The dataset that we used her is a subset of Caltech Dataset.Initially the algorithm is tried with Resnet convolutional features plus cosine similarity to find the best results, but got a good amount of false positives. So fixed with Resnet+PCA+KNN approach 

Dataset Link: http://www.vision.caltech.edu/Image_Datasets/Caltech101/101_ObjectCategories.tar.gz
