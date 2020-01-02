# tomato_prediction
This files detects the existence of tomato in the picture. For that, we used libraries as tensorflow, matplotlib, numpy. 7
We used colab for gpu. In the below, we will explain the structure of the file. 
It takes images from the drive mounted locally on colab, train the model and predict if there are tomato in the picture. For that, we develop the following methods:  
-	Extract_file : unzip .zip files mounted on colab
-	Read csv_file : read the .csv files et get all classes that contains tomato 
-	Read_json_file: reads the .json files and loads all images that contains tomato for training
-	Parse_function : parse every image in the dataset using map 
-	AlexNet : define the model alexNet 
-	Train(): in this function, we create dataset returning slices of filenames, compile alexnet model, train it and save it 
-	draw_acc_loss : draw the accuracy and the loss curve 
-	has_tomato : it takes the trained model and the test image and return the predicted class
For training, we first prepare the dataset (images with labels) and after we train the model 
For testing, we load the saved model and we return the predicted class: 1 if it contains tomato and 0 for none. 


