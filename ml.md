### What is Machine Learning?
- AI is the broad capability of machines to perform tasks using human-like intelligence.
- ML, a subset of AI, enables computers to learn from data and improve without explicit programming.

### Types of Machine Learning
- **Supervised Learning**: Training with labeled data to predict outcomes.
- **Unsupervised Learning**: Identifying patterns and distributions without labeled outputs.
- **Reinforcement Learning**: Models learn to maximize rewards through trial and error, similar to training a pet.

### How is Machine Learning Different from Traditional Programming?
- Traditional problem-solving requires explicit programming and detailed analysis.
- Machine learning automates pattern recognition and adapts to data, making it more flexible and efficient.
- Example: Writing a program to detect cats in images is complex with traditional methods but streamlined with ML.

### Traditional Programming vs. Machine Learning
- In traditional programming, solutions are explicitly coded to address problems.
- In machine learning, a model is created and trained using data to predict outcomes beyond the initial dataset.
- ML automates statistical reasoning and pattern-matching.

### Stages in Machine Learning
1. **Model Creation**: The initial framework or code representing potential solutions.
2. **Model Training Algorithm**: Adjusts model parameters based on data to achieve specific goals.
3. **Model Inference Algorithm**: Uses the trained model to make predictions or solve real-world problems.

### Example of How ML is Used
- A machine learning model is a flexible program shaped by data, used to solve specific problems.
- It undergoes training to adjust parameters, enabling it to make predictions effectively.

### Model Training Algorithms
- Model training involves an interactive process:
  1. **Inspection**: Evaluating the raw model and planning necessary changes.
  2. **Modification**: Adjusting the model to better meet the goal.
  3. **Iteration**: Repeating the process to refine the model until satisfactory results are achieved.

---

### Steps in Machine Learning

#### Step 1: Define a Specific Problem
- Begin with a precise question, such as whether an upcharge increases snow cone sales, instead of a broad question like "How do I increase sales?"

#### Step 2: Identify the Machine Learning Task
- Choose between **Supervised Learning** (using labeled data) and **Unsupervised Learning** (using unlabeled data).

#### Step 3: Understand the Data Needed for Training
- **Labeled Data**: Contains solutions or labels (e.g., predicting the number of snow cones sold using temperature data).
- **Unlabeled Data**: Lacks solutions or labels (e.g., identifying images of trees or clustering books by microgenres).

### Machine Learning Tasks

#### Supervised Learning
- **Classification**: Predicting categorical labels (e.g., identifying the type of flower from images).
- **Regression**: Predicting numerical values (e.g., the number of snow cones sold based on temperature).

#### Unsupervised Learning
- **Clustering**: Grouping data points based on natural similarities (e.g., grouping books by microgenres).

### The Four Aspects of Working with Data

#### Data Collection
- Methods range from simple SQL queries to complex web scraping.
- Essential question: Does the collected data match the defined machine learning task and problem?

#### Data Inspection
- Critical for ensuring high-quality data, affecting model performance.
- Check for outliers, missing values, and data that needs transformation or preprocessing.

#### Summary Statistics
- Use statistical tools to align data with model assumptions.
- Calculate metrics like mean, inner-quartile range (IQR), and standard deviation to understand dataset characteristics.

#### Data Visualization
- Helps identify outliers and trends.
- Useful for stakeholder communication through graphs and plots.

---
### Model Training Process

#### Step 1: Split the Dataset
- **Purpose**: To evaluate the model against the bias-variance trade-off before production.
- **Datasets**:
  - **Training Dataset**: Majority of data (~80%) used to train the model.
  - **Test Dataset**: Held-out data used to test the model’s generalization to new data.

#### Model Training Workflow
1. **Feed the Training Data into the Model**.
2. **Compute the Loss Function**: Measure the model's deviation from the goal.
3. **Update Model Parameters**: Adjust parameters to reduce the loss.

- **Stop Condition**: The process continues until a predefined condition is met (e.g., training time, number of cycles).

### Key Concepts in Model Training

- **Model Parameters**: Configurations updated by the training algorithm to change model behavior (e.g., weights in neural networks).
- **Loss Function**: A metric that quantifies the distance between the model’s predictions and the actual outcomes.

### Practical Advice for Model Training

- Use machine learning frameworks with pre-built models and algorithms.
- **Model Selection**: Test different models to find the best solution for your problem.
- **Hyperparameters**: Settings that affect model training but are not updated during training (e.g., number of clusters).
- **Iteration**: Be prepared to iterate, as machine learning is rarely an exact science.

### Types of Models

#### Linear Models
- **Description**: Simple models describing the relationship between inputs and outputs through a linear function (e.g., y = mx + b).
- **Use Case**: Often used as a baseline for comparison with more complex models.

#### Tree-Based Models
- **Description**: Models that categorize or regress by creating a structure of nested if/else blocks.
- **Example**: XGBoost is a commonly used tree-based model with enhancements.

#### Deep Learning Models
- **Description**: Based on the structure of the human brain, using neurons connected by weights.
- **Noteworthy Types**:
  - **FFNN (Feed Forward Neural Network)**: Layers of neurons connected by weights.
  - **CNN (Convolutional Neural Networks)**: Commonly used for image processing.
  - **RNN/LSTM (Recurrent Neural Networks/Long Short-Term Memory)**: Effective for processing sequences of data.
  - **Transformer**: Modern architecture for handling large datasets involving sequences of data.

### Machine Learning Libraries

- **Classical Models**: Use scikit-learn for linear, tree-based models, and common ML tools.
- **Deep Learning**: Libraries like mxnet, TensorFlow, and PyTorch are commonly used.

### Model Evaluation

#### Model Accuracy
- **Definition**: The fraction of predictions a model gets right.
- **Example**: Evaluating how often a flower species is correctly identified by the model.

#### Using Log Loss
- **Description**: Measures the model’s uncertainty about a prediction.
- **Example**: Evaluating how certain the model is that a customer will buy a t-shirt or a jacket.

### Iterative Nature of Machine Learning
- **Continuous Monitoring**: After deployment, continuously monitor the model’s performance.
- **Reevaluation**: Be ready to revisit the data, modify parameters, or change the model type as needed.

---
