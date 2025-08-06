Create a single-page web app where the user can draw a digit (0–9) on a canvas, and a pre-trained MNIST model (using TensorFlow.js) predicts the digit in real time or on button click. The app should include:

1. A 280x280 white canvas where the user can draw using the mouse (with a thick black brush).
2. A "Clear" button to reset the canvas.
3. A "Predict" button that:
    - Preprocesses the canvas image to 28x28 grayscale
    - Normalizes pixel values to [0, 1]
    - Feeds the image to the model
    - Displays the predicted digit and confidence score
4. The app should load a pretrained MNIST model using `tf.loadLayersModel` from this URL:
   https://storage.googleapis.com/tfjs-models/tfjs/mnist/model.json

Requirements:
- Use plain HTML/CSS/JavaScript (no frameworks).
- Use TensorFlow.js via CDN.
- Style the app minimally so it's clean and easy to use.
- Put the prediction in a `<div id="result">` section.
- Everything should run entirely in the browser (no server/backend).