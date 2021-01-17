# AI CUP 2020 Mango Image Recognition Challenge
[Challenge Main Page](https://aidea-web.tw/aicup_mango)

## Defective Classification

### Fill the testing label sheet from the predicted outputs
[IPython Notebook](https://github.com/ernestchu/ai-cup-2020-mango-defective/blob/main/fill.ipynb)

### Training
Download and untar the [dataset](https://drive.google.com/file/d/1kI7-eQBWs6F4_7ppuPIBi2SmZj2NR_XI/view?usp=sharing) to the root directory of this project. Then navigate into yolo directory.
```shell
cd yolov5
chmod +x train.sh
./train.sh
```
You can edit [train.sh](https://github.com/ernestchu/ai-cup-2020-mango-defective/blob/main/yolov5/train.sh) to config image size, batch size, number of epochs and the pre-trained model.

The result is at [runs](https://github.com/ernestchu/ai-cup-2020-mango-defective/tree/main/yolov5/runs).

### Inference
Make sure you have a trained weight and testing set at
```
yolov5/runs/train/exp/weights/best.pt
mango_data/images/Test
```
Then you can perform inference and generate the result [text files](https://github.com/ernestchu/ai-cup-2020-mango-defective/tree/main/yolov5/runs/detect/exp/labels)
