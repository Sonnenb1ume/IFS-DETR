# IFS-DETR: A real-time industrial fire smoke detection algorithm based on an end-to-end structured network
# Data set introduction
Aiming at the shortcomings of existing industrial fire smoke data sets in terms of clarity, data diversity and data volume, we collected more than 5000 images and 5 fire surveillance videos from actual industrial fire smoke scenes to construct a more comprehensive data set.

# Data annotation & Enhancement
We used the **[LabelImg](https://github.com/HumanSignal/labelImg)** tool to annotate the image data, and the samples were clearly divided into "fire" and "smoke" categories. After data cleaning, all the data is divided into training set, verification set and test set according to the ratio of 7:1:2. We apply three image enhancement algorithms to enhance the training set:
1. Randomly selecting 15% of the images, changing the brightness of the images in the range of [0.7-1.3] and generating a new image.
2. Randomly selecting 15% of the images, flipping them horizontally once and generating a new image.
3. Randomly selecting 10% of the images in the original image and adding fuzzy noise.

# Data set format
The resulting industrial fire smoke dataset consists of 4304 training set images, 439 validation set images, and 879 test set images. The format of the dataset is as follows:
```
IFS_dataset/
└── images/
    └── train/   # train images
    └── val/     # val images
    └── test/    # test images
└── labels/
    └── train/   # train labels.txt
    └── val/     # val labels.txt
    └── test/    # test labels.txt
└── labels_xml/
    └── train/   # train labels.xml
    └── val/     # val labels.xml
    └── test/    # test labels.xml
```
![The data set is labeled with case and sample distribution information](https://github.com/user-attachments/assets/43a8787a-4706-447c-bd76-f545b1764d6f)

# Data set linking
Images File:   **[https://pan.quark.cn/s/0a76663e183a](https://pan.quark.cn/s/0a76663e183a)**    提取码:WUGx

Lables File:   **[https://pan.quark.cn/s/c6d1ff91bc89](https://pan.quark.cn/s/c6d1ff91bc89)**    提取码:ngkp

Lables_xml File:   **[https://pan.quark.cn/s/d98657a7a721](https://pan.quark.cn/s/d98657a7a721)**    提取码:rRj9

# Cite
If you have used our data in your research work, please cite our work, thank you very much.

```
@article{IFS-DETR,
  title={IFS-DETR: A real-time industrial fire smoke detection algorithm based on an end-to-end structured network},
  author={Chen, JiaSheng and Han, HuiZi and Liu, Mei and Su, Peng and Chen, Xi},
  journal={Measurement},
  pages={115660},
  year={2024},
  publisher={Elsevier}
}
```
