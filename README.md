# 🏠 Real Estate Price Prediction

This project demonstrates the step-by-step process of building a **Real Estate Price Prediction** website. It combines data science, machine learning, and web development concepts to create a fully functional application for predicting property prices based on user inputs. The project is designed to enhance understanding of data science workflows and web technologies. 🚀

---

## 📌 Project Overview

The project is divided into three main components:

1. **Model Building** 🧠:  
   - Build a predictive model using **Linear Regression** from the **Bangalore Home Prices dataset** obtained from [Kaggle](https://www.kaggle.com/).  
   - Key concepts covered include:
     - Data loading and cleaning 🧹
     - Outlier detection and removal 🚫
     - Feature engineering 🔧
     - Dimensionality reduction 📉
     - Model evaluation using **k-fold cross-validation** ✅
     - Hyperparameter tuning using **GridSearchCV** 🎛️

2. **Backend Development** 🔙:  
   - Create a **Python Flask** server to handle HTTP requests.  
   - Serve predictions from the saved machine learning model via an API.  

3. **Frontend Development** 🎨:  
   - Build a user-friendly website using **HTML**, **CSS**, and **JavaScript**.  
   - Enable users to input details like area (in square feet), number of bedrooms, etc., and retrieve the predicted property price.

---

## 💻 Technologies and Tools Used

1. **Python** 🐍: Programming language for model development and server-side programming.  
2. **Numpy** and **Pandas**: For data manipulation and cleaning.  
3. **Matplotlib** 📊: For data visualization.  
4. **Scikit-learn (Sklearn)**: For machine learning and building predictive models.  
5. **Jupyter Notebook** 📓: For exploratory data analysis and model development.  
6. **Visual Studio Code (VS Code)** and **PyCharm**: Integrated Development Environments (IDEs).  
7. **Flask** 🌐: A lightweight web framework for backend development.  
8. **HTML**, **CSS**, and **JavaScript**: For creating the website's frontend.

---

## 🔄 Project Workflow

### 1. **Data Science Pipeline** 📈:
   - Load the dataset from Kaggle.
   - Perform exploratory data analysis (EDA) to understand the dataset.
   - Clean the data by handling missing values, removing outliers, and normalizing features.
   - Engineer features to improve model accuracy.
   - Split the data into training and testing datasets.
   - Use **Linear Regression** as the primary model.
   - Optimize the model using cross-validation and hyperparameter tuning.

### 2. **Backend Development** 🛠️:
   - Save the trained model to a file using **joblib** or **pickle**.  
   - Develop a Flask server that:
     - Loads the saved model.
     - Exposes an API endpoint to accept inputs and return predictions.

### 3. **Frontend Development** 🌟:
   - Build a clean and responsive website.
   - Use JavaScript to call the Flask API and dynamically display the predicted price.

---

## 📋 Installation and Setup

### Prerequisites
- Python 3.x installed on your system. 🖥️  
- Basic understanding of machine learning and web development.

### Steps to Run the Project Locally
1. Clone the repository:  
   ```bash
   git clone https://github.com/VedantPancholi/Real-Estate-Price-Prediction.git
   cd Real-Estate-Price-Prediction
   ```

2. Install the required Python packages:  
   ```bash
   pip install -r requirements.txt
   ```

3. Train the model:  
   - Open the `RealEstatePricePrediction.ipynb` notebook.  
   - Execute the cells to preprocess data, train the model, and save it.

4. Start the Flask server:  
   ```bash
   python app.py
   ```

5. Open the website:  
   - Navigate to `http://localhost:5000` in your web browser. 🌐  
   - Enter the property details and view the predicted price. 💰

---


## 📂 Folder Structure

```
Real-Estate-Price-Prediction/
│
├── data/                 # Dataset and related files
├── templates/            # HTML templates for the website
├── static/               # CSS and JavaScript files
├── app.py                # Flask server code
├── model/                # Trained model file
├── RealEstatePricePrediction.ipynb  # Jupyter Notebook for model building
└── README.md             # Project documentation
```

---

## 👨‍💻 Contributors

- **Vedant Pancholi**  
- [GitHub Repository](https://github.com/VedantPancholi/Real-Estate-Price-Prediction)

---

## 🚀 Future Enhancements

1. Integrate additional machine learning algorithms for better accuracy.  
2. Include advanced frontend frameworks like React or Angular for a modern UI.  
3. Deploy the application on cloud platforms like AWS or Heroku for wider accessibility. ☁️  
4. Expand the dataset to include other cities and additional features.

---

Feel free to explore, experiment, and enhance the project! ✨😊
