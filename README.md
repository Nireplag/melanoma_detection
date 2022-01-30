# melanoma_detection

##### Class: Computational Vision
##### Professor: Dr. Lucas Ferrari de Oliveira
##### Developed by: Gabriel Galperin (galperin@ufpr.br)
##### Program: Applied Artificial Inteligence specialization
##### University: Universidade Federal do Paraná (UFPR)

### Reason for the creation
> Have a hands-on approach on how we can develop a working model for a small unbalanced dataset of images. 

### Development methodology:
> Tensorflow was the adoptedframework for this development. 

> Usage of transfer learning weights from the IMAGENET dataset with the VGG16 to use the feature classification already determined. 
> Due the small amount of data to train the model, the ImageDataGenerator of Keras is being used to produce data augmentation and allow a better fit and avoid overfitting issues.

> Dropout layers were also added to avoid overfitting. 

> Initial weights and class weights were used to make unbalance issue less impating into model creation.


> Note:  Other methods of data augmentation were used and also image segmentation over region of interest, however those methods did not show a positive result and were removed from final model creation, but can be seen into file history of changes. 

### Results
> The model created exceded the developer expectations considering the amount of available data (45 negatives and 23 positives) and the usage of a base model that was not trained over skin related images. 


> The final metrics observed were: 


  Metrics     |    values
------------- | -------------
   Accuracy   |    0.714286
   Precision  |    1
   Recall     |    0.2
 Specificity  |    1
   F1 score   |    0.333333

### Future developments
> Use a differnet and large database related to skin issues to create a base model and than recerate model with same dataset to check if feature selection can be improved.

> Better select areas of interest (filter and mask creations) of the training data, avoiding the need of greated amount of data to define them.

> Create a web aplication to allow usage of teh model.

> Develop a smaller model that can be used in mobile devices

### Contacts:  
> Unfortunatelly github is not allowing the file to be made available due it size, therefore in case you wish to test in in you data feel free to contact the developer by email to request the .h5 file.

> validation sha256: fe84cbff9a20f25cb10acd1f39c55f3268aa99b5e0031c5b976fe8fb540636ab
