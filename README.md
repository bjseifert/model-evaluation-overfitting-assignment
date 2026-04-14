Performance Comparison
Baseline: The baseline model usually hits high training accuracy quickly but the validation loss starts to rise (overfitting). It struggles because it's just looking at raw pixels.

Improved Model: By adding Convolutional layers (Conv2D) and Data Augmentation, the model actually understands the shapes of the clothes in Fashion-MNIST. The Dropout and L2 keep the training and validation lines much closer together on the graph.

Reflection
i think Data Augmentation and Early Stopping had the biggest impact here.
Data Augmentation essentially gave the model a much bigger dataset to learn from by flipping the clothes around, which is huge for image sets.
Early Stopping is the best safety net—it stopped the training at exactly the right time before the model started "memorizing" the training data instead of actually learning it.
