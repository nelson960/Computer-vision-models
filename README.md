# Computer-vision-models
# MNIST CNN Pipeline

## 1. Load and Explore
- **Data**: MNIST dataset loaded (training and test sets).
- **Image Format**: Each image is 28×28 pixels, in grayscale.

## 2. Preprocess
- **Reshape**: Convert from 28×28 to 28×28×1 (adding the channel dimension).
- **Normalize**: Scale pixel values to the [0–1] range.

## 3. Build the Model
- **Architecture**: A **Sequential** CNN consisting of:
  1. Two convolutional–pooling blocks
  2. A fully connected (dense) layer
  3. A 10-unit **softmax** output layer for classification

## 4. Compile
- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy

## 5. Train
- **Process**: Fit the model on the training set for a chosen number of epochs
- **Monitoring**: Track accuracy and loss on the validation set

## 6. Evaluate
- **Performance**: Check model accuracy and loss metrics on the test set

## 7. Predict & Visualize
- **Inspection**: Use the trained model to make predictions
- **Examples**: Inspect and visualize a few predicted images to confirm correct classification

---

**Note**:  
This notebook demonstrates a standard CNN approach for digit classification using MNIST. Convolutional layers effectively extract spatial features from images. Since MNIST is relatively simple, even basic CNN architectures often achieve very high accuracy (98–99% or more).
