# Driver_attention

This project uses a **MobileNetV2** model trained to detect whether a driver is **attentive** or **distracted**.  
It combines deep learning with **MediaPipe** to verify face detection and hand counting, allowing correction of certain inconsistent predictions.

The project uses the **StateFarm Distracted Driver** dataset, which must be downloaded manually and placed inside the `data/` directory:
https://www.kaggle.com/c/state-farm-distracted-driver-detection

Make sure to download the dataset beforehand and update the path in Google Colab if necessary.

---

##  Usage

The project is designed to be used directly on **Google Colab**.  
To test or train the model, simply run each cell of the notebook in order.

1. Open the `driver_distraction.ipynb` notebook on Google Colab.
2. Mount Google Drive if needed to access images or the dataset.
3. Run all cells in the recommended order (preprocessing, training, testing).
4. You can upload your own images to test the model.

---

##  Results

- Final validation accuracy: **~92.7%**
- The confusion matrix and performance curves are available in the notebook.

---

##  Notes

- The notebook contains all steps needed for training, evaluation, and testing.  
- Make sure the dataset is downloaded before running the notebook.  
- The model corrects certain predictions using MediaPipe (face/hands consistency check).
