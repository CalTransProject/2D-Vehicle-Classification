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

This repository holds the code for our 2D vehicle classification model, a key part of our Real-Time Traffic Management (RTTM) web application. To explore the full RTTM project, check out the link provided.
* [RTTM](https://github.com/CalTransProject/rttm)
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


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Geeks-For-Geeks-Program-to-extract-frames-using-OpenCV](https://www.geeksforgeeks.org/python-program-extract-frames-using-opencv/)
* [Ultralytics](https://docs.ultralytics.com/)


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[product-screenshot]: images/screenshot.png
