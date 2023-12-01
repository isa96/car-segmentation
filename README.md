# Self_Driving_Car_Segmentation

This project has 367 dataset, and I split the dataset into train and test (65% for train, and 35% for test). The architecture that I used in this project is Unet architecture.

**here's the architecture looks like**

![u-net-architecture](https://user-images.githubusercontent.com/91602612/165755054-caf78b8b-4909-44dd-ad0e-85089fe595e1.png)

## Load Image

In this phase I also normalize and resize the image
![Load Image](https://user-images.githubusercontent.com/91602612/165887759-2560408e-ed5c-460e-8ef5-7d63d62493ed.png)

Then show 3 samples of actual image and 3 samples of annotation/mask image
![Screenshot 2022-04-28 205259](https://user-images.githubusercontent.com/91602612/165887832-6e26b4ab-5994-4b84-9264-620e850a309e.png)
![Screenshot 2022-04-28 205313](https://user-images.githubusercontent.com/91602612/165887840-4f9253f0-9afd-4a61-bad7-dd9a7fec4552.png)

##  Preprocessing Image

After load the images, we split the dataset
![Screenshot 2022-04-28 205337](https://user-images.githubusercontent.com/91602612/165890623-d13ccc1a-b26a-44ee-99e8-9c55068c8b26.png)

Then use to_categorical modul to one hot the labels
![One hot encoding](https://user-images.githubusercontent.com/91602612/165890995-35e606e8-40e7-49be-87a6-80ca151104e8.png)
![Screenshot 2022-04-28 205410](https://user-images.githubusercontent.com/91602612/165890999-2673da40-c77a-4d5d-ba6e-a4b42093e8b2.png)

## Then we create an Unet model based on the architecture show above
![Screenshot 2022-04-28 205445](https://user-images.githubusercontent.com/91602612/165891082-926d6c66-53e5-4d69-bbf7-c11ccc6bd273.png)
![Screenshot 2022-04-28 205454](https://user-images.githubusercontent.com/91602612/165891092-e94a2c06-b0fc-43a4-9489-aad53799af51.png)


