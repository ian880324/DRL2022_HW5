# 2022_DRL
# 2022.06.01 Update MountainCar-v0
## 1. Setup Environment (安裝必要的環境資源)
- !apt-get install -y xvfb
- !pip install gym==0.21 gym[box2d] pytorch-lightning==1.6.0 pyvirtualdisplay
## 2. Create the Deep Q-Network
- nn.Linear(in_features,out_features,bias=True): 是Pytorch中用來設置全連接層的寫法。in_features=輸入的二維的SIZE，out_features=輸出的二維的SIZE
