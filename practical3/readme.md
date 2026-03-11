```html
<!DOCTYPE html>
<html>
<head>
<title>Sentiment Analysis Practical</title>

<style>
body{
font-family:Arial;
margin:40px;
background:#f5f5f5;
}

.container{
background:white;
padding:30px;
border-radius:10px;
box-shadow:0 5px 20px rgba(0,0,0,0.1);
}

h1,h2{
color:#333;
}

p{
line-height:1.6;
}

</style>
</head>

<body>

<div class="container">

<h1>Sentiment Analysis Practical</h1>

<p><b>Student Name:</b> Yash Kapse</p>
<p><b>Technology Used:</b> HTML, JavaScript, TensorFlow.js (CDN)</p>

<h2>Overview</h2>
<p>
Sentiment Analysis is a Natural Language Processing technique used to determine 
whether a sentence expresses a positive or negative emotion. 
This practical demonstrates sentiment classification using TensorFlow.js 
directly in the browser.
</p>

<h2>Task 1: Train Sentiment Classifier</h2>
<p>
A small dataset of positive and negative sentences is created. 
The sentences are converted into numerical vectors and a neural 
network model is trained using TensorFlow.js to classify sentiment.
</p>

<h2>Task 2: Test Custom Sentences</h2>
<p>
The trained model is tested using sentences entered by the user. 
The system predicts whether the sentence is positive or negative 
and displays a confidence score representing the prediction probability.
</p>

<h2>Task 3: Compare Dense vs RNN</h2>
<p>
Two models are trained: a Dense Neural Network and a Recurrent Neural Network (RNN). 
Both models analyze the same user input sentence and their predictions and 
confidence scores are compared.
</p>

<h2>Conclusion</h2>
<p>
The experiment shows how neural networks can be used for sentiment analysis. 
RNN models generally perform better for text data because they understand 
word sequences and context.
</p>

</div>

</body>
</html>
```
