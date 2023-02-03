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
- nltk
- numpy
- json
- random
- PyTorch
- tkinter

# Reflection
My dataset came from "First Aid Recommendations Intents" on Kaggle - which I then modified to include some basic greetings, goodbye, and thanks responses.
https://www.kaggle.com/datasets/therealsampat/intents-for-first-aid-recommendations

I based my chatbot on Patrick Loeber's YouTube series: "Chat Bot With PyTorch - NLP And Deep Learning - Python Tutorial" 
https://www.youtube.com/playlist?list=PLqnslRFeH2UrFW4AUgn-eY37qOAWQpJyg

One of the biggest challenges I found was getting PyTorch installed and then understanding how to work with that environment in VS Code. 

In regards to ethical concerns - rather than having the chatbot respond with "I don't understand" if no match to the request was found - I included a default statement telling the user: "I don't seem to have an answer for that one. If this is a life-threatening situation, you should call 911 or head to the nearest emergency room immediately."

This may seem like a simple chatbot - but I spent many hours of trial and error getting this to work how I wanted and I'm proud of how it turned out.

# Screenshots
![first-aid-buddy-01](https://user-images.githubusercontent.com/30985537/216718817-87781845-0434-499f-bba3-8ea1d9e001e4.JPG)
![first-aid-buddy-02](https://user-images.githubusercontent.com/30985537/216718822-d826d1f8-2255-4c43-98ea-b3679f2d7e68.JPG)
![first-aid-buddy-03](https://user-images.githubusercontent.com/30985537/216718826-b1b1ac27-2208-4cd7-986a-94d64c63425f.JPG)
![first-aid-buddy-04](https://user-images.githubusercontent.com/30985537/216718828-328b6b5c-bf44-4be0-b233-62e1e7590aec.JPG)
![first-aid-buddy-05](https://user-images.githubusercontent.com/30985537/216718831-5bc3245e-ef32-4b72-a28b-f814c98a9329.JPG)


