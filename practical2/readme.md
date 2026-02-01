<!DOCTYPE html>
<html>
<head>
  <title>MNIST Digit Recognition Practical</title>
</head>
<body>

<h1><strong>Digit Recognition using MNIST Dataset</strong></h1>
<h2><strong>using CNN</strong></h2>

<hr>

<h2><strong>Aim</strong></h2>
<p>
To implement <strong>handwritten digit recognition</strong> using the
<strong>MNIST dataset</strong> by using
<strong>Convolutional Neural Network (CNN)</strong> and
<strong>TensorFlow.js</strong>.
</p>

<hr>

<h2><strong>Tools & Technologies Used</strong></h2>
<ul>
  <li><strong>Visual Studio Code (VS Code)</strong></li>
  <li><strong>Live Server Extension</strong></li>
  <li><strong>TensorFlow.js (via jsDelivr CDN)</strong></li>
  <li><strong>HTML & JavaScript</strong></li>
  <li><strong>Google Chrome Browser</strong></li>
</ul>

<hr>

<h2><strong>Dataset Description</strong></h2>
<ul>
  <li><strong>MNIST Handwritten Digit Dataset</strong></li>
  <li><strong>Image Size:</strong> 28 × 28 pixels</li>
  <li><strong>Color:</strong> Grayscale</li>
  <li><strong>Classes:</strong> 10 (Digits 0and t–9)</li>
  <li>Dataset loaded <strong>fully on client side</strong></li>
</ul>

<hr>

<h2><strong>Methodology</strong></h2>

<h3><strong>1. Environment Setup</strong></h3>
<ul>
  <li>Installed <strong>VS Code</strong></li>
  <li>Added <strong>Live Server Extension</strong></li>
  <li>Created a single file <strong>task3.html</strong></li>
  <li>Loaded TensorFlow.js using <strong>CDN</strong></li>
</ul>

<h3><strong>2. Data Loading</strong></h3>
<ul>
  <li>MNIST images loaded as <strong>sprite image</strong></li>
  <li>Pixel values <strong>normalized (0–1)</strong></li>
  <li>Labels loaded from binary label file</li>
  <li>Used <strong>1000 samples</strong> for faster training</li>
</ul>

<h3><strong>3. Dense Neural Network Model</strong></h3>
<ul>
  <li>Flatten layer (28×28 → 784)</li>
  <li>Dense hidden layer with <strong>128 neurons</strong></li>
  <li>ReLU activation</li>
  <li>Softmax output layer</li>
  <li><strong>Optimizer:</strong> Adam</li>
  <li><strong>Loss Function:</strong> Categorical Crossentropy</li>
  <li><strong>Epochs:</strong> 5</li>
</ul>

<h3><strong>4. Convolutional Neural Network (CNN)</strong></h3>
<ul>
  <li>Convolution layer (3×3 kernel)</li>
  <li>Max Pooling layer</li>
  <li>Flatten layer</li>
  <li>Dense layer</li>
  <li>Softmax output layer</li>
  <li><strong>Optimizer:</strong> Adam</li>
  <li><strong>Epochs:</strong> 5</li>
</ul>

<hr>

<h2><strong>Training & Logging</strong></h2>
<ul>
  <li>Epoch-wise <strong>loss and accuracy</strong> displayed</li>
  <li>Logs printed on <strong>webpage</strong></li>
  <li>Detailed logs shown in <strong>browser console</strong></li>
</ul>

<hr>

<h2><strong>Visualization</strong></h2>
<ul>
  <li>Accuracy comparison shown using <strong>bar chart</strong></li>
  <li>Clear visual comparison between <strong>Dense vs CNN</strong></li>
</ul>

<hr>

<h2><strong>Results</strong></h2>
<ul>
  <li><strong>Dense Network Accuracy:</strong> 92–94%</li>
  <li><strong>CNN Accuracy:</strong> 97–99%</li>
</ul>

<hr>

<h2><strong>Conclusion</strong></h2>
<p>
The <strong>CNN model performs better</strong> than the Dense Neural Network
because it preserves <strong>spatial features</strong> of images using
convolution operations. Dense networks lose spatial information after flattening.
</p>

<hr>

<h2><strong>Applications</strong></h2>
<ul>
  <li>Handwritten Digit Recognition</li>
  <li>Optical Character Recognition (OCR)</li>
  <li>Image Classification</li>
  <li>AI-based Form Processing</li>
</ul>

<hr>

<h2><strong>Files Included</strong></h2>
<ul>
  <li><strong>task3.html</strong></li>
  <li><strong>README.html / README.md</strong></li>
</ul>

<hr>

<h2><strong>Viva Explanation (Short)</strong></h2>
<p>
This practical demonstrates handwritten digit recognition using the MNIST dataset.
A Dense Neural Network and a CNN were trained using TensorFlow.js.
CNN achieved higher accuracy due to spatial feature extraction,
and results were visualized using an accuracy comparison chart.
</p>

</body>
</html>
