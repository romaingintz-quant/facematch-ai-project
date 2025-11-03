# FaceMatch
Face recognition using a Siamese neural network

## Project Description

This project aims to develop a face recognition system for age verification using the OpenFace model and DeepFace library. The system compares a captured image with a database of known individuals to determine a match and estimate the age of the identified person. If the person is of legal drinking age (18 or older), a thumbs-up image is displayed; otherwise, a thumbs-down image is shown.

## Project Team

- GINTZ Romain - ETIEVANT Thomas - HUCK Alban - BRUN Karl - WERNER Valentin
  
- For Mr. REHEISSER

## How to Run the Code

This project is implemented in Google Colab and requires access to the associated Google Drive account for data storage.

**Prerequisites:**

- Google Colab account : projetinfo2025@gmail.com	password : INFOPROJET2025!
- Google Drive account with access to the shared project folder (same account as the Google Colab one)

**Steps:**

1. **Access Google Colab:** You have to click on the FaceMatchFinal.ipynb file in the github and click on "open in colab". You will then have access to the whole code divided in three cells. WARNING : You have to be log in on google colab and on google drive with the account provided and not your personal one.
   
2. **Install DeepFace:** Run the first code cell that installs the DeepFace library. This library is used for face recognition tasks.
   
3. **Mount Google Drive:** Run the second code cell that mounts your Google Drive to the Colab environment. This allows the notebook to access the database images and captured image.
   
4. **Test the code:** Run the third cell in order to get your result, if a match is found, the code displays the matched person's name, age, and a thumbs-up or thumbs-down image based on their age. If no match is found, a message is displayed, and the captured image is shown. This step may take a while.
   
5. **Further testing:** If you want to try the code with other captured images (the trombinoscope stays the same) you will have to open the google drive with the projetinfo2025 account. Right after going to "MyDrive" you will see a folder "proim" that you have to open, then you can access the "cam" folder. You will find an image named "imagecam.jpg" that is the image currently tested and a folder "images de test". If you want to try another image, put the current "imagecam.jpg" in the folder and take another (the one you want to test) "imagecam.jpg" from the folder "images de test" and put it back inside the "cam" folder. Refresh the google drive page and run the code again. If it doesn't work, you might to refresh the whole google colab notebook and run again all the cells.  


**Code Structure:**

- `load_database_images_paths()`: Loads database images and their paths.
- `calculate_age()`: Calculates age from a birthdate string.
- `compare_with_database_openface()`: Compares the captured image with the database using OpenFace.

## Important Notes:

- The database of faces is stored in the Google Drive folder specified by '/content/drive/MyDrive/proim/trombi'.
- The captured image is located at the path specified by '/content/drive/MyDrive/proim/cam/imagecam.jpg'.

## In case of problems or anything, please send us an email.
