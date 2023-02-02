# First Aid Buddy

Name: Ryan Chadek
Codecademy Username: rchadek

# About
This is my Capstone project for Codecademy's "Build Chatbots with Python Capstone" course. I built a retrieval based chatbot because I'm new to Python and machine learning concepts - and I wanted to start with the easier option before tacking the more ambitious generative chatbot approach.

I call this chatbot "First Aid Buddy" and it's trained on a very basic 'firstaidintents.json' file to assist users with any questions about First Aid.

You can ask it things like "how to treat a scrape" or "how to treat a sting". Feel free to update the JSON file with more responses. 

I've included the training data in this repository. If you do make additions to the training date, you will just need to run 'train.py' in order for the app to work with those new intents and responses.

# Use Cases
My idea is that - if someone found themselves in a situation that required First Aid but they weren't sure what to do in this specific situation, they could use the First Aid Buddy chatbot to quickly get an answer.

# Techniques
I use a JSON file to train the application. The training process consists of tokenization, stemming, and ultimately we end up with a bag-of-words model of our data.

The model uses a custom feedforward NeuralNet class inherited from the PyTorch torch.nn Module base class - which consists of Linear transformations of the iinput, hidden, and output layers - along with a ReLU activation function.

The chat file itself relis on 'tkinter' to generate a GUI application for a user to interact with.

# Dependcies
nltk
numpy
json
random
PyTorch
tkinter

# Reflection







