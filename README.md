# Visual-Similarities-Images
Retrieving similar images from query based on its feature and similar color filter. This repo using two phase of processing. 

Short Description:
1. First, it uses VGG16 pre-trained model without last layer as predictions model. We modified the custom model which have the output "fc2" layer. 
2. Second, the custom model used to obtain all features vector from each images, then save them to list variable. 
3. Since it'll have very big size, we reduce its size without sacrifice important images feature using PCA reduction.
4. Finally, we query new image to calculate the similarity with every features of all image and add more filter images using K Means Clustering color filter. 


