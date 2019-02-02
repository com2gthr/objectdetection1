# objectdetection1
the code implement the object detection using the yolo algorithm
I have used python as my primarily language.
To run the above mentioned code you may need to import the following libraries and deafult files.Installation
Dependencies

Tensorflow Object Detection API depends on the following libraries:

    Protobuf 3.0.0
    Python-tk
    Pillow 1.0
    lxml
    tf Slim (which is included in the "tensorflow/models/research/" checkout)
    Jupyter notebook
    Matplotlib
    Tensorflow (>=1.9.0)
    Cython
    contextlib2
    cocoapi

For detailed steps to install Tensorflow, follow the Tensorflow installation instructions. A typical user can install Tensorflow using one of the following commands:

# For CPU
pip install tensorflow
The remaining libraries can be installed on Ubuntu 16.04 using via apt-get:

sudo apt-get install protobuf-compiler python-pil python-lxml python-tk
pip install --user Cython
pip install --user contextlib2
pip install --user jupyter
pip install --user matplotlib

Alternatively, users can install dependencies using pip:

pip install --user Cython
pip install --user contextlib2
pip install --user pillow
pip install --user lxml
pip install --user jupyter
pip install --user matplotlib

Note: sometimes "sudo apt-get install protobuf-compiler" will install Protobuf 3+ versions for you and some users have issues when using 3.5. If that is your case, try the manual installation.
COCO API installation

Download the cocoapi and copy the pycocotools subfolder to the tensorflow/models/research directory if you are interested in using COCO evaluation metrics. The default metrics are based on those used in Pascal VOC evaluation. To use the COCO object detection metrics add metrics_set: "coco_detection_metrics" to the eval_config message in the config file. To use the COCO instance segmentation metrics add metrics_set: "coco_mask_metrics" to the eval_config message in the config file.

git clone https://github.com/cocodataset/cocoapi.git
cd cocoapi/PythonAPI
make
cp -r pycocotools <path_to_tensorflow>/models/research/

Protobuf Compilation

The Tensorflow Object Detection API uses Protobufs to configure model and training parameters. Before the framework can be used, the Protobuf libraries must be compiled. This should be done by running the following command from the tensorflow/models/research/ directory:
I am just attachinng the main code for object detection if you need the full api do let me know at amanvrm2195@gmail.com
