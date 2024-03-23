<h3>Car Parts and Car Damage Segmentation using MA-Net</h3> 

This repository contains the code for a semantic segmentation project aimed at identifying car parts and car damages in images. The project utilizes the Multi Scale - Attention Network architecture from the Segmentation Models library, along with Dice Loss as the loss function and Intersection over Union (IoU) as the evaluation metric. The model is fine-tuned using ImageNet weights.

<h6> Highlights</h6>

    Architecture: MA-Net (Multi Scale - Attention Network) from the Segmentation Models library
    Loss Function: Dice Loss
    Evaluation Metric: Intersection over Union (IoU)
    Pre-trained Weights: ImageNet weights used for fine-tuning

**Dataset**

The dataset consists of 1,812 images, split into two categories: car parts (998 images) and car damages (814 images).

**Classes**

The classes for car parts segmentation include:
Windshield, Back-windshield, Front-window, Back-window, Front-door, Back-door, Front-wheel, Back-wheel, Front-bumper, Back-bumper, Headlight, Tail-light, Hood, Trunk, License-plate, Mirror Roof, Grille, Rocker-panel, Quarter-panel, Fender

**Training**

The model was trained using the following hyperparameters:

    Learning Rate: 0.0001
    Epochs: 50


**Model, Loss, and Optimizer**


The training progress was logged using the tqdm library, and the final evaluation results on the validation set are displayed below:

  Epoch 50/50: 100%|██████████| 50/50 [02:56<00:00,  3.53s/it, iou_score=0.868, loss=0.16]
  
  Epoch under Validation, Loss: 0.20312069356441498, IOUScore 0.8604951500892639


**Results**

![CarParts](https://github.com/VigneshArjunRaj/Car-Parts-Segmentation-using-Multi-Scale-Attention-Network/assets/45617829/748d5164-6be0-448c-be82-003074b14300)


