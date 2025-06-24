NeuroMind-Simulator

Project Title

Reading Memory & Emotion from Brainwaves: A Simulation of Thought Recognition Using FFT, ERP, and ML

Description

This project explores the intriguing possibility of recognizing specific thoughts or emotional memories from brainwave (EEG-like) data, particularly for individuals who may be unconscious or in a coma. It is a simulation-based proof-of-concept for an empathy-driven Neuro-AI system.

We simulate EEG-like signals for a fictional individual, "Shiny," whose emotional landscape includes family, friends, and personal interests like vivid dreams and Netflix.

Features & Methodology
This simulation project leverages key signal processing and machine learning techniques:

FFT (Fast Fourier Transform) Analysis: Explores the frequency spectrum of simulated brainwaves for different emotional categories, revealing distinct "signatures."
![image](https://github.com/user-attachments/assets/0445014e-961c-4b97-9218-b8375caa11af)

Visualized through power spectral density plots.

ERP (Event-Related Potential) Simulation: Incorporates simulated neural spike responses that occur after specific delays, mimicking the brain's reaction to discrete events (e.g., recognizing a name).
![image](https://github.com/user-attachments/assets/1e3af568-4b1b-4fb6-b269-e931b4a4932a)

Visualized in both time-domain and frequency-domain plots.

Time-Domain EEG Signal Visualization: Presents the raw-like simulated brainwave signals over time for intuitive understanding of the simulated events.
![image](https://github.com/user-attachments/assets/1bc6b3aa-ca62-4f7d-8983-134e0f9a7c19)

SVM (Support Vector Machine) Classification: Utilizes machine learning to classify simulated thought patterns based on frequency features extracted from the brainwave data, demonstrating the potential for automated recognition.
 ML Classification with SVM
--- Classification Report ---
              precision    recall  f1-score   support

         Mom       1.00      1.00      1.00         2
     Netflix       1.00      1.00      1.00         1
      Stella       1.00      1.00      1.00         3

    accuracy                           1.00         6
   macro avg       1.00      1.00      1.00         6
weighted avg       1.00      1.00      1.00         6

---------------------------

Simulation complete. Check generated plots and classification report.
Classification report showcases high discriminative power in the simulated environment.

Conceptual Inspiration & Neuroscience Backing
This project is deeply inspired by, and aligns with, cutting-edge neuroscience research:

Emotional Memory Recognition: Real-world studies show that emotionally charged memories and stimuli evoke distinct and measurable brain responses, often detectable via EEG and fMRI. Researchers are actively working on classifying emotional states from brain activity.

Name Recognition: The brain exhibits specific electrical patterns (ERPs like P300, N400) when familiar names or significant stimuli are perceived, reflecting cognitive processes like attention and memory retrieval.

Dream Recall: While complex, specific brainwave patterns associated with REM sleep and the act of dreaming are identified, and scientists are exploring neural correlates of conscious experience during sleep.

Communication in Unresponsive Patients: The core motivation of this project aligns with a significant area of BCI (Brain-Computer Interface) research. Scientists are developing EEG-based methods to detect signs of consciousness and facilitate "covert" communication (e.g., inferring "yes/no" answers from distinct brain activity patterns) in patients in vegetative or minimally conscious states.

Getting Started
Prerequisites
Ensure you have Python 3.x installed.

Installation
Clone the repository:

git clone https://github.com/thomaglads/NeuroMind-Simulator.git
cd NeuroMind-Simulator

Create a virtual environment:

python -m venv venv
# On Windows:
# .\venv\Scripts\activate
# On macOS/Linux:
# source venv/bin/activate

Install dependencies:

pip install -r requirements.txt

How to Run
To run the simulation and generate the plots and classification report:

python src/simulation.ipynb # If using Jupyter Notebook
# OR
# python src/simulation.py # If you converted it to a .py script

The plots will be displayed, and the classification report will be printed to your console.

Results
The simulation successfully demonstrates:

Distinct frequency spectra for different simulated thoughts/emotions.

The clear presence of simulated ERP spikes time-locked to events.

A high (often perfect in simulation) classification accuracy by the SVM model, indicating that the simulated features are discriminable.
(Note: In real-world EEG, perfect accuracy is highly unlikely due to signal complexity and noise, but this simulation provides a strong conceptual foundation.)

Next Steps & Future Work
We plan to enhance this project by:

Incorporating Real EEG Data: Validating the simulation concepts using publicly available EEG datasets (e.g., from PhysioNet) or data from consumer-grade devices (e.g., Muse Headband).

Advanced Machine Learning: Exploring deep learning models like Convolutional Neural Networks (CNNs) for more sophisticated pattern recognition.

Refining Dream vs. Random Thought Comparison: Developing more nuanced simulations for distinct brain states related to dreaming versus general cognition.

Technologies Used
Python 3.x

NumPy

Matplotlib

SciPy

scikit-learn

License
This project is licensed under the MIT License - see the LICENSE file for details.

Author-

Thoma Glads Choppala 

Acknowledgements
Inspired by cutting-edge neuroscience research in brain-computer interfaces and cognitive electrophysiology.
