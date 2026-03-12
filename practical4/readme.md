# Image Classification and Object Detection using TensorFlow.js

## Practical Title

**Image Classification with Pre-trained Models and Model Comparison in the Browser**

## Objective

To load pre-trained deep learning models in the browser using TensorFlow.js and perform image classification and object detection directly on user-uploaded images. The practical also compares the predictions of two different models.

## Technologies Used

* HTML
* CSS
* JavaScript
* TensorFlow.js (CDN)

## Pre-trained Models Used

1. **MobileNet** – Used for image classification. It predicts the main object present in an image.
2. **COCO-SSD** – Used for object detection. It detects multiple objects in an image and shows their positions using bounding boxes.

## Tasks Performed

### Task 1: Load Pre-trained Model

* TensorFlow.js was loaded using a CDN.
* The MobileNet model was loaded directly in the browser.
* An image was uploaded by the user and passed to the model for prediction.

### Task 2: Image Classification

* The MobileNet model analyzed the uploaded image.
* The model returned the **top 3 predictions** with confidence scores.
* The results were displayed on the user interface.

### Task 3: Model Comparison

* The COCO-SSD object detection model was loaded.
* The same image was processed using both models.
* MobileNet provided **classification results**, while COCO-SSD detected **multiple objects and their locations**.
* Bounding boxes were drawn around detected objects.

## Working Procedure

1. Load TensorFlow.js and model libraries using CDN links.
2. Load MobileNet and COCO-SSD models asynchronously.
3. Allow the user to upload an image.
4. Display the image on a canvas.
5. Run MobileNet to classify the image.
6. Display the top three predicted classes with probabilities.
7. Run COCO-SSD to detect objects in the image.
8. Draw bounding boxes around detected objects.
9. Display detected object names and confidence scores.

## Output

* MobileNet displays the **top 3 predicted classes**.
* COCO-SSD detects **multiple objects** in the image.
* Bounding boxes highlight detected objects on the image.

## Conclusion

The practical demonstrates how pre-trained deep learning models can run directly in a web browser using TensorFlow.js. MobileNet performs image classification by predicting the primary object in an image, while COCO-SSD performs object detection by identifying multiple objects and their locations. This comparison helps understand the difference between classification and detection models.

## Author

**Yash Kapse**
