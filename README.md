## Project Description

- Beer-detection-model-by-YOLOv9 is a project for training the YOLOv9 model and deploying it via a web application
- The purpose of our project is to develop an image analysis tool that can automatically detect key elements (brand logos, products, advertising materials, people, etc.) in images.
## Hackathon Category Selected

Heineken Detect - Utilizing technology to improve inspection and detection processes.

## Demo
- [Web - Image](https://minhkhanh-eternai.github.io/Beer-Detection-Model-By-YOLOv9/)
- [Mobile - Video (Realtime)](https://demo.roboflow.com/detect-beer-8c3cm/12?publishable_key=rf_RoiqmRyrawXjoL11CCpF)

  ![image](./public/image/qr-code.png)

## How it Works
1. **Data Collection and Annotation:** The dataset of beer images is collected and annotated using Roboflow. Each image is labeled to identify the beer bottles.
2. **Model Training:** The YOLOv9 model is trained using the annotated dataset. PyTorch is used as the deep learning framework to implement and train the model.
3. **Model Deployment:** A Flask web application is developed to deploy the trained model. The application uses OpenCV for image processing and allows users to upload images for beer detection.
4. **Inference:** When an image is uploaded, the Flask application processes it through the YOLOv9 model to detect and highlight beer bottles in the image.
5. **Output:** The result is displayed on the web interface, showing the original image with detected beer bottles highlighted.

## Technology Stack

- **Solution:** Object detection using YOLOv9
- **Technological Infrastructure:** 
  - Python for training the YOLOv9 model
  - Flask for web deployment
- **Technology Services:** 
  - Roboflow: A web allow to label dataset and deploy model
  - OpenCV: Library for computer vision tasks
  - PyTorch: Deep learning framework for training YOLOv9


## Installation

To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone <repository_url>
    ```
2. Navigate to the project directory:
    ```bash
    cd AIO-3KA_hackhcmc
    ```
3. Run following file to train:
    ```bash
    Yolov9_model.ipynb
    ```
4. Replace your model, version, api_key in ```scripts.js```:
    ```bash
    $('#model').val("YOUR MODEL NAME");
    $('#version').val("YOUR MODEL VERSION");
    $('#api_key').val("YOUR API");    ```

## Usage

The main entry point of the application is the `Yolov9_model.ipynb` for model training. Ensure that all dependencies are installed and correctly referenced.

## Project Structure

- `.git` - Version control directory
- `.gitignore` - Git ignore file
- `index.html` - Main HTML file for the web application
- `public` - Directory containing public assets
  - `css` - Custom stylesheets
  - `js` - Custom JavaScript files
- `Yolov9_model.ipynb` - Script to train model

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgements

- [Roboflow](https://roboflow.com/)
- [OpenCV](https://opencv.org/)
- [PyTorch](https://pytorch.org/)
- [YOLOv9](https://github.com/SkalskiP/yolov9.git)
