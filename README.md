# Human_Activity_Recognition
**Human Activity Recognition (HAR) for Office Surveillance**

**🧠 Overview: **
        This project implements machine learning models to recognize common office activities from video footage, aiming to improve workplace monitoring and enhance security systems. Activities include:

            1. Walking
            2. Sleeping on Desk
            3. Typing
            4. Handshaking
            5.  Opening/Closing Door

**🎯 Objectives**

    * Automate activity recognition in office environments
    * Compare the performance of different deep learning architectures
    * Address challenges like occlusion, lighting variance, and dataset diversity

**🧰 Technologies & Tools**

    * Python, Keras, TensorFlow
    * OpenCV for frame extraction
    * NumPy, Matplotlib for data handling and visualization

**Machine Learning Models:**

    1. ConvLSTM
    2. Gated Recurrent Convolutional Neural Network (GRCNN)
    3. Long-term Recurrent Convolutional Network (LRCN)

**🗃️ Dataset**

    * Custom dataset collected from online sources (e.g., YouTube) ensuring privacy and diversity.
    * 5 activity classes, each stored as labeled video folders.
    * Preprocessing steps include frame extraction, resizing, normalization, and one-hot encoding.

🛠️ Methodology

    1. Data Preprocessing: Frame extraction, resizing, normalization
    2. Dataset Creation: Aggregating frames, labeling, and converting to numpy arrays
    3. Modeling: Training ConvLSTM, GRCNN, and LRCN architectures
    4. Evaluation: Training/testing accuracy, loss comparison, overfitting analysis

📊 Results

    * Model	Train Accuracy	Test Accuracy
    * ConvLSTM	94.47%	60.68%
    * GRCNN	98.73%	82.67%
    * LRCN	96.72%	86.17%

✅ LRCN showed the best generalization and is most suitable for real-world use.

📈 Key Takeaways

    * LRCN offers the best trade-off between accuracy and complexity.
    * Custom datasets can still perform well if curated properly.
    * Model complexity must be balanced against overfitting and computational cost.

🚀 Future Work

    * Expand to other environments like hospitals, schools, or public surveillance
    * Integrate abnormal activity detection
    * Optimize models for edge devices (low-power environments)
