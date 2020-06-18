# AI_begin
#yolov3_deepsort(object detected in video and webcam with CPU)
use anacaonda3 prompt
B1: git clone
B2: cd yolov3_deepsort
B3: conda env create -f conda-cpu.yml
B4: conda activate tracker-cpu
B5: pip install -r requirements.txt
B6: Down weight
B7: move this to folder weight of your project
B8: nomal weight:
python load_weights.py
-----------------
OR
tiny weight:
python load_weights.py --weights ./weights/yolov3-tiny.weights --output ./weights/yolov3-tiny.tf --tiny
B9: Running
Video
python object_tracker.py --video ./data/video/test.mp4 --output ./data/output/results.avi
webcam
python object_tracker.py --video 0 --output ./data/output/results.avi
-----------------
OR
tiny
python object_tracker.py --video ./data/video/test.mp4 --output ./data/video/results.avi --weights ./weights/yolov3-tiny.tf --tiny
#yolo_beginer
read all about object detected in picture at miai.vn (YOLO series #1)
