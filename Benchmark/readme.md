## Overview

The `Benchmark` folder contains **srsRANBench.json**, a JSON file tailored for assessing the performance of Large Language Models (LLMs) in code understanding and generation within the srsRAN project.

## File Structure

The JSON contains a list of questions, where each question is represented as a list:

```json
[
  [
    "Question text goes here",
    ["Option 1", "Option 2", "Option 3", "Option 4"],
    "Correct option index (1, 2, 3 or 4)"
  ],
  ...
]
```

- **Question text**: A string representing the multiple-choice question.
- **Options**: An array of strings, each representing a possible answer.
- **Correct option index**: A string representing the index of the correct answer within the options array.

### Example

Here's a Python example of how to load and use these JSON files:

```python
import json

# Load Easy questions
with open('Benchmark/srsRANBench.json', 'r') as file:
    easy_questions = json.load(file)

# Display first question
first_question = easy_questions[0]
print(f"Question: {first_question[0]}")
for i, option in enumerate(first_question[1]):
    print(f"{i+1}. {option}")
print(f"Answer: {first_question[1][int(first_question[2]) - 1]}")
```

This README file provides a comprehensive guide on the structure and usage of the JSON files within the `MCQA` folder, ensuring users can effectively utilize the resources for evaluating LLMs in O-RAN contexts.
