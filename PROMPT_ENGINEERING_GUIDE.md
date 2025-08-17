# Prompt Engineering

## LLM Output Configuration

### Output Length
Reducing the output length of the LLM doesn't cause the LLM to become more stylistically or textually succinct in the output it creates, it just causes the LLM to stop predicting more tokens once the limit is reached.

### Sampling Controls
LLMs do not formally predict a single token. Rather, LLMs predict probabilities for what the next token could be, with each token in the LLM's vocabulary getting a probability.

#### Temperature
Temperature controls the degree of randomness in token selection. Lower temperatures are good for prompts that expect a more deterministic response, while higher temperatures can lead to more diverse or unexpected results.

#### Top-K and Top-P
Top-K and Top-P (also known as nucleus sampling) are two sampling settings used in LLMs to restrict the predicted next token to come from tokens with the top predicted probabilities.

Like temperature, these sampling settings control the randomness and diversity of generated text.

- **Top-K sampling** selects the top K most likely tokens from the model's predicted distribution. The higher top-K, the more creative and varied the model's output; the lower top-K, the more restrictive and factual the model's output. A top-K of 1 is equivalent to greedy decoding.

- **Top-P sampling** selects the top tokens whose cumulative probability does not exceed a certain value (P). Values for P range from 0 (greedy decoding) to 1 (all tokens in the LLM's vocabulary).

The best way to choose between top-K and top-P is to experiment with both methods (or both together) and see which one produces the results you are looking for.

#### Putting it All Together
Choosing between top-K, top-P, temperature, and the number of tokens to generate depends on the specific application and desired outcome, and the settings all impact one another.

As a general starting point, a temperature of 0.2, top-P of 0.95, and top-K of 30 will give you relatively coherent results that can be creative but not excessively so. If you want especially creative results, try starting with a temperature of 0.9, top-P of 0.99, and top-K of 40. And if you want less creative results, try starting with a temperature of 0.1, top-P of 0.9, and top-K of 20.

Finally, if your task always has a single correct answer (e.g., answering a math problem), start with a temperature of 0.

## Prompting Techniques

When creating prompts for AI models, it is helpful to provide examples.

### One-Shot and Few-Shot Prompting
A **one-shot prompt** provides a single example, hence the name one-shot. The idea is the model has an example it can imitate to best complete the task.

A **few-shot prompt** provides multiple examples to the model. This approach shows the model a pattern that it needs to follow. The idea is similar to one-shot, but multiple examples of the desired pattern increases the chance the model follows the pattern.

### System, Contextual and Role Prompting
System, contextual and role prompting are all techniques used to guide how LLMs generate text, but they focus on different aspects:

- **System prompting** sets the overall context and purpose for the language model. It defines the 'big picture' of what the model should be doing, like translating a language, classifying a review etc.

- **Contextual prompting** provides specific details or background information relevant to the current conversation or task. It helps the model to understand the nuances of what's being asked and tailor the response accordingly.

- **Role prompting** assigns a specific character or identity for the language model to adopt. This helps the model generate responses that are consistent with the assigned role and its associated knowledge and behavior.

### Step-Back Prompting
Step-back prompting is a technique for improving the performance by prompting the LLM to first consider a general question related to the specific task at hand, and then feeding the answer to that general question into a subsequent prompt for the specific task. This 'step back' allows the LLM to activate relevant background knowledge and reasoning processes before attempting to solve the specific problem.

### Chain of Thought (CoT)
Chain of Thought (CoT) prompting is a technique for improving the reasoning capabilities of LLMs by generating intermediate reasoning steps. This helps the LLM generate more accurate answers. You can combine it with few-shot prompting to get better results on more complex tasks that require reasoning before responding as it's a challenge with a zero-shot chain of thought.

### Self-Consistency
Self-consistency gives a pseudo-probability likelihood of an answer being correct, but obviously has high costs.

It follows the following steps:
1. **Generating diverse reasoning paths**: The LLM is provided with the same prompt multiple times. A high temperature setting encourages the model to generate different reasoning paths and perspectives on the problem.
2. **Extract the answer** from each generated response.
3. **Choose the most common answer**.

### Tree of Thoughts (ToT)
Now that we are familiar with chain of thought and self-consistency prompting, let's review Tree of Thoughts (ToT). It generalizes the concept of CoT prompting because it allows LLMs to explore multiple different reasoning paths simultaneously, rather than just following a single linear chain of thought.

The model can then explore different reasoning paths by branching out from different nodes in the tree.

### ReAct (Reason & Act)
Reason and act (ReAct) prompting is a paradigm for enabling LLMs to solve complex tasks using natural language reasoning combined with external tools (search, code interpreter etc.) allowing the LLM to perform certain actions, such as interacting with external APIs to retrieve information which is a first step towards agent modeling.

ReAct mimics how humans operate in the real world, as we reason verbally and can take actions to gain information. ReAct performs well against other prompt engineering approaches in a variety of domains.

## Automatic Prompt Engineering
At this point you might realize that writing a prompt can be complex. Wouldn't it be nice to automate this (write a prompt to write prompts)? Well, there's a method: Automatic Prompt Engineering (APE).

## Working with Schemas
Using structured JSON as an output is a great solution, as we've seen multiple times in this paper. But what about input? While JSON is excellent for structuring the output the LLM generates, it can also be incredibly useful for structuring the input you provide.
