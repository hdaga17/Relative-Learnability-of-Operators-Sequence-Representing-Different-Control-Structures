
# Relative Learnability of Operators Sequence Representing Different Control Structures

![License](https://img.shields.io/github/license/hdaga17/Relative-Learnability-of-Operators-Sequence-Representing-Different-Control-Structures)
![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![ML](https://img.shields.io/badge/ML-Control%20Structures-orange)
![Status](https://img.shields.io/badge/status-Completed-brightgreen)

## Overview
This project explores the relative learnability of different operator sequences that represent control structures like **Sequence**, **Selection**, and **Iteration**. Inspired by the **Böhm–Jacopini theorem**, the research assesses the ability of machine learning models to predict control structures, with implications for **program synthesis** and **Inductive Logic Programming (ILP)**.

## Table of Contents
1. [Project Motivation](#project-motivation)
2. [Methodology](#methodology)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Results](#results)
6. [Future Improvements](#future-improvements)
7. [Contributing](#contributing)
8. [License](#license)

## Project Motivation
In computational theory, the Böhm–Jacopini theorem asserts that any deterministic program can be represented with three control structures: Sequence, Selection, and Iteration. This project aims to:
- Evaluate the learnability of these control structures by machine learning models.
- Understand the predictive accuracy of models on different control structures.
- Apply findings to enhance **Inductive Logic Programming (ILP)** techniques.

## Methodology
The project follows these main steps:

1. **Data Preparation**:
   - Compiled and preprocessed a dataset representing different control structures in operator sequences.
   - Applied tokenization and vectorization for structured data representation.

2. **Model Training and Evaluation**:
   - Implemented various **supervised learning models** (e.g., neural networks, decision trees) to classify operator sequences.
   - Evaluated models using **accuracy metrics** to determine learnability differences across control structures.

3. **Dimensionality Reduction and Visualization**:
   - Applied **t-SNE** and **PCA** for feature space reduction and visualization.
   - Generated cluster plots to analyze model interpretations of control structures.

4. **Experimentation and Analysis**:
   - Analyzed model performance, revealing higher learnability for Selection and Iteration over Sequence.
   - Derived insights into structural differences in control learnability, with potential applications in ILP.

## Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/hdaga17/Relative-Learnability-of-Operators-Sequence-Representing-Different-Control-Structures.git
   cd Relative-Learnability-of-Operators-Sequence-Representing-Different-Control-Structures
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   python3 -m venv env
   source env/bin/activate
   pip install -r requirements.txt
   ```

## Usage
To run the learnability experiment:

1. **Data Preprocessing**: Run `data_preprocessing.py` to process and prepare the dataset.
   ```bash
   python data_preprocessing.py --input data/raw_dataset.csv --output data/processed_dataset.csv
   ```

2. **Model Training**: Execute `train_model.py` to train and evaluate models on control structure sequences.
   ```bash
   python train_model.py --input data/processed_dataset.csv --output results/
   ```

3. **Visualization**: Run `visualize_results.py` to generate t-SNE and PCA plots.
   ```bash
   python visualize_results.py --input results/ --output plots/
   ```

## Results
The project demonstrated significant findings in learnability:
- **Higher Accuracy** for Selection and Iteration compared to Sequence, suggesting differing complexity levels.
- Clustering visualizations indicated clear distinctions between structures, validating the hypothesis of relative learnability.

## Future Improvements
- **Extended Model Architectures**: Experiment with transformer-based architectures for complex sequence representations.
- **Enhanced Dataset Variety**: Include more diverse operator sequences and control structures.
- **Real-World Applications**: Apply findings to real-world programming datasets to validate implications for ILP.

## Contributing
Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request. For major changes, please open an issue to discuss your ideas.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For further inquiries, please contact the project maintainer at hdaga17.
