## Wildlife cam 2.0 

This repo contains the code needed to build an object detection web app using TensorFlow.js and React. 

### The model
The model featured in the app, is a pre-trained [COCO SSD](https://github.com/tensorflow/tfjs-models/tree/master/coco-ssd) system.

### Requirements
Only a browser and a local web server.

### Instructions

Start video on pi by going to `/mjpg-streamer/mjpg-streamer-experimental` folder and running `export LD_LIBRARY_PATH="$(pwd)"` then `./mjpg_streamer -o "output_http.so -w ./www" -i "input_raspicam.so" -b` This will start the image stream at `http://<pi-ip>:8080/`

To launch the web app, go to the root directory of the app, and launch a web server. An easy way to create a one is with Python, using the following command `$ python3 -m http.server` or `$ python -m SimpleHTTPServer` if you're using Python 2.

Once the server is up and running, open your browser, and go to http://localhost:8000/

### Tutorial
For a complete tutorial, and a theory lesson about the model and what's under the hood, please refer to the following link: [In-Browser Object Detection Using Tensorflow.js](https://nanonets.com/blog/object-detection-tensorflow-js/)

