# INSTRUCTIONS - YOLOv5
  1. Go to YOLOv5 github: `https://github.com/ultralytics/yolov5` and download the files.
  2. Create a new conda enviroment with python 3.8 `conda create -n yolov5 python=3.8 jupyter notebook`
  3. Go to the environment by `conda activate yolov5`
  4. Open up yolov5.ipynb, put the correct directories for images and labels.
  5. **IF YOU ARE NOT USING AZURE VIRTUAL MACHINE, DO NOT RUN CELLS THAT INVOLVE AZURE MACHINE. ONCE YOU CREATED YAML FILE, STOP**
  6. Train the yolov5 model on your local machine by: 
     - `%run yolov5/train.py --img 640 --batch 16 --epochs 1 --data ./molecule_images/molecule_detection_yolov5.yaml --weights yolov5s.pt`
  7. Training results will be saved to: yolov5/runs/train/exp*
     - go to train folder and get the best.pt file, which is already uploaded on our main branch. The whole image set to get the weight file is too big and will not be uploaded here. But you can still download the test.zip file and test the weight file by running this command: `python3 ./yolov5/detect.py --weights ./yolov5/weights/best.pt --iou 0.05 --save-txt --source ./test/images` be sure to put the test images in the appropriate folder before runnning this command.


# INSTRUCTIONS - NORFAIR
  1. Install Norfair with `pip install norfair[video]`
  2. Install `YOLOv5 with pip install yolov5`
  3. Run `python norfair.py <video file>`
  4. Bonus: Use additional arguments --detector_path, --img_size, --iou_thres,--conf_thres, --classes, --track_points as you wish
     - for details, go to `https://github.com/tryolabs/norfair`
  5. Demo test video is uploaded on the main branch as bgremovedphase.avi

## RESULT FROM RUNNING NORFAIR WITH THE VIDEO FILE AND THE WEIGHT FILE PROVIDED
(https://github.com/juniorfutang/qpm_data/blob/main/bgremovedphase_out.mp4?raw=true)

