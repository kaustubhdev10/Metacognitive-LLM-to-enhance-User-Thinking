# Metacognitive-LLM-to-enhance-User-Thinking

We have completed the initial stages of the Metacognitive LLM project in a structured manner. First, we set up the project environment on macOS by creating a new project folder and setting up a Python virtual environment using VS Code. Required packages including transformers, pandas, and torch were installed and their installations were verified through test scripts.

Next, we spent time understanding the problem statement based on the recent MIT study discussing how AI models influence human critical thinking. From this, we defined our project objective as designing metacognitive LLMs that enhance user thinking by integrating Socratic questioning and counter-arguments into model outputs.

Following this, we created a high-quality dataset. We designed a CSV schema with columns for id, context, question, answer, and metacognitive_prompt. A total of 50 diverse entries were compiled covering topics such as general knowledge, science, AI, and history, ensuring proper formatting and UTF-8 encoding before saving the dataset as metacognitive_questions.csv.

Finally, we tested our dataset integration with a QA pipeline. The dataset was successfully loaded into a pandas DataFrame, and we initialized the HuggingFace distilbert-base-uncased-distilled-squad QA pipeline to test it on sample questions. Outputs were printed systematically, displaying the model-predicted answer, the true answer from the dataset, and the stored metacognitive prompt to simulate final system flow.
