# Scoliosis Detection   
  
- The project aim's to identify the patients who is having Scoliosis in their Early Stage   
- With the help of sample data present in the **folder 224** and has 2 subfolders with images of Normal human spine and person with Scoliosis - Train & Test Data   
- The Main code for the Model Training is in the file **scoliosis-detection-using-cnns.ipynb**   
- The Architecture of Model :   
  **model = Sequential()  
  model.add(Conv2D(32, (3,3), input_shape=(img_size,img_size,1), activation = 'relu', padding='same'))   
  model.add(MaxPooling2D())   
  model.add(Conv2D(64, (3,3),activation = 'relu', padding='same'))  
  model.add(MaxPooling2D())   
  model.add(Conv2D(128, (3,3), activation = 'relu', padding='same'))   
  model.add(MaxPooling2D())   
  model.add(Flatten())   
  model.add(Dense(512, activation='relu'))  
  model.add(Dense(1, activation = 'sigmoid'))**  
![image](https://github.com/user-attachments/assets/4fdc282f-9204-475a-bc4a-fefb6efd7392)   

## The Pre-Processing  
- The file **ProcessingImages.ipynb** has the image processing filters to get more depth and sharpness of the original x-rays of patients for having more detailed and optimized output   
- The preprocessing requires because the original x-ray images may contains Noise and blurry inorder to overcome them we have done Gaussian Blur, Median-Filter, Sharpening the image, Equalizing the image  
- The Output of Above preprocessed images are stored in another folder **processed_images** 
- Again these processed images are given to model and the results are avaluated

Here the conclusion is the Original images are trained and tested with the model and the same model trained and tested by thr processed Images - The Efficiency has been improved and Optimization can be acheived!



