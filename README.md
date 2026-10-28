🌱 SVC Machine Learning Classification Project
📌 Project Overview
This project applies Support Vector Classifier (SVC), a supervised machine learning algorithm, to solve a classification problem.

The project demonstrates the main stages of a machine learning workflow, including data exploration, preprocessing, feature scaling, model training, and evaluation.

🎯 Project Objectives
Understand and explore the dataset.

Identify and handle duplicate and missing values.

Prepare the features for machine learning.

Encode categorical target labels.

Split the dataset into training and testing sets.

Apply feature scaling using StandardScaler.

Train an SVC classification model.

Evaluate model performance using classification metrics.

📊 Dataset Description
The dataset contains numerical features describing the physical characteristics of dry beans.

Features may include:

Area

Perimeter

Major Axis Length

Minor Axis Length

Aspect Ratio

Eccentricity

Convex Area

Equivalent Diameter

Extent

Solidity

Roundness

Compactness

Shape Factors

Target Variable: Class

The target represents the bean variety that the model attempts to classify.

🛠️ Technologies and Libraries
Python

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook

⚙️ Machine Learning Workflow
1. Import Libraries
Import the libraries required for data analysis, visualization, preprocessing, and model evaluation.

2. Load the Dataset
Load the dataset into a Pandas DataFrame.

3. Exploratory Data Analysis (EDA)
Examine the dataset's structure, data types, statistical summaries, and target class distribution.

4. Data Cleaning
Check for missing values and duplicate records, and handle data quality issues where necessary.

5. Explore the Target Variable
Analyze the distribution of bean classes to understand the classification problem.

6. Train-Test Split
Divide the data into training and testing sets to evaluate the model on unseen observations.

7. Label Encoding
Convert categorical target labels into numerical values.

8. Feature Scaling
Apply StandardScaler to standardize numerical features, which is important for SVC because it is sensitive to feature scales.

Fit the scaler on the training data and use the same scaler to transform the test data.

9. Model Training
Train an SVC model using the scaled training features.

10. Model Evaluation
Evaluate the model using:

Accuracy Score

F1-Score

Classification Report

These metrics help assess the model's classification performance.

📈 Results
The model's final performance should be reported using the actual evaluation results obtained from the notebook.

Metric	Score
Training Accuracy	Add your result
Testing Accuracy	Add your result
Training F1-Score	Add your result
Testing F1-Score	Add your result
Note: Replace the placeholders with the actual results from your notebook.

🚀 How to Run the Project
Prerequisites
Install Python and the required libraries.

pip install numpy pandas matplotlib seaborn scikit-learn jupyter
Run the Notebook
Clone the repository:

git clone https://github.com/ae6340915-lang/ML-SVC.git
Navigate to the project directory:

cd ML-SVC
Start Jupyter Notebook:

jupyter notebook
Open 9999.ipynb and run the cells in order.

📚 Key Concepts Learned
Exploratory Data Analysis

Data Cleaning

Label Encoding

Train-Test Split

Feature Scaling

Support Vector Classification

Classification Metrics

Model Evaluation

👨‍💻 Author
Abdelrahman Elsayed

Aspiring Data Engineer | Python | SQL | Machine Learning

GitHub: ae6340915-lang

⭐ Acknowledgment
This project was developed for educational purposes to practice machine learning classification and understand the complete model development workflow.

ترفع ملف README على GitHub إزاي؟
1. أنشئ الملف
داخل VS Code، افتح مجلد مشروعك:

C:\Users\20912023100033\Downloads\9999-ML-Project
أنشئ ملفًا جديدًا باسم:

README.md
الصق المحتوى السابق واحفظه باستخدام Ctrl + S.

2. ارفع الملف على GitHub
افتح Terminal داخل مجلد المشروع ونفّذ الأوامر التالية بالترتيب:

إضافة الملف:

git add README.md
حفظ التعديلات:

git commit -m "Add project README"
رفع الملف:

git push
3. شاهد النتيجة
افتح مستودعك:


سيظهر محتوى README.md تلقائيًا أسفل قائمة الملفات.

نصيحة مهمة: قبل نشر المشروع، شغّل الـ Notebook وتأكد من نتائج الـ Accuracy وF1-Score، ثم استبدل القيم التوضيحية في قسم Results بالنتائج الحقيقية.



Pasted markdown(3).md
File
 دة المشرؤع ظبت المشرؤع READM   علية

تمام يا عبده 💪 راجعت مشروعك الفعلي، وهو تصنيف أنواع الفاصوليا باستخدام SVC (Support Vector Classifier)، وظبطت لك ملف README باللغة الإنجليزية بناءً على الكود والنتائج الموجودة في الـ Notebook، مش مجرد قالب عام. 


📄 1. حمّل ملف README الجاهز

الملف يحتوي على:

✅ وصف المشروع والهدف منه.

✅ وصف البيانات والـ 7 أنواع من الفاصوليا.

✅ خطوات تنظيف البيانات وتجهيزها.

✅ شرح LabelEncoder وStandardScaler.

✅ إعدادات نموذج SVC.

✅ نتائج Accuracy وF1-Score.

✅ جدول Classification Report.

✅ طريقة تثبيت المكتبات وتشغيل المشروع.

✅ معلومات صاحب المشروع ورابط GitHub.

📊 2. النتائج الفعلية للمشروع
المقياس	النتيجة
Test Accuracy	92.54%
Weighted F1-Score	92.54%
عدد أنواع الفاصوليا	7
عدد سجلات الاختبار	2,709
هذه النتائج مأخوذة من مخرجات الـ Notebook التي أرسلتها. 


🚀 3. ارفع README على GitHub
الخطوة الأولى: ضع الملف الذي حمّلته داخل مجلد المشروع الموجود على جهازك:

C:\Users\20912023100033\Downloads\9999-ML-Project

تأكد أن الملفات أصبحت بهذا الشكل:

9999-ML-Project/
├── 9999.ipynb
└── README.md
الخطوة الثانية: افتح Terminal داخل مجلد المشروع ونفّذ الأوامر التالية بالترتيب:

إضافة الملف:

git add README.md
حفظ التعديلات:

git commit -m "Add project README"
رفع الملف:

git push
🔗 4. شاهد مشروعك بعد التحديث
افتح مستودعك على GitHub:


بعد رفع الملف، سيظهر وصف المشروع تلقائيًا أسفل قائمة الملفات.

ملاحظة مهمة: الـ Notebook يستخدم حاليًا مسار بيانات محليًا على جهازك C:\pandas\Dry_Bean_Dataset.xlsx. لذلك، لكي يستطيع شخص آخر تشغيل المشروع، ستحتاج إلى توفير ملف البيانات أو تعديل المسار ليتناسب مع مكان وجوده. 



Library
/
README.md



🌱 Dry Bean Classification using SVC
📌 Project Overview
This project uses a Support Vector Classifier (SVC) to classify dry bean varieties based on numerical measurements of their shape and size.

The model is trained on the Dry Bean Dataset and predicts one of seven bean classes using features such as area, perimeter, axis lengths, eccentricity, compactness, and shape factors.

🎯 Objectives
Explore and understand the dataset.

Check data types, descriptive statistics, missing values, and duplicate records.

Remove duplicate rows.

Examine correlations between numerical features.

Split the dataset into training and testing sets.

Encode the target classes using LabelEncoder.

Standardize numerical features using StandardScaler.

Train and evaluate an SVC classification model.

📊 Dataset
The notebook loads the dataset from an Excel file named Dry_Bean_Dataset.xlsx.

Original dataset size: 13,611 rows and 17 columns.

Duplicate rows found: 68.

Missing values: None were found in the inspected columns.

Rows after removing duplicates: 13,543.

Target column: Class.

Number of target classes: 7.

Target Classes
BARBUNYA

BOMBAY

CALI

DERMASON

HOROZ

SEKER

SIRA

Features
The dataset contains 16 numerical features, including:

Area, Perimeter, MajorAxisLength, MinorAxisLength, AspectRation, Eccentricity, ConvexArea, EquivDiameter, Extent, Solidity, roundness, Compactness, and ShapeFactor1 through ShapeFactor4.

🛠️ Tools and Libraries
Python

Jupyter Notebook

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

⚙️ Workflow
Load the data from Dry_Bean_Dataset.xlsx.

Explore the data using head(), info(), columns, and describe().

Clean the data by identifying and removing duplicate rows and checking missing values.

Analyze correlations between numerical features using a correlation heatmap.

Separate features and target: Class is the target variable.

Split the data into training and testing sets with an 80/20 split, using random_state=42 and stratification.

Encode target labels with LabelEncoder.

Scale features with StandardScaler, fitting the scaler on the training set and transforming the test set with the same scaler.

Train the model using SVC(kernel="rbf", C=10, gamma=0.1, random_state=42).

Evaluate the model with accuracy, weighted F1-score, and a classification report.

🤖 Model Configuration
SVC(kernel="rbf", C=10, gamma=0.1, random_state=42)
kernel="rbf": uses the Radial Basis Function kernel to model non-linear decision boundaries.

C=10: sets the regularization strength trade-off.

gamma=0.1: controls how far the influence of each training sample reaches.

📈 Results
The reported results from the notebook are:

Metric	Score
Test Accuracy	92.54%
Weighted F1-Score	92.54%
Classification Report
Bean Class	Precision	Recall	F1-Score	Support
BARBUNYA	0.93	0.91	0.92	265
BOMBAY	1.00	1.00	1.00	104
CALI	0.92	0.94	0.93	326
DERMASON	0.92	0.93	0.92	709
HOROZ	0.97	0.94	0.95	372
SEKER	0.94	0.95	0.95	406
SIRA	0.88	0.87	0.88	527
Overall accuracy	

0.93	2,709
Macro average	0.94	0.94	0.94	2,709
Weighted average	0.93	0.93	0.93	2,709
🚀 How to Run
1. Clone the repository
git clone https://github.com/ae6340915-lang/ML-SVC.git
cd ML-SVC
2. Install dependencies
pip install numpy pandas matplotlib seaborn scikit-learn openpyxl jupyter
3. Add the dataset
Place Dry_Bean_Dataset.xlsx in the location expected by the notebook, or update the notebook's pd.read_excel(...) path to match where you saved the file.

4. Open the notebook
The notebook file is named 9999.ipynb. Start Jupyter:

jupyter notebook
Then open 9999.ipynb and run the cells in order.

📁 Repository Contents
9999.ipynb — notebook containing data exploration, preprocessing, model training, and evaluation.

README.md — project documentation.

Dataset note: The notebook currently uses a local Windows path (C:\\pandas\\Dry_Bean_Dataset.xlsx). To make the notebook reproducible on another computer, use a relative path or upload the dataset to the repository if its license and size allow it.

👨‍💻 Author
Abdelrahman Elsayed

Aspiring Data Engineer | Python | SQL | Machine Learning

GitHub: ae6340915-lang

This project was developed for learning and practicing machine learning classification with SVC.

