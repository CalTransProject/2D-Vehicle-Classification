<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/CalTransProject/rttm">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>
  <h3 align="center">YoloV8-2D-Vehicle-Classification-Model</h3>

</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com) 

This repository holds the code for our 2D vehicle classification model, a key part of our Real-Time Traffic Management (RTTM) system. To explore the full RTTM project, check out the provided links:
* [RTTM](https://github.com/CalTransProject/rttm)
* [3D Object Detection Research Project](https://arcs.center/3d-object-detection-and-vehicle-classification-based-on-lidar-point-clouds-for-real-time-traffic-flow-monitoring/)
<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

* [![Logo](https://assets-global.website-files.com/646dd1f1a3703e451ba81ecc/64777c3e071ec953437e6950_logo.svg)](https://docs.ultralytics.com/)
* [![Logo](https://opencv.org/wp-content/uploads/2022/05/logo.png)](https://opencv.org/)
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you can download and use the model

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
  ```sh
  pip install ultralytics
  ```

### Installation

* Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Download Model From: <br>
   [git clone https://github.com/your_username_/Project-Name.git](https://github.com/CalTransProject/2D-Vehicle-Classification/blob/main/model/Newest-YoloV8-2D-Vehicle-Classification-Model.pt)

3. Install Ultralytics packages
   ```py
   pip install ultralytics
   ```
4. Import Library
   ```py
   from ultralytics import YOLO
   ```
5. Load Pretrained Model (The model you downloaded previously)
   ```py
   model_path = 'path/to/model'
   model = YOLO(model_path)
   ```
6. Run Inference on a image
   ```py
   image_path = 'path/to/image.png"
   model.predict(image_path, save=True, imgsz=320, conf=0.5)
   ```
7. Run Inference using webcam
   ```py
   model.predict(source = "0", save=True, imgsz=320, conf=0.5)
   ```
8. For more Details check the documentation:
   [Documentation](https://docs.ultralytics.com/)
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

The project aims to classify vehicles in real-time from a 2D video stream.

For more examples, please refer to the complete project repository [rttm.](https://github.com/CalTransProject/rttm)
<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

Robin Rosculete - [linkedin](https://www.linkedin.com/in/robin-rosculete-b51641202/) - robin.rosculete.860@my.csun.edu

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- File Structure -->
## File Structure
```
   .
    ├── Configuration-Files # Directory consisting of both testing and training configuration files.
    │   ├── config_test.yaml  # Config file for testing. Testing data is set as the validation to enable the use of model.val() for testing on new data.
    │   └── config_train.yaml  # Config file for training and validation during training. 
    ├── images  # Images used in the readme.md file                   
    │   ├── logo.png       
    │   └── screenshot.png                    
    ├── model # Directory holding the models obtained after training the YoloV8 model on our data
    │   ├── Newest-YoloV8-2D-Vehicle-Classification-Model.pt # Model trained on the dataset collected and labeled in 2023 - 2024
    │   └── Old-YoloV8-2D-Vehicle-Classification-Model.pt  # Model trained on the dataset collected and labeled in 2022 - 2023
    ├── notebooks # Directory holding the notebooks 
    │   ├── runs/detect # Results from training, validation, and testing the model
    │   │   ├── train # Training and validation (during training) result in images and also weights of the last trained model
    │   │   │   ├── weights # Model weights after training
    │   │   │   │   ├── best.pt # Weights for the model at the best epoch
    │   │   │   │   └── last.pt # Weights for the model at the last epoch
    │   │   │   ├── ... # Files and images consisting of results from training and validation
    │   │   ├── val # Results from testing the model on new data, it is called val because of the model.val() was used as a workaround for testing with a different config file
    │   │   │   └── ... # Files and images consisting of results from testing the model
    │   ├── AutoLabeling.ipynb # Notebook containing the Autolabeling code used to label new data
    │   ├── Extract-Frames.ipynb # Notebook containing code for breaking collected video data into frames
    │   └── vehicle-classification-using-yolo-v8.ipynb # Notebook containing the code for both training and testing code (main notebook of model)
    ├── .gitignore
    └── README.md
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Professor Xunfei Jiang](https://www.csun.edu/~xjiang/)
* [CSUN-ARCS](https://arcs.center/)
* [Geeks-For-Geeks-Program-to-extract-frames-using-OpenCV](https://www.geeksforgeeks.org/python-program-extract-frames-using-opencv/)
* [Ultralytics](https://docs.ultralytics.com/)


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[product-screenshot]: images/screenshot.png
