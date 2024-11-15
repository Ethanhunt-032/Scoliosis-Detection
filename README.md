# Scoliosis Detection
In this project we will identify the patients who is having Scoliosis by Training the model with the help of sample tain data present in the **folder 224** 
Folder 224 has 2 subfolders with images of Normal human spine and person with Scoliosis - Train & Test Data
The Main code for the Model Training is in the file **scoliosis-detection-using-cnns.ipynb**
The Architecture of Model :
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


