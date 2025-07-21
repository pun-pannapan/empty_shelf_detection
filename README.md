# empty_shelf_detection

yolo7 roboflow
this information folder is raw and requirement for run ipny file
it will contain  data, require file, image, source code that require for run the ipny file

after run cell 1 in code copy config file to yolov5
1. "copy_file_to_yolo5" copy the config file in "data" and "models"  to the target folder at "clone yolov5 folder" after run "AIEmptyShelfDetection.ipynb" first cell.
2. "dataset" this is a image for train, valid, test for train model.
3. the rest folder is the raw image anotation folder from the "roboflow" that download for yolov5 pytorch model.

step to run in vscode
1. install python 3.11.0 64 bit in windows os.
2. open folder that contain "TestTrainImage2.ipynb" file and "Information" folder.
3. run command below in bash terminal
    python -m venv venv
    .\venv\Scripts\activate
    pip install ipykernel notebook
4. on the top right in vs code select kernel select python 3.11.0
5. save the "AIEmptyShelfDetection.ipynb" file.
5. click run on first cell on "AIEmptyShelfDetection.ipynb" file it
    will clone the yolov7 to local machine and install all the package
    it will take around 4 minute to complete this step. (for the first time)
6. Click run the next cell it should show result for detect the "Horse.jpg" picture
7. Go to "https://wandb.ai/authorize" in browser and copy the API key 
    and put the Api Key in the ipynb file like this "!wandb login abc1234567890abcdef1234567890abcdef1234"
8. Click run the next cell it should login to wandb.
9. Check the "train" and "val" path exists in "C:\Work\Task Shelf Monitoring - AI Camera\TestTrainImage2\Information\copy_file_to_yolo5\data\custom.yaml"
10. Copy file from "Information\copy_file_to_yolo5" to yolo5 folder.
11. Click run the next cell to train model.
12. Click run the next cell to test dataset with best model the result must be in .

