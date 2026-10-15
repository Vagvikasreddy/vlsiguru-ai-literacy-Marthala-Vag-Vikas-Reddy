# Mission 05 - Understand the Anatomy of an ML Model

## Research Question

**What happens between giving data to a Machine Learning system and getting a prediction?**

## My Understanding

When we give data to a Machine Learning system, it does not immediately know how to make the correct prediction. First we need an **algorithm**, which is basically the method or process used for learning. During training, this algorithm looks at many examples and tries to find a relationship between the input data and the expected output. While learning, it adjusts some internal values called **parameters**. After the training is completed, the learned result is called the **model**. So I understood it as: the algorithm is the learning method, parameters are the values learned during training, and the model is what we finally use for predictions.

During **training**, we already know the expected answer for the examples. The model makes a prediction and compares it with the actual target. The difference between the predicted answer and the expected answer is measured using a **loss or error measure**. If the error is high, the learning process changes the model parameters to try to reduce the error. This repeated process of adjusting the parameters to reduce the loss is called **optimization**. Once the model has been trained, we can give it new data that it has not seen before. Using the trained model to produce an output for new data is called **inference**.

## Training and Inference Flow

```text
Training Examples
(Input Features + Target Answers)
              │
              ▼
        Learning Algorithm
              │
              ▼
        Model Prediction
              │
              ▼
Prediction compared with Target
              │
              ▼
         Loss / Error
              │
              ▼
      Adjust Parameters
        (Optimization)
              │
              ▼
         Trained Model
              │
              ▼
            New Input
              │
              ▼
           Inference
              │
              ▼
          Prediction
```

## Algorithm, Model and Parameters

| Term | My Understanding |
|---|---|
| Algorithm | The method used to learn patterns from the training data. |
| Parameters | Internal values that are adjusted and learned during training. |
| Model | The learned system that we use later to make predictions. |

## Training vs Inference

**Training** is the learning stage. The system uses examples, compares its predictions with the expected answers and adjusts its parameters to reduce the error.

**Inference** happens after training. We give new input to the trained model and it produces a prediction. The model is now using what it already learned rather than going through the complete training process again.

## Simple Example

Suppose I want an ML system to estimate the delay of a design. I have previous design examples where I already know some design measurements and the actual delay.

During training, the model tries to predict the delay for these examples. If it predicts `8 ns` but the actual delay is `6 ns`, there is an error between the prediction and the real value. The training process uses this error to adjust the model parameters. After seeing many examples and repeatedly reducing the error, we get a trained model. Now I can give it the measurements of a new design and ask it to estimate the delay.

## Linear Regression

Linear regression is one simple Machine Learning method used when we want to predict a numerical value. The basic idea is to learn a relationship between an input and a numerical output from previous examples.

For example, suppose I have historical data showing a relationship between one design measurement and delay. Linear regression tries to learn a line that represents this relationship as well as possible.

```text
Previous Examples

Input                     Actual Delay
  │                            │
  └──────────┬─────────────────┘
             ▼
      Learn Relationship
             ▼
         Best-fit Line
             ▼
          New Input
             ▼
     Estimated Delay
```

Once the relationship is learned, a new input can be given to the model and it can estimate the corresponding numerical output. The important point for me at this stage is not the mathematics of finding the line, but understanding that the model is learning the relationship from examples instead of us manually writing a rule for every possible input.

## What I Learned

Before this mission, I thought an algorithm and a model were basically the same thing. Now I understand that the algorithm is the method used for learning, while the model is the result we get after learning from the training data. I also understood why error is important during training. The model needs some way to know how far its prediction is from the expected answer so that its parameters can be adjusted and the prediction can improve.
