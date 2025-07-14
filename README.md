# Traffic-AI

# Traffic Sign Classifier

## Model Summary
My model consists of two Conv2D layers (32 and 64 filters) with ReLU activations, followed by max pooling. After flattening, it has one Dense layer with 128 units and dropout, followed by a softmax output layer with 43 units.

## Experiments
- Tried a single conv layer: underfit.
- Added a second conv layer: improved accuracy.
- Increased dense layer to 256: no impact.
- Dropout 0.4 gave better generalization than 0.2.

## What Worked
- Two Conv2D layers
- Dropout 0.4
- Adam optimizer with categorical crossentropy

## What Didn't Work
- More epochs (led to overfitting)
- Third Conv2D layer (no significant gain)

## Final Accuracy
- Training: 98.3%
- Testing: 95.1%

## Reflection
This project taught me how to apply CNNs to real image data and how critical architecture tuning and regularization are to avoid overfitting.
