# Lacuna Solar Survey Challenge: Satellite Imagery Detection
> Mapping sustainable energy infrastructure through high-precision Computer Vision.

## 🌍 Project Overview
Identifying renewable energy infrastructure at scale is critical for tracking global sustainability goals and expanding clean energy grids. This project tackles the Zindi Lacuna Solar Survey Challenge by developing a robust Computer Vision pipeline to detect solar panels from raw satellite and aerial imagery. The resulting model serves as a scalable solution for governments and energy providers to autonomously map and monitor decentralized solar assets.

## 🚀 Key Highlights
* **High-Precision Detection**: Engineered a model achieving strong IoU (Intersection over Union) and F1 scores in detecting small-scale solar installations.
* **Robust Preprocessing Pipeline**: Applied advanced image augmentation and normalization techniques to handle diverse lighting, weather, and terrain conditions in aerial data.
* **Scalable Architecture**: Developed an end-to-end inference pipeline capable of processing large volumes of high-resolution satellite imagery efficiently.
* **Data-Centric Approach**: Handled severe class imbalances and noisy annotations through targeted oversampling, strategic data splitting, and careful validation.

## 📊 Dataset Description
The dataset consists of high-resolution aerial imagery paired with structured annotations, sourced from the Zindi platform.

* `Train.csv` / `Test.csv`: Structured metadata mapping image IDs to target variables and bounding box/segmentation coordinates.
* `images/`: Raw satellite and aerial images varying in resolution, geographical location, and lighting conditions.
* `SampleSubmission.csv`: Standardized format for evaluating model predictions against the unseen test set.

## 🔬 Approach & Methodology
Our methodology emphasizes data quality and model generalization across varying geographies:

* **Data Preprocessing**: Standardized image resolutions, normalized pixel intensities, and handled missing values in structured metadata.
* **Image Augmentation**: Implemented dynamic transformations (rotations, flips, contrast adjustments) to prevent overfitting and improve generalization.
* **Model Selection**: Leveraged transfer learning with state-of-the-art CNN architectures (e.g., ResNet, EfficientNet) adapted for object detection/segmentation.
* **Training Strategy**: Utilized stratified K-Fold cross-validation to ensure model stability across distinct geographical distributions.

## ⚙️ Tech Stack
* **Languages**: Python
* **Machine Learning & Vision**: Scikit-Learn, TensorFlow / PyTorch, OpenCV
* **Data Manipulation**: Pandas, NumPy
* **Visualization**: Matplotlib, Seaborn
* **Environment**: Jupyter Notebook

## 📈 Results & Insights
* **Performance**: Achieved highly competitive accuracy/F1-score on the validation set, demonstrating strong generalization to unseen geographies.
* **Key Finding**: Heavy data augmentation combined with a tailored learning rate schedule proved critical in overcoming severe background noise.
* **Challenge Overcome**: Handled extreme variations in solar panel sizes (from residential rooftops to utility-scale farms) using feature pyramid networks and multi-scale training.

## 📂 Project Structure
```text
lacuna-solar-detection/
├── data/
│   ├── images/                 # Raw aerial and satellite images
│   ├── Train.csv               # Training labels and metadata
│   ├── Test.csv                # Test metadata
│   └── SampleSubmission.csv    # Submission format
├── notebooks/
│   ├── 01_EDA.ipynb            # Exploratory Data Analysis
│   ├── 02_Preprocessing.ipynb  # Image augmentation and feature engineering
│   └── 03_Modeling.ipynb       # Model training and evaluation
├── src/
│   ├── dataset.py              # Custom data loaders
│   ├── models.py               # Model architectures and weights
│   └── utils.py                # Helper functions and metrics
├── README.md                   # Project documentation
└── requirements.txt            # Dependency configuration
```

## 🛠️ How to Run the Project
1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/lacuna-solar-detection.git
   cd lacuna-solar-detection
   ```
2. **Set Up the Environment**
   ```bash
   pip install -r requirements.txt
   ```
3. **Download Data**
   Place `Train.csv`, `Test.csv`, `SampleSubmission.csv`, and the `images/` folder inside the `data/` directory.
4. **Execute the Pipeline**
   Launch Jupyter Notebook and run the sequence in the `notebooks/` directory to train and evaluate the model.
   ```bash
   jupyter notebook
   ```

## 🖼️ Visuals & Predictions

![Dataset Overview Placeholder](https://via.placeholder.com/800x400?text=Exploratory+Data+Analysis+Insights)

![Model Predictions Placeholder](https://via.placeholder.com/800x400?text=Model+Predictions+vs+Ground+Truth)

## 🏢 Case Study: Business Impact
Accurate, automated solar panel detection transforms how organizations manage energy infrastructure:
* **Energy Utility Companies**: Can dynamically forecast decentralized energy supply based on mapped residential and commercial solar adoption.
* **Governments & Planners**: Gain real-time visibility into renewable energy growth to inform public policy and grid modernization investments.
* **Climate Initiatives**: Can track global progress toward carbon neutrality with objective, high-frequency satellite data.

## 👤 About Me
**Boniface Thuo Mwaura**
*Data Scientist | AI Specialist*

I specialize in building intelligent, scalable machine learning solutions that bridge the gap between complex raw data and actionable business impact. With expertise in Computer Vision, predictive modeling, and data pipelines, I focus on solving real-world challenges efficiently and elegantly.

## 📬 Portfolio & Contact
* **Portfolio**: [boniface-thuo-m-portifolio.vercel.app](https://boniface-thuo-m-portifolio.vercel.app/#about)
* **GitHub**: [https://github.com/Bonifacethuo](#)
* **LinkedIn**: [https://www.linkedin.com/in/boniface-thuo-52ab3816a/(#)
* **Email**: [bonithuo@gmail.com]

## 🤝 Call to Action
Open to exciting Data Science and ML engineering opportunities. Let's connect to discuss how my expertise in Machine Learning and Computer Vision can drive value for your team! Feel free to reach out via LinkedIn or Email.
