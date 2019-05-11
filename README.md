# Closed-Set-Face-Recognition

Face Recognition has many applications ranging from small level attendance systems, home surveillance to large country level surveillance system as implemented for China’s Social credit system.


For face detection – Haar Cascades from OpenCV is used
For face Recognition – Vgg19 is used.

DATA: A custom dataset is created based on images from the internet of few celebrities and few of my images and my partner’s.

VGG19 model is pretrained on VGGface dataset.  The last layers are removed and new layers are added in accordance with the custom dataset. Then the model is trained for around 100 epochs. The trained model is used for real time face recognition.
OpenCV enables us to capture real time video and it is then sent frame by frame to first face detector, which then crops the detected face from original image to VGG19. VGG19 classifies the detected face. The only problem with this model is that if a new identity is added to the database , whole network has to be trained again which takes a lot of computing power and time.
