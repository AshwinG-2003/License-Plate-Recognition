# License-Plate-Recognition
## Demo
Please click on the image below to watch the demonstration video:
[![Watch Video here](https://github.com/user-attachments/assets/6123bca0-5244-469a-acae-1a15532b5aa4)](https://drive.google.com/file/d/1_6m-6Rubs2BMixEhzdayYr-sOmlbxoSg/view?usp=sharing)


## Data

The video used can be downloaded [here](https://drive.google.com/file/d/1JbwLyqpFCXmftaJY1oap8Sa6KfjoWJta/view?usp=sharing).

## Model

A Yolov8 pre-trained model (YOLOv8n) was used to detect vehicles.

- The model is available in models folder for both the yolo model and license plate model.

## Dependencies

The sort module needs to be downloaded from [this repository](https://github.com/abewley/sort).

```bash
git clone https://github.com/abewley/sort
```

## Project Setup
* Install the project dependencies using the following command 
```bash
pip install -r requirements.txt
```
* Run main.py with the sample video file to generate the test.csv file 
``` python
python main.py
```
* Run the add_missing_data.py file for interpolation of values to match up for the missing frames and smooth output.
```python
python add_missing_data.py
```

* Finally run the visualize.py passing in the interpolated csv files and hence obtaining a smooth output for license plate detection.
```python
python visualize.py
```
