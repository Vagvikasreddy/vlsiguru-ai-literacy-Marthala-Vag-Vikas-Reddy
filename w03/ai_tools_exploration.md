# AI Tools Exploration

## Tools explored

- **ChatGPT:** beginner explanations, code walkthroughs and quizzes.
- **Gemini:** comparison of explanations and Google learning resources.
- **Claude:** longer technical explanations and writing review.
- **NotebookLM:** questions over my Week 2 assignment and ML sources, with source-grounded answers.
- **Perplexity:** technical research and discovery of follow-up sources.

## Same-question comparison

I asked ChatGPT and Gemini: **Why do training, validation and test datasets have different purposes?** ChatGPT gave a step-by-step beginner explanation with an example. Gemini gave a shorter explanation and connected it to Google ML resources. Both agreed that training data fits parameters, validation data supports development decisions and test data is reserved for a final estimate.

## Prompt refinement

Initial prompt: `Explain neural networks.`

Improved prompt: `Explain a feed-forward neural network to a beginner using a semiconductor defect-inspection example. Define inputs, weights, bias, activation, output and loss. Use a numbered explanation, one limitation and two self-check questions.`

Adding context, audience, constraints and an output format made the answer more useful.

## NotebookLM experiment

I supplied my Week 2 assignment and an introductory ML source, asked about validation versus test data, opened the cited passages and checked the answer against the sources. I also asked about a topic not covered by the sources and treated that response as unsupported until another reliable source was found.

## Verified claim

Test data should not be repeatedly used to guide training decisions because this can make performance look better than it really is. The [Google ML Crash Course discussion of overfitting](https://developers.google.com/machine-learning/crash-course/overfitting) supports keeping validation and test purposes separate.
