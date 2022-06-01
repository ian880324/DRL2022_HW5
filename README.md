# 2022_DRL
# 2022.06.01 Update MountainCar-v0
## 1. Setup Environment (安裝必要的環境資源)
- !apt-get install -y xvfb
- !pip install gym==0.21 gym[box2d] pytorch-lightning==1.6.0 pyvirtualdisplay
## 2. Create the Deep Q-Network
- nn.Linear(in_features,out_features,bias=True): 是Pytorch中用來設置全連接層的寫法。in_features=輸入的二維的SIZE，out_features=輸出的二維的SIZE。
- nn.ReLU(): 一種激活函數。
## 3. Create the policy
- 本篇是使用Greedy Policy。
# MountainCar 環境介紹
參考: https://mathpretty.com/14172.html
- 這裡介紹一個 OpenAI 中的環境，MountainCar-v0。該環境是一輛汽車在一維軌道上，位於兩座「山」之間。目標是在右邊開車上山；然而，這輛車的引擎不夠強勁，無法一次性翻越這座山。因此，成功的唯一方法是 "來回驅動" 以積聚動力。
- 在 MountainCar-v0 環境中，action是離散值，有三個不同的選項，分別是0 表示「向左行駛」，1 表示「停止」，2 表示「向右行駛」。
- Observation由兩個值表示，分別是position, velocity，表示「小車當前的位置」和「小車當前的速度」。
- 關於position，最左側的位置為-1.2，最右側的值為0.6，谷底是-0.5。
- 關於velocity，向右側行駛速度為「正」，左側為「負」。這裡速度的取值為[-0.07, 0.07]。
# 以下是訓練過程以及最終成果
- epoch 0


https://user-images.githubusercontent.com/62320138/171365922-2615aa74-84c1-4b90-a181-5b8289e75458.mp4


- epoch 100


https://user-images.githubusercontent.com/62320138/171366013-ca44bc77-54e7-49f8-a699-346cabcc2ec9.mp4


- epoch 1500


https://user-images.githubusercontent.com/62320138/171365214-e1a5b699-26e5-4367-819e-06e56a8e99fb.mp4


