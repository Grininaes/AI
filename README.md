# Summary

This project uses a CNN to classify traffic signs from the GTSRB dataset. The goal was to build an accurate and efficient model.

## Approach

- Started with a basic model (1 conv + dense layer), but it underfit (<85% accuracy).
- Improved architecture with 3 convolutional layers (32, 64, 128 filters) and ReLU activations boosted accuracy above 90%.
- Added Dropout(0.5) after the dense layer to reduce overfitting.
- Adam optimizer with a `0.001` learning rate performed best.
- Downscaled images to `30x30` for faster training without loss in accuracy.
- Used ReLU in hidden layers and Softmax in the output layer.

## Results

- Final model: 3 conv layers + pooling + dropout + dense
- Balanced speed, accuracy, and generalization
