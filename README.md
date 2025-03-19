# Road-Crack-Segmentation-LiteFusionNet
(Paper link and model file will be provided soon, stay tuned!!!)

This repository gives the overview of our proposed work on road crack detection problem (segmentation).


![Image](https://github.com/user-attachments/assets/1d419394-7ec9-4882-be6c-830a3402a8d9)


## Dataset
This work considers [CRACK500](https://github.com/fyangneil/pavement-crack-detection), [DeepCrack](https://github.com/yhlleo/DeepCrack/tree/master) and [RCD]() (which combines CRACK500 and DeepCrack). Moreover, to have real-world road crack segmentation, it uses [CrackSeg](https://github.com/TRMetaGroup/CrackSeg) dataset.

## Performance
Performance of key models compared to the proposed LiteFusionNet



|Dataset | Model | DS | mIoU | P | R | Params | GFLOPs | Inference (ms) | 
|:--------|:----:|:---:|:--:|:--:|:--:|:--:|:--:|:--:|		
| Crack500 | UNet-small | 0.6017 | 0.4303 | 0.7396 | 0.5072 | 0.537M | 4.930 | 1.23 |
|          | ULite      | 0.6944 | 0.5319 | 0.7454 | 0.6499 | 0.878M | 1.183 | 1.55 |
|          | DABNet     | 0.7776 | 0.6361 | 0.7997 | 0.7566 | 0.752M | 2.064 | 2.17 |
|          | ENet       | 0.7805 | 0.6400 | 0.8143 | 0.7494 | 0.349M | 0.836 | 4.07 |
|          | CFPNet     | 0.7753 | 0.6330 | 0.8060 | 0.7468 | 0.547M | 1.563 | 8.44 |
|          | LiteFusionNet (ours) | 0.7828 | 0.6431 | 0.7642 | 0.8022 |0.493M | 0.397 | 3.69 |
| DeepCrack | UNet-small | 0.7662 | 0.6210 | 0.8573 | 0.6926 | 0.537M | 4.930 | 1.27 |
|           | ULite      | 0.8245 | 0.7014 | 0.8840 | 0.7735 | 0.878M | 1.183 | 1.57 |
|           | DABNet     | 0.8038 | 0.6720 | 0.8644 | 0.7512 | 0.752M | 2.064 | 2.08 |
|           | ENet       | 0.8279 | 0.7064 | 0.8819 | 0.7802 | 0.349M | 0.836 | 4.06 |
|           | CFPNet     | 0.8106 | 0.6815 | 0.8345 | 0.7880 | 0.547M | 1.563 | 8.24 |
|           | LiteFusionNet (ours) | 0.8338 | 0.7150 | 0.8516 | 0.8167 | 0.493M | 0.397 | 3.58 |
| RCD     | UNet-small | 0.5620 | 0.3908 | 0.6961 | 0.4712 | 0.537M | 4.930 | 1.23 | 
|         | ULite      | 0.7254 | 0.5692 | 0.7757 | 0.6813 | 0.878M | 1.183 | 1.54 |
|         | DABNet     | 0.7780 | 0.6367 | 0.8211 | 0.7392 | 0.752M | 2.064 | 2.16 |
|         | ENet       | 0.7801 | 0.6394 | 0.8093 | 0.7796 | 0.349M | 0.836 | 4.69 |
|         | CFPNet     | 0.776  | 0.6342 | 0.8161 | 0.7398 | 0.547M | 1.563 | 8.25 |
|         | LiteFusionNet (ours) | 0.7908 | 0.6540 | 0.7750 | 0.8077 | 0.493M | 0.397 | 3.33 |


## Model
The model file is provided in the repository; researchers can use it if they wish to train the model from scratch on road crack datasets or other problems in their training framework.

(Note: The results may vary slightly due to the environment, library versions, GPU, and framework used on the same datasets.)

The published work provides the remaining information on the model and performance analysis with detailed ablations.



## Cite

Please cite this publication if you use RCD dataset and/or LiteFusionNet in your research.


