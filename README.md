# TermProject-2021-kitti  

## 1. Dataset Preparation    
- [KITTI dataset](https://drive.google.com/drive/folders/1f47HB5gLQDElIAf600SX-VtrX58i7SpU?usp=sharing)  
    - Training images  : 3000  
    - Validation images: 81  
    - Testing images   : 4481  

- Sample numbers of the training data with 8 classes:  

    |   Classes     |  Car   | Van|Truck|Walker|Sitter|Rider|Tram|Misc.|
    | ------------- |:------:|:--:|:---:|:----:|:----:|:---:|:--:|:---:|
    | Sample number |   11379|1197|  428|  1816|    93|  671| 208|  428|
    

## 2. Testing Result:
- ### YOLOv3 `AP: 32.7%`  

  - Mean average precision of each class:  
    |   Classes         |Car|  Van|Truck|Walker|Sitter|Rider|  Tram|Misc.|
    | ----------------- |:-:|:---:|:---:|:----:|:----:|:---:|:----:|:---:|
    | Average Precision |73%|35.9%|56.5%| 31.5%|    0%|30.5%| 33.8%| 0.3%|  
    
  - Performance:  

    <img src="figures/v3_1.jpg" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/v3_2.jpg" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/v3_3.jpg" alt="arch" width="500" style="zoom:100%;" />  
    
- ### YOLOv4 `AP: 43.8%`  

  - Mean average precision of each class:  
    |   Classes         |Car|  Van|Truck|Walker|Sitter|Rider|  Tram|Misc.|
    | ----------------- |:-:|:---:|:---:|:----:|:----:|:---:|:----:|:---:|
    | Average Precision |63.6%|63%|79%| 26.7%|   19.1%|40.1%| 57.5%| 50.2%|  
    
  - Performance:  

    <img src="figures/v4_1.jpg" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/v4_2.jpg" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/v4_3.jpg" alt="arch" width="500" style="zoom:100%;" />  

    
- ### Scaled YOLOv4 `AP: 47.6%`  

  - Mean average precision of each class:  
    |   Classes         |Car|  Van|Truck|Walker|Sitter|Rider|  Tram|Misc.|
    | ----------------- |:-:|:---:|:---:|:----:|:----:|:---:|:----:|:---:|
    | Average Precision |65.7%|60.9%|65.3%| 23.5%|   15.0%|60.4%| 62.9%| 59.1%|  
    
  - Performance:  
    
    <img src="figures/sv4_1.jpg" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/sv4_2.jpg" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/sv4_3.jpg" alt="arch" width="500" style="zoom:100%;" />  
    
- ### SSD (VGG-300, pretrained model) `AP: 24%`  

  - Mean average precision of each class:  
    |   Classes         |Car|  Van|Truck|Walker|Sitter|Rider|  Tram|Misc.|
    | ----------------- |:-:|:---:|:---:|:----:|:----:|:---:|:----:|:---:|
    | Average Precision |59.6%|39.3%|29.9%| 9.1%| 0%|10.6%| 23.6%| 20.0%|  
    
  - Performance:  
    
    <img src="figures/sv4_1.jpg" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/sv4_2.jpg" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/sv4_3.jpg" alt="arch" width="500" style="zoom:100%;" />  
    
- ### Faster RCNN (ResNet-101, pretrained model) `AP: 63.6%`  

  - Mean average precision of each class:  
    |   Classes         |Car|  Van|Truck|Walker|Sitter|Rider|  Tram|Misc.|
    | ----------------- |:-:|:---:|:---:|:----:|:----:|:---:|:----:|:---:|
    | Average Precision |80.0%|78.4%|86.3%| 57.8%| 16.5%|67.3%| 75.7%| 49.1%|  
    
  - Performance:  
    
    <img src="figures/faster_1.jpg" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/faster_2.jpg" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/faster_3.jpg" alt="arch" width="500" style="zoom:100%;" />  
    
- ### Mask RCNN (ResNet-101, pretrained model) `AP: 57.99%`  

  - Mean average precision of each class:  
    |   Classes         |Vehicle|  Person|
    | ----------------- |:-----:|:------:|
    | Average Precision |  75.1%|   45.0%|
    
  - Performance:  
    
    <img src="figures/mask_1.JPG" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/mask_2.JPG" alt="arch" width="500" style="zoom:100%;" />  
    <img src="figures/mask_3.JPG" alt="arch" width="500" style="zoom:100%;" />  
    
## 3. Summary

