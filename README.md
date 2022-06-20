
## Installation

```shell
conda create -n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -c pytorch -y
conda activate open-mmlab
pip3 install openmim
mim install mmcv-full
mim install mmdet
git clone https://github.com/open-mmlab/mmocr.git
cd mmocr
pip3 install -e .
```

## To Run the file
```
conda activate open-mmlab
python mmocr/utils/ocr.py demo/demo_text_ocr.jpg --print-result --imshow

```