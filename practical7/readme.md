# 🤖 Model Deployment in Browser using TensorFlow.js

## 👤 Author

**Yash Kapse**

---

## 📌 Project Overview

This project demonstrates how to deploy a machine learning model directly in the browser using TensorFlow.js. It includes training a model, saving it locally, reloading it, exporting it as files, and re-importing it to verify prediction consistency.

---

## 🎯 Objectives

* Train a simple machine learning model in the browser
* Save the trained model in browser storage
* Reload the saved model and verify predictions
* Export the model as downloadable files (`.json` and `.bin`)
* Import the model from files and test predictions again
* Compare outputs across original, loaded, and imported models

---

## ⚙️ Technologies Used

* HTML, CSS, JavaScript
* TensorFlow.js
* Browser Local Storage / IndexedDB
* File Upload API

---

## 🧠 Model Description

A simple linear regression model is used:

[
y = 2x
]

The model learns the relationship between input `x` and output `y`.

---

## 🔄 Workflow

### 1️⃣ Training

* Create a sequential model
* Train using sample data
* Example:

  * Input: `[1,2,3,4,5]`
  * Output: `[2,4,6,8,10]`

---

### 2️⃣ Saving the Model

Two methods are used:

#### ✔ Browser Storage

```js
model.save('localstorage://my-model')
```

#### ✔ File Download

```js
model.save('downloads://my-model')
```

Downloaded files:

* `my-model.json` → Model structure
* `my-model.weights.bin` → Model weights

---

### 3️⃣ Reloading the Model

```js
tf.loadLayersModel('localstorage://my-model')
```

* Loads model from browser storage
* Used to verify persistence

---

### 4️⃣ Importing Model from Files

```js
tf.loadLayersModel(tf.io.browserFiles([jsonFile, binFile]))
```

* Upload `.json` and `.bin` files
* Reconstruct model in browser

---

### 5️⃣ Prediction

* Input value is provided by user
* Model predicts output
* Compared across:

  * Original model
  * Reloaded model
  * Imported model

---

## 📊 Results

Example Output:

```
Original: 14.02 | Loaded: 14.01 | Imported: 14.02
```

✔ Predictions are nearly identical
✔ Confirms successful deployment and portability

---

## ⚠️ Common Issues & Fixes

### ❌ Error: Weight file not provided

**Cause:** Filename mismatch
**Fix:** Ensure:

```
my-model.json
my-model.weights.bin
```

---

### ❌ File renamed automatically

Example:

```
my-model.weights (1).bin
```

**Fix:** Rename to:

```
my-model.weights.bin
```

---

### ❌ Only JSON uploaded

**Fix:** Upload both `.json` and `.bin` together

---

## 🚀 How to Run

### Step 1: Save File

```bash
index.html
```

### Step 2: Run in Browser

Use:

* VS Code Live Server
  OR

```bash
python -m http.server
```

---

### Step 3: Perform Tasks

#### ✔ Task 1

* Train → Save → Predict

#### ✔ Task 2

* Load model → Predict → Compare

#### ✔ Task 3

* Upload files → Import → Predict

---

## ⚖️ Comparison

| Model Type | Source             | Accuracy |
| ---------- | ------------------ | -------- |
| Original   | In-memory          | High     |
| Reloaded   | localStorage       | Same     |
| Imported   | Files (.json/.bin) | Same     |

---

## 🔮 Future Improvements

* Use real-world datasets
* Add graphical visualization
* Deploy model on web server
* Integrate with image/text models

---

## ✅ Conclusion

This projec
