# Image_Captioning# Image-Captioning
Explaining Encoder and Decoder
Encoder:
![image](https://user-images.githubusercontent.com/102589680/174859064-8fb1029b-3251-41a0-90e6-819ec253e239.png)
  For Encoder we use VGG-16. VGG-16 is a convolutional neural network that is trained on more than a million images from the ImageNet database. The network is 50 layers deep and can classify images into 1000 object categories, such as keyboard, mouse, pencil, and many animals. As a result, the network has learned rich feature representations for a wide range of images. The network has an image input size of 224-by-224.
![image](https://user-images.githubusercontent.com/102589680/174859109-984399c0-4366-4666-b94c-44669006cddf.png)
Decode:
  For Decoder we use LSTM. Long Short-Term Memory (LSTM) networks are a modified version of recurrent neural networks, which makes it easier to remember past data in memory. The vanishing gradient problem of RNN is resolved here. LSTM is well-suited to classify, process and predict time series given time lags of unknown duration. It trains the model by using back-propagation
# Results

![image](https://user-images.githubusercontent.com/102589680/174859452-6c6dabab-f213-4600-9c73-911a1093c78e.png)

              ---------------------Actual---------------------
             startseq black dog and spotted dog are fighting endseq
 startseq black dog and tri-colored dog playing with each other on the road endseq 
 startseq black dog and white dog with brown spots are staring at each other in the street endseq 
 startseq two dogs of different breeds looking at each other on the road endseq 
          startseq two dogs on pavement moving toward each other endseq
              --------------------Predicted--------------------
          startseq two dogs play with each other in the grass endseq
          
![image](https://user-images.githubusercontent.com/102589680/174860032-ae4ea684-5c08-4de0-b3e0-df50f57fafef.png)
          
              ---------------------Actual--------------------- 
startseq little girl covered in paint sits in front of painted rainbow with her hands in bowl endseq
            startseq little girl is sitting in front of large painted rainbow endseq 
startseq small girl in the grass plays with fingerpaints in front of white canvas with rainbow on it endseq 
    startseq there is girl with pigtails sitting in front of rainbow painting endseq 
          startseq young girl with pigtails painting outside in the grass endseq
              --------------------Predicted-------------------- 
     startseq little girl in pink dress is lying on the side of the grass endseq
     
![image](https://user-images.githubusercontent.com/102589680/174860201-4ea83084-c433-47bd-9a27-f6181f26e5ca.png)

              ---------------------Actual--------------------- 
    startseq man in hat is displaying pictures next to skier in blue hat endseq
   startseq man skis past another man displaying paintings in the snow endseq 
  startseq person wearing skis looking at framed pictures set up in the snow endseq
   startseq skier looks at framed pictures in the snow next to trees endseq 
  startseq man on skis looking at artwork for sale in the snow endseq 
              --------------------Predicted--------------------
                  startseq two people are hiking up snowy mountain endseq

