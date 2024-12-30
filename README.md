# Image Classification Neural Network
This project showcases a custom-implemented deep neural network for binary image classification, written entirely in Python using NumPy. The model is trained to classify images as either containing a cat or not.
<p>
  <img src="https://user-images.githubusercontent.com/48511939/127961427-aeec8c42-8767-4f65-9d82-e47aeb6e2eaa.png", width="700" height="500"> <br/>
  You got a cat!
</p>
  
## Highlights
- **Mathematical Implementation**: All machine learning computations, including forward propagation, backward propagation, activation functions (ReLU, sigmoid), cost computation, and gradient descent, were implemented from scratch using NumPy.
- **Custom-built Neural Network**: No reliance on high-level libraries like TensorFlow or PyTorch; all components of the neural network are manually coded for transparency and understanding.
- **Performance**: Achieved 100% training accuracy and 72.5% test accuracy on a small dataset.

## Features
- **Dataset Handling**: Images are preprocessed (resized, normalized, and flattened) and automatically labeled based on file naming conventions.
- **Neural Network Architecture**: A flexible L-layer architecture using ReLU and sigmoid activations, designed for binary classification.
- **Visualization**: Cost reduction is plotted over training iterations to showcase learning progress and convergence.

## Project Workflow
**Dataset Preparation:**
- Images are resized to a uniform shape and converted into flattened feature vectors (12,288 features for 64x64 RGB images).
- Data is normalized to enhance numerical stability during training.
- Labels are generated automatically based on image file formats.

**Model Training:**
- Forward Propagation: Computes activations using manually implemented linear transformations (W·X + b) and activation functions (ReLU, sigmoid).
- Cost Computation: Uses cross-entropy loss to measure prediction error.
- Backward Propagation: Implements manual gradient computation for weights and biases.
- Gradient Descent: Updates parameters iteratively to minimize the cost function.

**Model Evaluation:**
- Predictions are made on test images using the trained model, and classification accuracy is calculated.
- Outputs are visualized, comparing model predictions with ground truth labels.

## Results
- Training Accuracy: 100.0%
- Test Accuracy: 72.5%

## How to Run
1. Clone the repository:
```bash
git clone git@github.com:AmiraliSajadi/Image-Classification-Neural-Network.git
```
2. Organize your dataset:
```
catnoncat_dataset/
├── train/
│   ├── cat1.png
│   ├── noncat1.jpg
└── test/
    ├── cat2.png
    ├── noncat2.jpg
```
3. Run the Jupyter Notebook:
```bash
jupyter notebook cat_noncat_L_layer_NN.ipynb
```
