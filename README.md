# GuitarRecognizer
This project labels guitars in real-time video on the edge.

# References
The backbone of this project utilizes much of the code from this Mask Detection Tutorial (https://www.pyimagesearch.com/2020/05/04/covid-19-face-mask-detector-with-opencv-keras-tensorflow-and-deep-learning/) to set up the video stream and reformat the model to run in OpenCV for use on the Intel Movidius NC2.

# Model
Transfer learning was used to expand upon a pretrained MobileNet SSD model.

# Data
Images of guitars were scraped from an image search engine result.

# Running the model on the Raspberry Pi
> python3 openvino_real_time_guitar_detection.py -- model MobileNetSSD_deploy.caffemodel -- prototxt MobileNetSSD_deploy.prototxt -- modeltransfer guitar_case.model

