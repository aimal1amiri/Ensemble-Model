<h1 align="center">Ensemble Classification for Monkeypox (Mpox) Detection Using Inception and NASNet</h1>

###

<h4 align="left">Abstract</h4>

###

<p align="left">This project implements an ensemble classification approach for Monkeypox (Mpox) detection using a voting mechanism that combines predictions from two advanced deep learning models: Inception and NASNet. This method leverages the strengths of both architectures to classify skin lesions across six categories with an accuracy of 93%. While computationally efficient, it struggles with ambiguous classes due to reliance on individual model outputs.</p>

###

<h2 align="left"></h2>

###

<h5 align="left">Features</h5>

###

<p align="left">Ensemble Learning: Combines predictions of Inception and NASNet using majority voting.<br>Multi-Class Classification: Includes six classes—Chickenpox, Cowpox, HFMD, Measles, Healthy, and Monkeypox.</p>

###

<h2 align="left"></h2>

###

<h5 align="left">Dataset</h5>

###

<p align="left">The dataset includes images from six skin lesion classes:<br><br>    Chickenpox<br>    Cowpox<br>    Healthy<br>    HFMD<br>    Measles<br>    Monkeypox<br><br>Preprocessing steps include:<br><br>    Resizing images .<br>    Normalization of pixel values to [0, 1].<br>    Data augmentation: rotations, flips, brightness adjustments, and cropping.</p>

###

<h2 align="left"></h2>

###

<h5 align="left">Methodology</h5>

###

<p align="left">Steps:<br><br>    Preprocessing:<br>        Resize and normalize images.<br>        Apply augmentation to increase dataset diversity.<br><br>    Model Training:<br>        Train Inception and NASNet independently on the preprocessed dataset.<br>        Optimize using dynamic learning rates (1e-3 to 1e-5) over 100 epochs with a batch size of 32.<br><br>    Ensemble Voting:<br>        During inference, both models predict class probabilities for each input image.<br>        Use majority voting to decide the final classification:<br>            If both models agree, the shared prediction is selected.<br>            If models disagree, the class with the highest combined probability is chosen.<br><br>    Classification:<br>        Predict the final class for each input image based on ensemble decisions.</p>

###

<h2 align="left"></h2>

###

<h5 align="left">Results</h5>

###

<p align="left">Classification Metrics:<br><br>    Accuracy: 93%<br>    Macro-average F1-Score: 0.93<br>    Challenges observed in ambiguous classes like Monkeypox and Chickenpox due to overlapping features.<br><br>Confusion Matrix:<br><br>    Strong diagonal dominance but minor misclassifications between similar classes.</p>

###

<h2 align="left"></h2>

###

<h2 align="left">I code with</h2>

###

<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tensorflow/tensorflow-original.svg" height="40" alt="tensorflow logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original.svg" height="40" alt="jupyter logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="40" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" height="40" alt="numpy logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/matlab/matlab-original.svg" height="40" alt="matlab logo"  />
</div>

###
