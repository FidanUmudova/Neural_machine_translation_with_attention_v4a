# Neural Machine Translation with Attention

This project implements an **Attention Mechanism** for Neural Machine Translation (NMT) and builds an Encoder-Decoder architecture using Keras/TensorFlow. The main objective of the project is to translate human-readable date formats (e.g., *"3 May 1979"*) into a standardized machine-readable format (*"1979-05-03"*).

---

##  Key Features

1. **One-Step Attention (`one_step_attention`):** 
   - Computes attention weights ($\alpha$) and the context vector based on the Bi-LSTM hidden states ($a$) and the previous hidden state of the post-attention LSTM ($s_{prev}$).
2. **Encoder-Decoder Architecture (`modelf`):**
   - Utilizes a **Pre-attention Bi-LSTM** to process the input sequence.
   - Applies the attention mechanism at each time step ($T_y$) and generates the next character via a **Post-attention LSTM cell**.
3. **Model Compilation and Training:**
   - Configured with a custom **Adam optimizer** (`lr=0.005`, `beta_1=0.9`, `beta_2=0.999`, `decay=0.01`) and the `categorical_crossentropy` loss function.

---

##  Technologies & Libraries Used

* **Python**
* **TensorFlow / Keras**
* **NumPy**

