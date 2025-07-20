#  🧵 Pattern-Sense-Classifying-Fabric-Patterns-Using-Deep-Learning

---
## 📥 Clone or Download the Project

This project classifies fabric patterns such as 
* floral
* striped
* checked
* plain
* geometric

  
using a Convolutional Neural Network (CNN) and provides a web interface for prediction using Flask.
---
## 📁 Project Structure

```plaintext
project_directory/
├── app.py
├── Data.py
├── TrainCNN.py
├── requirements.txt
├── fabric_pattern_model.h5 # generated after training
├── templates/
│ ├── index.html
│ └── result.html
```


---

## ⚙️ Setup Instructions

### 1. Clone or Download the Project

Download or clone this repository and navigate into it:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2.Create a Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate  # For Windows
# OR
source venv/bin/activate  # For macOS/Linux
```

### 3.Install Dependencies

```bash
pip install -r requirements.txt
```
---

## 📊 Dataset Preparation

Ensure your dataset is located at the following path:

D:\projectfabric\Fabric\Clothing Pattern Classification Dataset (MD-Fashion-2)_Samples


### Or update the `data_dir` path in `Data.py` to reflect your actual dataset location.

---

## 🧠 Model Training

### 1. Run the data preprocessing script:

```bash
python Data.py
```

### 2.Train the CNN model and save it:
```bash
python TrainCNN.py
```
### This will generate a fabric_pattern_model.h5 file.

⚠️ Note: Make sure variables like X_train, y_train, etc., are correctly defined or imported in TrainCNN.py.


---

## 🌐 Launch the Web App

Start the Flask web application using:

```bash
python app.py
```
### Then visit: http://127.0.0.1:5000/ in your browser to use the app.
---
🖼️ Web App Usage

* Upload a fabric image via the UI.
* The model will predict the pattern class and display the result.
---
✅ Requirements

* Python 3.7+
* TensorFlow
* Flask
* OpenCV
* NumPy
* Pillow
* scikit-learn
---
📌 Notes

* Ensure fabric_pattern_model.h5 is present before running app.py.
* The templates/ folder must contain index.html and result.html for the web interface to function.
---
🧵 Author

* Project: Pattern Sense
* Task: Classifying fabric patterns using Deep Learning
* Interface: Built with Flask
---
