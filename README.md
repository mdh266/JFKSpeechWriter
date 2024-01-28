# Creating An AI Powered JFK Speech Writer
-----------------

## Part 1 
In this short post I went over how to scrape the President John F. Kennedy Library's website to create a collection of JFK speeches. I covered how to do this using [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) and upload them as text files to [Google Cloud Storage](https://cloud.google.com/storage). One thing I could have done is to use an asynchronous HTTP client [AIOHTTP](https://docs.aiohttp.org/en/stable/) to read and write using asynchronous I/O.

## Part 2
In this blog post I covered how to create a generative text model using bi-directional [gated recurrent unit (GRU)](https://en.wikipedia.org/wiki/Gated_recurrent_unit) that is trained on speeches made by President John F. Kennedy. The model was built in [Keras](https://keras.io/) using [TensorFlow](https://www.tensorflow.org/) as a back-end and I covered how to use this model to generate text based off an input string. 

The GRU model is a specific type of [Recurrent Neural Network (RNN)](https://en.wikipedia.org/wiki/Recurrent_neural_network) and models sequences. RNNs were quite popular for Natural Language Processing until around 2017/2018. More recently, Recurrent Neural Networks have fallen out of popularity for NLP tasks as <a href="https://en.wikipedia.org/wiki/Transformer_(machine_learning)">Transformer</a> and <a href="https://en.wikipedia.org/wiki/Attention_(machine_learning)">Attention</a> based methods have shown substantially better performance. Using transformers for generating text that is meant to sound like JFK would be a natural next step and will be a follow up for a future blog post!