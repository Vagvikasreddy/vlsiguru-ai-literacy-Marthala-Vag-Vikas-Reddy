# Mission 4 - Make AI Explain Itself, Then Test It

## Objective

The objective of this mission is to understand how a Large Language Model (LLM) generates answers and to learn that AI explanations should always be verified instead of accepted blindly.

## Prompt 1

**Explain how an LLM produces an answer to my prompt.**

## Prompt 2

**Now explain it to me as a beginner using a simple example.**

## My Explanation

When I put a question to a Large Language Model (LLM), my question is the prompt. The model initially breaks the prompt down into small units called tokens. It then looks at the present prompt and the preceding conversation , termed context . The model then uses this information to forecast the most likely next token, token by token, until a complete answer is generated.

The model does not " think " or " understand " the question like a human . But it predicts the next token based on probability, depending on the patterns it learnt during training. This is why it can answer many different questions and produce natural language. However, it generates the most probable answer, without examining each fact, therefore it might sometimes create false or unsubstantiated information.
## Important Claims Verified

### Claim 1

An LLM generates responses by predicting the next token one token at a time.

**Verification Source:** OpenAI Documentation

### Claim 2

An LLM uses the prompt and conversation context while generating a response.

**Verification Source:** Google Machine Learning Crash Course

## What AI Explained Well

The AI clearly explained how prompts, tokens, and context work together to generate a response. The beginner explanation made the concept much easier to understand.

## What I Had to Clarify

The AI explanation sounded like the model understands the meaning of the question. After reading the documentation, I understood that the model predicts the next token based on learned patterns and probabilities instead of thinking like a human.

## Sources

- OpenAI Documentation
- Google Machine Learning Crash Course

## Conclusion

This mission helped me understand how a Large Language Model generates responses and why it is important to verify AI explanations using reliable sources before trusting them.
