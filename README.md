
# Tropical Storm Damage Detection 🌪️

This project focuses on developing a machine learning model for detecting damage to coastal infrastructure caused by tropical storms. Built with Python and YOLOv8, the model classifies infrastructure into four damage categories, aiding disaster response teams in improving assessment accuracy and response efficiency.

## Features ✨

- **Damage Classification**: Classifies coastal infrastructure into four categories based on severity of damage.
- **Machine Learning Model**: Uses YOLOv8 for object detection and classification.
- **Improved Accuracy**: Enhanced model accuracy from 0.34 to 0.45 with advanced image processing techniques and model evaluation tools.
- **Visualizations**: Generates damage detection results using matplotlib for better interpretability.

## Tech Stack 🛠️

- **Languages**: Python
- **Model**: YOLOv8 (You Only Look Once)
- **Visualization**: matplotlib
- **Annotation Tool**: LabelMe (for image annotation)

## Results 📊

### Confusion Matrix
Here is the confusion matrix for our model, which shows how well the classifier performed:

![Confusion Matrix](./confusion-matrix.png)

### Overall Mean Average Precision (mAP)

mAP: 0.34

![Charts](./results-chart.png)


## Setup and Installation 🚀

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/tropical-storm-damage-detection.git
   cd tropical-storm-damage-detection
   ```

2. **Install dependencies**:
   - Create a virtual environment and install required libraries:
     ```bash
     python -m venv env
     source env/bin/activate
     pip install -r requirements.txt
     ```

3. **Prepare the dataset**:
   - Use LabelMe to annotate images for training.
   - Ensure that the dataset is properly organized into training and validation sets.

4. **Run the model**:
   - Train the YOLOv8 model using the annotated dataset:
     ```bash
     python train.py --data <path_to_dataset> --model yolov8
     ```

5. **Evaluate the model**:
   - Evaluate the model's performance and visualize results with matplotlib:
     ```bash
     python evaluate.py --model yolov8 --data <path_to_test_data>
     ```

## Usage 📊

After setting up the environment and training the model, you can run the detection on new images by using:
```bash
python detect.py --image <path_to_image>
```
The model will output the detected infrastructure damage category along with visual results.

Created by: 
- [Neel Patel](https://www.linkedin.com/in/neel-h-patel1/)
- [Timothy Chae](https://www.linkedin.com/in/timmy-chae-306b371a9/)
- [Hemin Lim](https://www.linkedin.com/in/heminlim/)
