# AUTOMATIC RECIPE GENERATOR 
The Automatic Recipe Generator is a Python code that leverages the GPT-2 model, a powerful
language model, in combination with the Transformers library to automatically create detailed recipe instructions
based on a list of ingredients provided by the user. The tokenizer is configured to better suit the recipe
generation task. Then a dataset of Indian food recipes is loaded. It performs initial data preprocessing,
shuffling the dataset for variety and resetting the index. For model training, a custom dataset class
(RecipeDataset) is defined. This class tokenizes and encodes the recipe strings, generating input IDs
and attention masks.

The GPT-2 model is fine-tuned on the recipe dataset. The training process includes configuring
various training parameters and utilizing the Trainer class from Transformers. The model learns to
generate contextual relevant recipes. A function is created to generate recipes where a list of
ingredients are given as input, constructs a recipe prompt, and utilizes the fine-tuned GPT-2 model to
generate text. The generated text is returned as a complete recipe.

The Automatic Recipe Generator serves as a valuable tool for cooking enthusiasts, individuals seeking
culinary inspiration, or anyone interested in experimenting with new recipes. It demonstrates the power
of using pre-trained language models like GPT-2, fine-tuning them for specific tasks, and generating
human-like text to fulfill various natural language generation tasks, including recipe creation.
