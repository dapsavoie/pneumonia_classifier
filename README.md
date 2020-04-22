# Pneumonia Classifier

![image](https://github.com/dapsavoie/pneumonia_classifier/blob/master/jZqpV51%20(1).png)

This project requires creating an image classifier that identifies pneumonia in patients. 

The best performing model contains data that was augmented in the normal category and added to a file called normal_aug.

This augmented was data was then tested on the best performing model. It improved recall score by 6% to 86% with 97% accuracy.

This indicates that class balancing improved the output. However, further work is needed to prevent false negatives.

# Conclusion

The best peforming model is a multi layered keras sequential model with a relu activation function. The model includes conv2d layers, max pooling, and a binary cross-entropy loss function. I also added dense and dropout layers to improve the final performance. In addition, an additional 2540 images were added by augmenting the normal images. As target classes were imbalanced towards pneumonia, balancing them proved key to improving the final recall score.

# Next Steps & Recommendations

Configure results of model to deliver a probability ranking to medical imaging experts. The highest probability cases can then be viewed quickly and assesed by a professional to reduce risk to patients. This could be used to speed up triage in times of need where medical imaging professionals are lacking. 

In order to improve the model, clearer images of normal lungs should be generated and augmentation processes used above should be reviewed. Further review of misclassified false negatives is also needed.


