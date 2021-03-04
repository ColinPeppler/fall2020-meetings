## Deploy a Machine Learning Model to the Internet!
This workshop will show you how machine learning works outside your local environment. The classification model can classify whether a sentence is positive or negative, and it will be trained on IMDB movie reviews. 

Instead of running the model locally (what we're familiar with), the model will be running on a server. All we need to do is have the server listen for a user inputted sentence at a web endpoint (eg. myurl.com/predict). Then pass the sentence received at the endpoint to our classification model.

The sentence is typed in a textbox on the client side and sent to the server's endpoint (eg. myurl.com/predict) via an HTTP request. Our server will be running in Google Colab so we'll need to use a package called ngrok for a public accessible url.

### Directions
1. Run all the cells in Workshop.ipynb
2. Copy the ngrok url from the output of the `app.run()` cell (NOTE: ngrok generates a public url for our flask server running in Google Colab)
3. Paste the ngrok url into where the url goes at **Line 40** in index.html
4. Open index.html in a browser (drag it into the browser or run `open index.html` in terminal)
5. Type in a sentence and hit the button
