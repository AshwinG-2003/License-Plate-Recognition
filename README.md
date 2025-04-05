# License-Plate-Recognition-YOLOv8
## Demo

https://github.com/Muhammad-Zeerak-Khan/Automatic-License-Plate-Recognition-using-YOLOv8/assets/79400407/1af57131-3ada-470a-b798-95fff00254e6


## Data

The video used in the tutorial can be downloaded [here](https://drive.google.com/file/d/1JbwLyqpFCXmftaJY1oap8Sa6KfjoWJta/view?usp=sharing).

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
