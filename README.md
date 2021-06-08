# INSTRUCTIONS - YOLOv5
  1. Go to YOLOv5 github: `https://github.com/ultralytics/yolov5` and download the files.
  2. Create a new conda enviroment with python 3.8 `conda create -n yolov5 python=3.8 jupyter notebook` `conda activate yolov5`
  3. Make a jupyter notebook file
  4. Install essentials by writing these lines on the first line of the cell: `%pip install -r yolov5/requirements.txt` `%pip install sklearn scikit-image azureml-core`
  5. prepare YOLO labels
Install Norfair with pip install norfair[video].
Install YOLOv5 with pip install yolov5.
Run python yolov5demo.py <video file>.
Bonus: Use additional arguments --detector_path, --img_size, --iou_thres,--conf_thres, --classes, --track_points as you wish.
