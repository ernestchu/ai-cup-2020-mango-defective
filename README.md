# AI CUP 2020 Mango Image Recognition Challenge
[Challenge Main Page](https://aidea-web.tw/aicup_mango)
## Defective Classification
### Fill the testing label sheet from the predicted outputs
[IPython Notebook](https://github.com/ernestchu/ai-cup-2020-mango-defective/blob/main/fill.ipynb)
### Training
Download and untar the [dataset](https://drive.google.com/file/d/1kI7-eQBWs6F4_7ppuPIBi2SmZj2NR_XI/view?usp=sharing) to the root. Then navigate into yolo directory.
```shell
cd yolov5
chmod +x train.sh
./train.sh
```
You can edit [train.sh](https://github.com/ernestchu/ai-cup-2020-mango-defective/blob/main/yolov5/train.sh) to config image size, batch size, number of epochs and the pre-trained model.
