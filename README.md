# Monkeypox Detection

---

## Objective

This program was created to detect monkeypox. The input for this program is an image, which will be analyzed using deep learning to determine whether the image shows a case of monkeypox or not.

---

## Conclusions
1. **Data Volume:** There are a total of 2,142 training data and 420 validation data for model training.

2. **Model Architecture:**
   - Uses a Sequential model with an EfficientNetV2B0 base.
   - The model has a total of 38,109,553 parameters, with 32,190,241 trainable parameters.
   - Several Dense layers with dropout were used to prevent overfitting.

3. **Model Training:**
   - The model was trained for 30 epochs.
   - The results of training on the validation data achieved an accuracy of 0.6905 and a loss of 0.6921.

4. **Evaluation Results:**
   - After training, the model achieved a validation accuracy of 80%.
   - Evaluation results on the test data showed that the model performed well in detecting Monkeypox (precision 58%, recall 90%) but less well in detecting other categories (precision 86%, recall 48%).
   - The overall accuracy on the test data is 67%, with an F1-score of 0.66.

The model achieved good accuracy on the validation data, particularly in recognizing Monkeypox. However, improvements are still needed, especially in enhancing recall for other categories to achieve a more balanced evaluation result. Consideration should also be given to using a newer model storage format.

---

The deployment results can be viewed at [HuggingFace](https://huggingface.co/spaces/saepulhilal/gc7)
