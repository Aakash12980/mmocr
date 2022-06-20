
## Installation
Please install Anaconda first and then replicate the following steps to make it ready to test.

```shell
conda create -n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -c pytorch -y
conda activate open-mmlab
pip3 install openmim
mim install mmcv-full
mim install mmdet
git clone https://github.com/Aakash12980/mmocr.git
cd mmocr
pip3 install -e .
```

## To Run the file

To infer on custom images, Place the images inside ```mmocr/demo``` folder.
The output image will be saved inside ``` mmocr/output/out.jpg ``` with all the bounding detected bounding boxes printed in the image.
The information regarding angles is printed in the command line. Each bounding box's angles can be seen with their mean value and with highest recurring angle.
The list of predicted text is also printed in the command screen.

```
conda activate open-mmlab
python mmocr/utils/ocr.py demo/demo_text_ocr.jpg --print-result --imshow

```