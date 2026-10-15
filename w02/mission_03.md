
# Mission 03 - Understand the Main ML Approaches

## Research Question

**How does a system learn when it has labels, no labels, or feedback from actions?**

## My Understanding

Machine Learning systems can learn in different ways depending on what type of data and feedback are available. The main approaches are supervised learning, unsupervised learning and reinforcement learning. There is also self-supervised learning, where the training targets are created from the data itself. These approaches are different mainly because the information given to the model during learning is different.

In supervised learning, the model learns from examples where the correct answer is already provided. In unsupervised learning, there is no target answer and the system tries to find patterns or groups in the available data. Reinforcement learning is different because the system learns by taking actions and receiving rewards or penalties. Self-supervised learning creates its own training targets from the available data, such as hiding part of an input and asking the model to predict the missing part.

## Comparison Table

| Learning Approach | Training Signal | What It Produces | Example | One Limitation |
|---|---|---|---|---|
| Supervised Learning | Examples with known target labels | Predictions for new inputs | Predict whether a timing run will Pass or Fail | Requires enough good-quality labelled data |
| Unsupervised Learning | Data without target labels | Patterns, groups or structure in data | Group similar design runs | The discovered groups may not always have useful engineering meaning |
| Reinforcement Learning | Rewards based on actions | A strategy for choosing actions | Explore design choices using a reward based on PPA objectives | Learning can require many trials and a good reward definition |
| Self-Supervised Learning | Targets created from the data itself | Learned patterns or representations | Predict a hidden or next part of an input | The automatically created learning task may not directly match the final problem |

## Supervised Learning

Supervised learning is used when we already have examples along with the correct answers. For example, suppose I have previous timing runs containing frequency, voltage and temperature along with the result `Pass` or `Fail`. The model can learn the relationship between these features and the known result. After training, it can predict the result for a new timing run.

### Simple Flow

```text
Input Data + Correct Labels
            ↓
         Training
            ↓
     Model Learns Pattern
            ↓
        Trained Model
            ↓
         New Input
            ↓
        Prediction
```

Supervised learning is suitable when the required output is known and enough labelled examples are available.

## Unsupervised Learning

Unsupervised learning is used when the data does not contain target labels. Instead of learning to predict a known answer, the model tries to find structure or patterns in the data. For example, if I have information about many design runs but no categories for them, an unsupervised method could group runs that have similar characteristics.

### Simple Flow

```text
Unlabelled Data
      ↓
Model Searches for Patterns
      ↓
Similar Data is Grouped
      ↓
Patterns / Structure
```

Unsupervised learning is useful when we want to explore data and understand whether natural groups or patterns exist without already knowing the answers.

## Reinforcement Learning

Reinforcement learning works differently. An agent takes an action in an environment and receives a reward based on the result. It uses this feedback to learn which actions are useful for achieving a goal. For example, in design-space exploration, different design choices could be tried and a reward could be based on Power, Performance and Area (PPA) objectives.

### Simple Flow

```text
Agent
  ↓
Takes Action
  ↓
Environment
  ↓
Reward / Feedback
  ↓
Agent Learns
  ↓
Chooses Better Actions
```

Reinforcement learning can be useful when a problem involves a sequence of decisions and there is a way to measure whether an action moves the system closer to the required goal.

## Self-Supervised Learning

Self-supervised learning creates the training target from the data itself instead of depending on manually supplied labels. For example, part of an input can be hidden and the model can be trained to predict the missing part, or it can predict the next portion of an input.

### Simple Flow

```text
Unlabelled Data
      ↓
Create Target From the Data
      ↓
Training
      ↓
Model Learns Patterns
```

Self-supervised learning may look similar to unsupervised learning because both can start with unlabelled data, but they are not exactly the same. In self-supervised learning, the system creates a prediction task and target from the data itself. In unsupervised learning, the main goal is usually to discover patterns or structure without supplied target labels.

## When Each Approach May Be Suitable

**Supervised Learning:** Useful when I have labelled examples and want to predict a known target such as Pass or Fail.

**Unsupervised Learning:** Useful when I do not have labels and want to discover groups or patterns in the data.

**Reinforcement Learning:** Useful when a system needs to choose actions and can receive rewards based on how good those actions are.

**Self-Supervised Learning:** Useful when large amounts of unlabelled data are available and useful training targets can be created from the data itself.

## Conclusion

This mission helped me understand that supervised, unsupervised and reinforcement learning are different learning approaches and not different ML task types. The main difference is the training signal available to the system. Supervised learning uses labelled answers, unsupervised learning finds structure without labels, reinforcement learning uses rewards from actions, and self-supervised learning creates training targets from the data itself.
