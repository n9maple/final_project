# Model Reproducing steps

This project are tested on Google colab, and it is strongly recommened to use Google colab as the work environment since the following steps are based on it. These steps may need modification to successfully run the code on the other environments.

## Requirements

The requirements.txt is attached on this project. In Google colab, you can install certain version package by runnin the code:
```ddd
!pip install package==x.x.x
```
You should replace 'package' with package name and x.x.x with the version.

Now let's start.

First, create a folder in your Google drive and put train.csv and test.csv in it.
![](https://i.imgur.com/zCgEdle.jpg)
![](https://i.imgur.com/qcql2Qm.jpg)

Second, please modify the path name in "both" 109550095_Final_inference.ipynb and 109550095_Final_train.ipynb. The path string is in the second block counted from the top, and you only need to modify where red arrow points to the name of your folder (In this example, 'ML_final')
![](https://i.imgur.com/Ddezz5n.jpg)

## Training

Run all the blocks in 109550095_Final_train.ipynb. After running, you should see an model file named 'final_model' in the folder you create.
![](https://i.imgur.com/yDGxAIy.jpg)

## Prediction

Run all the blocks in 109550095_Final_inference.ipynb. After running, you should see an csv file named 'output.csv' in the folder you create.
![](https://i.imgur.com/HLzfuHl.jpg)

## Evaluation

To evaluate my model on Kaggle, enter the following website, sign in Kaggle, and join the competition below:
https://www.kaggle.com/competitions/tabular-playground-series-aug-2022/leaderboard

After you join the competition, you should see "Late Submission" bottom. Click it and submit 'output.csv' to it.
![](https://i.imgur.com/QchSVOB.jpg)
![](https://i.imgur.com/gFZc2Ph.jpg)




## Pre-trained Models

The pre-trained model named "final_model" can be accessed via link:https://drive.google.com/drive/folders/1CR-N9encIodLJ7SmQiexBP9y4-LZohhr?usp=sharing. Notice that this model is saved with 'joblib' package of python, so it's not guarantee the model can be successfully load with other package. In addition, with the pre-trained model, the trainning step can be skiped, but the trainning data (train.csv) is still needee because it will be used in data preprocessing.
![](https://i.imgur.com/g4m5wnp.jpg)

## Results

If the submission succeeds, the score should be exactly the same as the below:
![](https://i.imgur.com/EyC8gZs.jpg)


## Contributing

[1] ZJY27, “TPS-Aug22 9th solution” September, 2022. [Online]. 
Available: https://www.kaggle.com/code/takanashihumbert/tps-aug22-9th-solution/notebook [Accessed Jan. 8, 2023].

[2] KAUSHIK as writer, VK as translator, “KNNImputer：一种可靠的缺失值插补方法” July 28, 2020. [Online].
Available: https://www.cnblogs.com/panchuangai/p/13390354.html [Accessed Jan. 8, 2023].

[3] Ben Hu,” （機器學習）可解釋性(2) Permutation Importance” February 2,2020. [Online].
Available: https://medium.com/@hupinwei/%E6%A9%9F%E5%99%A8%E5%AD%B8%E7%BF%92-%E5%8F%AF%E8%A7%A3%E9%87%8B%E6%80%A7-machine-learning-explainability-%E7%AC%AC%E4%BA%8C%E8%AC%9B-c090149f0772 [Accessed Jan. 8, 2023].
