# melanoma_detection

##### Class: Computational Vision
##### Professor: Dr. Lucas Ferrari de Oliveira
##### Developed by: Gabriel Galperin (galperin@ufpr.br)
##### Program: Applied Artificial Inteligence specialization
##### University: Universidade Federal do Paraná (UFPR)

### Reason for the creation
> Have a hands-on approach on how we can develop a working model for a small unbalanced dataset of images. 

### Development methodology:
> Usage of transfer learning weights from the IMAGENET dataset with the VGG16 to use the feature classification already determined. 
> Due the small amount of data to train the model, the ImageDataGenerator of Keras is being used to produce data augmentation and allow a better fit and avoid overfitting issues.
> Dropout layers were also added to avoid overfitting. 
> Initial weights and class weights were used to make unbalance issue less impating into model creation. 
> Note:  Other methods of data augmentation were used and also image segmentation over region of interest, however those methods did not show a positive result and were removed from final model creation, but can be seen into file history of changes. 

### Results
> The model created exceded the developer expectations considering the amount of available data (45 negatives and 23 positives) and the usage of a base model that was not trained over skin related images. 
> The final metrics observed were: 
Metric          Value
-----------  --------
Accuracy     0.714286
Precision    1
Recall       0.2
Specificity  1
F1 score     0.333333
