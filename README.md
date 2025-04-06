# License-Plate-Recognition
## Demo
Please click on the image below to watch the demonstration video:
[![Watch Video here](https://private-user-images.githubusercontent.com/124408051/430674363-1191bd08-88d7-423e-992d-63a3aacd741a.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDM5MDg0OTgsIm5iZiI6MTc0MzkwODE5OCwicGF0aCI6Ii8xMjQ0MDgwNTEvNDMwNjc0MzYzLTExOTFiZDA4LTg4ZDctNDIzZS05OTJkLTYzYTNhYWNkNzQxYS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQwNlQwMjU2MzhaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1iZWY4YTM1YmM5N2U1MWY1ODYyNmUyODI5NzVkY2Q3NTYxZmUyMzg3NzBiYzM1NzllNWMxNjg0MzAxY2ZmNDZhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.i-xDRevtFsiOGk4sez7Gb77g8a4L3WQdkzql6uw0k6M)](https://drive.google.com/file/d/1_6m-6Rubs2BMixEhzdayYr-sOmlbxoSg/view?usp=sharing)


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
