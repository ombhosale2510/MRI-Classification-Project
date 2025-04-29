# AI-Driven MRI Classification System

## Overview
This project implements a deep learning-based classification system for brain MRI images, capable of identifying different types of brain tumors including glioma, meningioma, pituitary tumors, and cases with no tumors. Multiple state-of-the-art deep learning architectures are implemented and compared.

## Project Structure
```
├── data/
│   ├── processed/      # Preprocessed and cleaned dataset
│   │   ├── Testing/    # Test dataset split by tumor types
│   │   └── Training/   # Training dataset split by tumor types
│   └── raw/           # Original unprocessed dataset
├── notebooks/         # Jupyter notebooks for implementation
├── reports/          # Project documentation and results
```

## Models Implemented
- ResNet50
- DenseNet121
- GRU and LSTM models
- EfficientNet (implemented in Google Colab)

## Implementation Pipeline
1. **Data Preprocessing** (`01_preprocessing.ipynb`)
   - Image resizing and standardization to 256x256
   - Dataset organization and preparation

2. **Data Cleaning** (`02_remove_duplicates.ipynb`)
   - Duplicate image detection and removal
   - Dataset validation

3. **Model Training and Evaluation**
   - DenseNet implementation (`03_model_densenet.ipynb`)
   - ResNet implementation (`04_model_resnet.ipynb`)
   - GRU & LSTM implementation (`05_model_gru_lstm.ipynb`)
   - EfficientNet implementation (via Google Colab)

## Getting Started

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Required Python packages (requirements.txt coming soon)

### Installation
1. Clone the repository
```bash
git clone https://github.com/[username]/MRI-Classification-Project.git
cd MRI-Classification-Project
```

2. Set up a Python environment (recommended)
```bash
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
```

3. Install dependencies (requirements.txt coming soon)
```bash
pip install -r requirements.txt
```

## Usage
1. Start with the preprocessing notebook to prepare your dataset
2. Run the duplicate removal notebook if needed
3. Choose and run any of the model implementation notebooks based on your needs

## Results and Documentation
- Detailed results and analysis can be found in the [Final Report](reports/ENGG6600(04)_S24_Final_Report.pdf)
- [Presentation Slides](https://docs.google.com/presentation/d/e/2PACX-1vTvZjzgbPW7YcfcgMFaxFoe2eVweKC8iWAsJaGzSYP8PYoyeWcZveDz8tilTeSCSWw7F6rGIg2G_Q7J/pub?start=false&loop=false&delayms=3000)

## Additional Resources
- EfficientNet Implementation: [Google Colab Notebook](https://drive.google.com/file/d/1qdNURatihf_mRYdHcPtvDsPFlU1UGCHs)

## Future Improvements
- Add requirements.txt for easy dependency installation
- Implement cross-validation
- Add model performance metrics and comparisons
- Include data augmentation techniques
- Add visualization notebooks for results analysis

## License
This project is licensed under the terms of the LICENSE file included in the repository.
