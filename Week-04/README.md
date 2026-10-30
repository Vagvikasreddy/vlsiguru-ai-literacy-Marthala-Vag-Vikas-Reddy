# Week 04 - Data and Deep Learning Foundations

## Mission 1 - Data behind deep learning

Flow: Raw inspection images → Data preparation → Labelled dataset → Training → Trained model → Prediction → Evaluation.

Raw camera images are numerical pixel arrays. Preparation may resize, clean, format and normalise them. Each image receives a reviewed label such as defect or no-defect. Training uses labelled examples to calculate loss and update model parameters. A trained model predicts on new images, and evaluation compares those predictions with known labels using accuracy, precision, recall, confusion matrices and false-negative rates.

Incorrect labels can teach the model the wrong patterns. Class imbalance can make the model perform well on common examples while missing rare defects. Training, validation and test data have different purposes; repeatedly using test data for decisions can make results overly optimistic.

## Mission 2 - Traditional ML versus deep learning

| Approach | How it works | Example | Limitation |
|---|---|---|---|
| Rule-based | Human-written if/then rules | Reject images below a brightness threshold | Brittle when conditions change |
| Traditional ML | Learns from human-selected features | Random forest using texture and edge features | Feature engineering may miss useful patterns |
| Deep learning | Learns representations through multiple layers | CNN classifies semiconductor inspection images | Needs data, compute and careful evaluation |

Deep learning is a part of machine learning, which is a part of AI. More layers do not automatically improve accuracy: they can increase capacity and overfitting. A simple rule or traditional model may be better when data are limited or the problem is simple.

## Mission 3 - Neural network diagram

Image pixels → [Input layer] → [Hidden layers: weights, biases and activations] → [Output layer: defect probability]

An input neuron receives a numerical pixel value. A neuron calculates a weighted sum plus a bias and applies an activation function. Hidden layers combine simple patterns into more useful representations. The output reports a score or probability, not proof that a defect exists. Lighting changes, poor labels and unseen defects can make the prediction wrong.

## Mission 4 - How a neural network learns

Input and target → Forward pass → Prediction → Loss calculation → Backpropagation → Parameter update → Repeat for batches and epochs → Evaluation on unseen data.

The forward pass uses current weights and biases to produce a prediction. The loss measures disagreement with the target. Backpropagation uses the error to calculate how the parameters affected the loss. An optimiser updates parameters to reduce future loss. One epoch means processing the training set once. Training changes parameters; inference uses fixed parameters. High training performance with poor new-data performance indicates overfitting or distribution shift. Incorrect labels provide contradictory learning signals.

## Mission 5 - Playground experiment

I explored a two-class non-linear problem in the [TensorFlow Neural Network Playground](https://playground.tensorflow.org/). I started with one hidden layer and two neurons, then changed to two hidden layers with four neurons per layer. The larger network represented a more flexible decision boundary, but added capacity did not guarantee better generalisation. The experiment showed why validation performance, test performance, class-specific metrics and robustness matter in addition to training loss.

## Mission 6 - Engineering case study: semiconductor defect inspection

A proposed system would classify inspection images as defect or no-defect and send uncertain cases to a human engineer. The dataset should include multiple lots, tools, lighting conditions and defect types. Engineers should remove duplicates, review labels, address imbalance and split data by lot or time to reduce leakage. A CNN could learn spatial features, with augmentation limited to realistic variation.

I would report recall, precision, false-negative rate, confusion matrix, calibration and results by lot, tool and defect type. A later held-out production period would test generalisation. Accuracy alone is unsafe when defects are rare.

The model may fail on unseen defects, sensor changes, unusual lighting or process changes. Engineers must define risk limits, approve labels, review uncertain predictions, investigate failures and decide whether deployment is safe. This is a proposed workflow, not a claim about a specific factory.

## Sources

- [Google Machine Learning Crash Course](https://developers.google.com/machine-learning/crash-course/)
- [Google - Numerical Data](https://developers.google.com/machine-learning/crash-course/numerical-data)
- [Google - Overfitting and Generalisation](https://developers.google.com/machine-learning/crash-course/overfitting)
- [Google - Neural Networks](https://developers.google.com/machine-learning/crash-course/neural-networks)
- [TensorFlow Neural Network Playground](https://playground.tensorflow.org/)

## Reflection

Traditional ML generally depends more on human-designed features, while deep learning learns representations from raw inputs. Data preparation controls the numerical inputs, labels and distributions from which the model learns. The experiment showed that model complexity can represent richer patterns but can also overfit. I still want to learn systematic architecture selection and distribution-shift diagnosis. My masterclass question is how to complete a small image-classification experiment with proper splits and error analysis.

## Responsible use

I used AI for clarification and organisation, checked important claims against the listed sources and marked the case study as a proposed workflow.
