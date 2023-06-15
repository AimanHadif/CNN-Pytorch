# Intel Image Classification Dataset Using PyTorch
- Image classification using CNN PyTorch format of Intel Image Classification dataset
- Link to Dataset : https://www.kaggle.com/datasets/puneet6060/intel-image-classification
- The model achieved a training accuracy of 98.76% and a testing accuracy of 79.50% without doing any parameter tuning

## The Dataset Information
- Consist of image data of Natural Scenes around the world.
- This Data contains around 25k images of size 150x150 distributed under 6 categories.
1. Buildings
<img src="example-images/building.jpg" alt="building" width="100">
     
2. Forest
<img src="example-images/forest.jpg" alt="forest" width="100">
     
3. Glacier
<img src="example-images/glacier.jpg" alt="glacier" width="100">
     
4. Mountain
<img src="example-images/mountain.jpg" alt="mountain" width="100">
     
5. Sea
<img src="example-images/sea.jpg" alt="sea" width="100">

6. Street
<img src="example-images/street.jpg" alt="street" width="100">   

## Training Results
- The settings of the image size can be tuned depending on your experiments
- This code takes the image into 224x224 size image
<img src="example-images/accuracy graph.png" alt="acc" width="500">

1. Training Accuracy
<img src="example-images/training results.png" alt="train" width="600">

2. Testing Acccuracy
<img src="example-images/loss graph.png" alt="test" width="500">

## Testing Results
- Inference was done using the Intel_CNN_Inference.ipynb script in this repo
- There are 2 options to output the inference
  > Pie Chart </br>
  > Bar Plot
- There are also 2 preprocessing in the test folder which are
   > Masking the Image </br>
   > Unmasking the Image (normal)
- Refer to https://github.com/AimanHadif/Image-Masking for details on Masked Image
- Example output will produce the file for class and the each image predicted in the class, the visualization (pie/bar), and csv file of the filename and the predicted label
  
<img src="example-images/example output.png" alt="output" width="800">

1. Pie w/ Mask
<img src="example-images/pie mask.png" alt="pie" width="300">   
2. Pie w/o Mask
<img src="example-images/pie no mask.png" alt="pie no mask" width="300">   
3. Pie (Both Mask and No Mask)
<img src="example-images/pie both.png" alt="pie both" width="600">   
4. Bar w/ Mask
<img src="example-images/bar mask.png" alt="bar mask" width="300">   
5. Bar (Both Mask and No Mask)
<img src="example-images/bar both.png" alt="bar both" width="600">    

## Error
- There should not be any error unless you've changed the input size, and the number of class. If that is the case then refer back to the CNN architecture to adjust the output number and the image size on the final layer
- If you found any error while implementing this code with different datasets. Please understand the code completely especially in the inference script
- If the error is still unsolvalbe, feel free to reach me
