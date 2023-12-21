# DETAMP
DETAMP (Defection Template Matching PCB) adalah model machine learning AI Computer Vision yang dapat mendeteksi kerusakan pada jalur PCB setelah produksi sebelum dilakukan penyolderan dan pemasangan komponen.

Step by Step

1.download file data pada link tersebut 
https://drive.google.com/file/d/1UmMugpgDqP8ZFhLIMHaEG1HRQWa2eWth/view?usp=sharing(checkpoints)
https://drive.google.com/file/d/1EHxZblCSBCqAJrT9RpmZy7JR8itXMUam/view?usp=sharing(yolov4-pcb.weights)

2.lakukan install python versi 3.10.1
3.melakukan install pip pada visual code
- pip install tensorflow
- pip install pillow
- pip install flask
- pip install opencv-python
- pip install easydict
- pip install waitress
- pip install paste
4. ## yolov4(membuat folder checkpoints) setelah itu lakukan terminal 
python save_model.py --weights ./data/yolov4.weights --output ./checkpoints/yolov4-416 --input_size 416 --model yolov4 

# Run Waitress wsgi for production deployment

python waitress-server.py

### Run Flask app

python app.py

