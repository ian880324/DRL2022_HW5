# 2022_DRL
# 2022.06.01 Update MountainCar-v0
## 1. Setup Environment (安裝必要的環境資源)
- !apt-get install -y xvfb
- !pip install gym==0.21 gym[box2d] pytorch-lightning==1.6.0 pyvirtualdisplay
## 2. Create the Deep Q-Network
- nn.Linear(in_features,out_features,bias=True): 是Pytorch中用來設置全連接層的寫法。in_features=輸入的二維的SIZE，out_features=輸出的二維的SIZE。
- nn.ReLU(): 一種激活函數。
## 3. Create the policy
- 本篇是使用Random Policy。
# 以下是訓練過程以及最終成果
- epoch 0


https://user-images.githubusercontent.com/62320138/171365922-2615aa74-84c1-4b90-a181-5b8289e75458.mp4


- epoch 100


https://user-images.githubusercontent.com/62320138/171366013-ca44bc77-54e7-49f8-a699-346cabcc2ec9.mp4


- epoch 1500


https://user-images.githubusercontent.com/62320138/171365214-e1a5b699-26e5-4367-819e-06e56a8e99fb.mp4


