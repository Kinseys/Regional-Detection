# Regional-Detection
Yolov5 + Deepsort + Regional detection for regional detection and tracking

For the environments: <br> <br>
  `pip install -r requirements.txt`  <br> <br>
  
## If you want to use regional detection on video with tracking:<br> <br>
The default weight is `yolov5/weights/yolov5s.pt` you can change it by add `--yolo_weights xxx.pt`

run `python RegionDetect.py --source xxx.mp4 --show-vid` for video detection<br> <br>
run `python RegionDetect.py --source 0 --show-vid` for stream detection use your own camera<br> <br>

For saving the results:
run `python RegionDetect.py --source xxx.mp4 --show-vid --save-vid` for video detection<br> <br>
run `python RegionDetect.py --source 0 --show-vid --save-vid` for stream detection use your own camera<br> <br>
The results are saved in `inference/`<br> <br>
### If you want to change the detection region, go to `RegionDetect.py` line 96 to change the four points.


## If you only want to use regional detection on image/video without tracking:<br> <br>

Go to `yolov5/`:<br> <br>
The default weight is `yolov5s.pt` you can change it by add `--weights xxx.pt` like:<br>
`python detect.py --source data/images --weights xxx.pt`<br> <br>
run `python detect.py --source data/images` for image detection<br> <br>
run `python detect.py --source xxx.mp4` for video detection<br> <br>
run `python detect.py --source 0` for stream detection use your own camera<br> <br>
The results are saved in `yolov5/results/`<br> <br>

### If you want to change the detection region, go to `detect.py` line 96 to change the four points.

  
  
