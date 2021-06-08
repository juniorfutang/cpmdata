# INSTRUCTIONS - YOLOv5
  1. Go to YOLOv5 github: `https://github.com/ultralytics/yolov5` and download the files.
  2. Create a new conda enviroment with python 3.8 `conda create -n yolov5 python=3.8 jupyter notebook` `conda activate yolov5`
  3. Open up yolov5.ipynb, put the correct directories for images and labels.
  4. **IF YOU ARE NOT USING AZURE VIRTUAL MACHINE, DO NOT RUN CELLS THAT INVOLVE AZURE MACHINE. ONCE YOU CREATED YAML FILE, STOP**
  5. Train the yolov5 model on your local machine: `%run yolov5/train.py --img 640 --batch 16 --epochs 1 --data ./molecule_images/molecule_detection_yolov5.yaml --weights yolov5s.pt`
  6. yolov5/runs/train/exp* - go to train folder and get the best.pt file, which is already uploaded on our main branch. The whole image set to get the weight file is too big and will not be uploaded here. But you can still download the test.zip file and test the weight file by running this command: `python3 ./yolov5/detect.py --weights ./yolov5/weights/best.pt --iou 0.05 --save-txt --source ./test/images` be sure to put the test images in the appropriate folder before runnning this command.


# INSTRUCTIONS - NORFAIR
Install Norfair with pip install norfair[video].
Install YOLOv5 with pip install yolov5.
Run python yolov5demo.py <video file>.
Bonus: Use additional arguments --detector_path, --img_size, --iou_thres,--conf_thres, --classes, --track_points as you wish.
