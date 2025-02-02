# Machine Learning Project: Mathematical Expression Recognition

## Overview
This project explores the use of **OpenCV**, **TensorFlow**, and **Python** to segment and evaluate mathematical expressions. It leverages:

- **LSTM (Long Short-Term Memory)** for analyzing the sequential order of mathematical symbols.
- **CNN (Convolutional Neural Network)** trained to recognize digits and symbols.

By combining these approaches, the system can read an expression character-by-character, classify each component, and then produce an evaluated result.

---

## Key Components

1. **Segmentation with OpenCV**  
    - Preprocessing images to extract individual symbols and digits.  
    - Applying image processing techniques (e.g., thresholding, contour extraction) to isolate each character.

2. **Symbol Recognition using CNN**  
    - A CNN trained on digits (0–9) and various mathematical operators.  
    - Once trained, the CNN identifies each segmented character with high accuracy.

3. **Sequential Ordering with LSTM**  
    - LSTM analyzes the recognized symbols in the correct order to maintain context.  
    - Correctly interprets multi-digit numbers and operator placement.

4. **Output Evaluation**  
    - After classification, the recognized expression is evaluated.  
    - Compares the interpreted expression against expected results (ground truth).

---

## Features

- Automated pipeline for scanning images of mathematical expressions and classifying each symbol.  
- Real-time evaluation of recognized expressions.  
- Extensible framework for additional symbols or complex notation.  

---

## Getting Started

1. **Clone the Repository**  
    ```bash
    git clone https://github.com/AgVicCodes/Machine_Learning_Project.git
    ```

2. **Install Dependencies**  
    ```bash
    pip install -r requirements.txt
    ```
    Make sure you have Python 3.7+ installed.

3. **Prepare the Dataset**  
    - Place images of handwritten or typed mathematical expressions in the `data/` directory (or as specified).  
    - Extend or modify the dataset as needed for custom symbols.

4. **Training the Models**  
    - Run the CNN training script to train digit/operator recognition.  
    - Train the LSTM for sequential context.  
    - Adjust hyperparameters as needed.

5. **Running the Pipeline**  
    - Execute the main script to perform segmentation, recognition, and evaluation.  
    - Monitor the logs for debug information or performance analysis.

---

## Contributing

Contributions are welcome! Feel free to:
- Open an issue if you discover bugs or have questions.  
- Submit pull requests with improvements or new features.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

Thank you for your interest in our **Machine Learning Project** for mathematical expression recognition!
