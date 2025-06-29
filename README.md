
# Sericulture Disease Detection using CNN

---

## **Project Overview**

This project focuses on early disease detection in silkworms using Convolutional Neural Networks (CNN). Diseases like Grasserie severely impact silk yield and quality, making early intervention critical. By leveraging deep learning and image processing techniques, this system detects infected silkworms based on visual symptoms, enabling timely action for improved sericulture health and productivity.

> **Note:** The dataset used in this project is not uploaded to this repository due to size limitations (305MB). Please download it from the following link:
> [Roboflow Silkworms Dataset](https://universe.roboflow.com/sericulturenew/silkworms/dataset/3)
>
> After downloading, extract the ZIP file and update the file paths accordingly in the `.ipynb` notebook.

---

## **Key Features**

- **Image-Based Classification**: Uses CNN to distinguish between healthy and diseased silkworms.
- **Preprocessing Pipeline**: Applies grayscale conversion, resizing, normalization, and noise reduction.
- **Training & Validation**: Model trained on labeled images of healthy and Grasserie-affected worms.
- **Integration Ready**: Can be embedded into Node-RED or any real-time system for continuous health monitoring.

---

## **Dataset**

- **Source**: Roboflow Silkworm Disease Dataset
- **Images**: Healthy and diseased silkworms captured in various orientations and lighting
- **Preprocessing**:
  - Resize to 128x128 pixels
  - Convert to grayscale
  - Apply Gaussian blur and normalization

---

## **Model Architecture**

- Input Layer: 128x128 grayscale images
- Convolutional Layers with ReLU activation
- MaxPooling for dimensionality reduction
- Dense Layers with dropout for regularization
- Output Layer: Softmax for binary classification

---

## **Usage**

1. **Clone Repository**
```bash
git clone https://github.com/yourusername/silkworm-disease-detection.git
cd silkworm-disease-detection
```

2. **Install Dependencies**
```bash
pip install -r requirements.txt
```

3. **Download Dataset**
Go to [Roboflow Dataset Page](https://universe.roboflow.com/sericulturenew/silkworms/dataset/3), download the ZIP file, and extract it into a `data/` folder. Update paths in `Silkworm_Disease_Detection.ipynb` as needed.

4. **Train the Model**
Open the notebook and run all cells to preprocess data, train, and evaluate the CNN model.

---

## **Example Results**

| Metric     | Value   |
|------------|---------|
| Accuracy   | 96.4%   |
| Precision  | 95.8%   |
| Recall     | 96.9%   |
| F1-Score   | 96.3%   |

---

## **Future Work**

- Extend dataset with real-time captured images
- Deploy model using edge devices (ESP32-CAM + Raspberry Pi)
- Integrate alerts and automation based on disease detection

---

## **License**

MIT License

---

**Contact:** For issues or contributions, please create an issue in this repository.
