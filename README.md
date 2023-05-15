# Natural-Scene-Neural-Encoding

Predicting fMRI responses from the natural scene images.

Linearizing encoding approach: Images --> nonlinear feature extraction --> linear mapping(linear regression) --> fMRI

We experimented with several nonlinear feature extraction methods:
- AlexNet (Provided in the tutorial)
- ResNet 50 (Yixiao)
- ResNext 101 (Yixiao)
- ResNest 50 (Yixiao)
- VAE (Wenshuo)
- ResNet 50 & AlexNet mixture (Wenshuo) 

To run the jupyter notebook:
1. Get Natural Scene Dataset here: https://docs.google.com/forms/d/e/1FAIpQLSehZkqZOUNk18uTjRTuLj7UYmRGz-OkdsU25AyO3Wm6iAb0VA/viewform
2. Upload the notebooks and the dataset to BC GPU machine to get enough memory 
3. Put the subject folders ("subj01" / "subj02" / "subj03" ...) and the notebooks under the same directory
4. The notebook code can only run on one subject each time, select the subject id you want to run in the second code block (eg:"subj = 1" or "subj = 2" etc.)
5. Run the notebook

To visualize ResNext result, put ResNext.ipynb and Res_Next_Result.ipynb under the same directory, then run ResNext.ipynb and run Res_Next_Result.ipynb
To run VAE_implemented.ipynb, download the pretrained model parameters here: https://www.kaggle.com/code/maunish/training-vae-on-imagenet-pytorch/output

Results(for subj 01):
- ResNet 50 & AlexNet mixture has our best results so far:
![image](https://github.com/qinwenshuo/Natural-Scene-Neural-Encoding/assets/53549553/72d993ff-e212-4cac-9ac9-a674ca7b405c)

- RestNet 50:
![image](https://github.com/qinwenshuo/Natural-Scene-Neural-Encoding/assets/53549553/a3106938-4f4f-450b-b67d-8c10c907dcb1)

- ResNext 101
![image](https://github.com/qinwenshuo/Natural-Scene-Neural-Encoding/assets/53549553/cd8326ac-5a89-4e1c-a650-b3b0b9154a14)

- ResNest 50
![image](https://github.com/qinwenshuo/Natural-Scene-Neural-Encoding/assets/53549553/9726ff46-d9e7-45db-8b38-2b0b0f84dc9f)

- AlexNet
![image](https://github.com/qinwenshuo/Natural-Scene-Neural-Encoding/assets/53549553/df3a7398-99a7-46ab-ad19-b2d73b04883b)

- VAE
![image](https://github.com/qinwenshuo/Natural-Scene-Neural-Encoding/assets/53549553/f56c344a-8ea6-424c-b844-be2e7b6d9f7f)
