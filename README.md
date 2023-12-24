# AI-Quality-Control

Dylan
* Verify class distribution to determine if defective and undefective chips have roughly the same size
* Dividing everything by 255 constraints all values between 0 and 1
* Needed to resize images to prevent overfitting
     * Identify another way of scaling to prevent overfitting
* Total of 900 training samples a little limited
* Data augmentation: take an existing image and modify it through transformations
     * e
* Test the accuracy on the test set itself
     * Keep validation set (subset of training set) to prevent it is overfitting
     * At the end of the training set, run on the test set
     * Loss function is a log, undues the effect of the sigmoid (differentiable)
     * Sigmoid returns the probability between 0 and 1 (exponential function)
          * Only use Relu's in the hidden layers of the fully connected layers