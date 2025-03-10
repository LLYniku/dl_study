# dl_study

今天使用torch>2的版本和d2l1.0.3版本构建了一个MNIST物件识别，使用的学习率算法是2024 NeurIPS会议上的算法Less Scheduled。
Less Scheduled的学习率算法，避免了时间表，在从凸问题到大规模深度学习问题等一系列问题上，与时间表相比，表现出最先进的性能，与带动量的标准优化器相比，无时间表方法没有引入额外的超参数。
## 环境配置

torch > 2
torchvision
d2l 1.0.3
SGDScheduleFree

## 与SGD进行比较

![image](https://github.com/user-attachments/assets/917c7cfd-93a5-415f-8838-280dabc1a6b3)
传统的SGD最终的训练损失是0.389，测试精确度是0.838
![image](https://github.com/user-attachments/assets/7c9678ca-4ba6-4425-bd3c-0f6bf7d73fd5)
使用Less Scheduled后训练损失是0.287，测试精确度是0.868
