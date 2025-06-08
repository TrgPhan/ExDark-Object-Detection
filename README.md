# ExDark Object Detection

This project focuses on object detection in low-light environments using the Exclusively Dark (ExDARK) dataset for AI training. The ExDARK dataset, containing 7,363 low-light images derived from PASCAL VOC and Microsoft COCO, includes annotations for 12 object classes: Bicycle, Boat, Bottle, Bus, Car, Cat, Chair, Cup, Dog, Table, Motorbike, and People. Annotations are provided in the ExDark_Anno text file with labels, bounding box coordinates (`xmin`, `ymin`), and dimensions (`box_width`, `box_height`). The dataset was preprocessed to normalize annotations to the COCO format (`[xmin, ymin, xmax, ymax]`) with class IDs 1–12, reserving ID 0 for the background, enabling robust training with models like Faster R-CNN.

## Faster R-CNN Model
Faster R-CNN, a two-stage object detection framework, was trained on the ExDARK dataset, achieving a test mAP@0.5 of 0.7209 at epoch 10, with notable AP@0.5 scores for Bus (0.8918) and Bicycle (0.8488). Despite challenges like dataset noise and limited GPU resources (240 hours of training across four Kaggle accounts), dataset normalization improved mAP@0.5 from 0.3 to 0.72. This work pioneers Faster R-CNN's application to ExDARK, outperforming baseline models like EdgeBoxes and demonstrating superior real-world performance compared to YOLOv5 and RCNN (mAP@0.5 0.48).

## Dataset and Models
Access the ExDARK dataset and trained models via the following link:  
[Google Drive](https://drive.google.com/drive/folders/1PAJxv8rJoWVdqw5uueNruL1AUci0Sul9?usp=drive_link)
