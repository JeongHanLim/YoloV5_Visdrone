training option: python train.py --cfg yolov5l.yaml --weights yolov5l.pt --epoch 200 --batch-size 40 --device 0
test option : python test.py --weights ./runs/train/exp4/weights/best.pt 

default
--cfg yolov5s.yaml
--data ./data/coco128.yaml

My concern
1. while using yolov5s model, I haven't changed class number
2. annotation 0 and 11 refers ignored region and others respectively. This may lead to bad inference, as they make wrong choose.

*annotations vs labels
annotations : exist on visdrone dataset
labels : changed to yolov5 format using Visdrone2YOLO.py

*You may change your dataset path and label path at ./data/coco128.yaml


