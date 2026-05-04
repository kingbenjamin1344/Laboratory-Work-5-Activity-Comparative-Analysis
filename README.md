<img width="210" height="197" alt="image" src="https://github.com/user-attachments/assets/0df855c2-9670-49bd-97e2-7a2d3f0346ff" />**PART 1: Dataset Preparation**
--

- Step 1: Collect Dataset
- Step 2: Organize Dataset

**PART 2: Load Dataset in Colab**
--

<img width="456" height="91" alt="image" src="https://github.com/user-attachments/assets/9a0487c7-1f30-400a-95f4-8ded734a3fbf" />


**PART 3: Data Preprocessing**
--

<img width="369" height="327" alt="image" src="https://github.com/user-attachments/assets/4c46a992-7f08-4346-83ba-6414536b3a59" />

**PART 4: Define Pre-trained Model Function**
--

<img width="376" height="210" alt="image" src="https://github.com/user-attachments/assets/49b99453-efca-4c19-abe4-554da487e465" />

**PART 5: Load Pre-trained Models**

<img width="806" height="182" alt="image" src="https://github.com/user-attachments/assets/4baba379-5e22-4a35-9792-7ff5627cef73" />

**PART 6: Train Each Model**
--

<img width="528" height="312" alt="image" src="https://github.com/user-attachments/assets/1997f8a1-7957-46d5-9010-91175896f0a8" />
<img width="809" height="315" alt="image" src="https://github.com/user-attachments/assets/93e88570-816a-4bf0-a16f-098cc6348abd" />
<img width="788" height="310" alt="image" src="https://github.com/user-attachments/assets/2b052bc8-0dad-49e6-a24f-edcf1bb8c146" />
<img width="772" height="309" alt="image" src="https://github.com/user-attachments/assets/55af64f0-fad9-47f4-9231-b2ffcd3941b3" />

**PART 7: Evaluation Metrics (Core Requirement)**
--

<img width="549" height="211" alt="image" src="https://github.com/user-attachments/assets/08867f98-8dbb-49dd-a008-506c8f135928" />

**PART 8: Confusion Matrix Plot**
--

<img width="525" height="355" alt="image" src="https://github.com/user-attachments/assets/ffc1eeae-fe94-41a6-94d6-162fe6032315" />

**PART 9: ROC Curve & AUC**
--

<img width="466" height="384" alt="image" src="https://github.com/user-attachments/assets/8a5a2ac2-5a71-4a57-9b1d-ff5ad93ed9b2" />


**PART 10: Grad-CAM (Explainability)**
--

<img width="398" height="105" alt="image" src="https://github.com/user-attachments/assets/0dfc5823-d130-4164-ac1d-4d7ca48493aa" />


**DenseNet121**
--

<img width="258" height="211" alt="image" src="https://github.com/user-attachments/assets/2378c80b-3340-45cd-a09e-e6ad28689aa6" />
<img width="356" height="331" alt="image" src="https://github.com/user-attachments/assets/d2d1b1fd-d8a4-4b69-b526-a4468d498428" />
<img width="468" height="406" alt="image" src="https://github.com/user-attachments/assets/b28ddc53-0550-4f43-b1f6-b58b72280036" />
<img width="527" height="435" alt="image" src="https://github.com/user-attachments/assets/c35b5bd6-31e6-4a36-95d4-dcf9cf957882" />



**MobileNetV2**
--

<img width="210" height="197" alt="image" src="https://github.com/user-attachments/assets/05617a82-3a6a-4d06-9a95-394319d66128" />
<img width="419" height="368" alt="image" src="https://github.com/user-attachments/assets/ac6e4151-1b29-4157-b12c-ab7a71367b59" />
<img width="567" height="499" alt="image" src="https://github.com/user-attachments/assets/16df9caa-a238-4fdc-919c-ad27027e36a1" />
<img width="523" height="436" alt="image" src="https://github.com/user-attachments/assets/3fc47228-6845-4cf6-ac1b-aed7f4905b88" />

**EfficientNetB0**
--

<img width="235" height="182" alt="image" src="https://github.com/user-attachments/assets/4d89246c-83ac-499c-beab-a8fe720c313a" />
<img width="335" height="287" alt="image" src="https://github.com/user-attachments/assets/19bec8d3-07b4-441c-b543-43b117e5754e" />
<img width="576" height="502" alt="image" src="https://github.com/user-attachments/assets/143a62ed-a71b-446b-8540-002c259dee64" />
<img width="533" height="439" alt="image" src="https://github.com/user-attachments/assets/0d88622e-9753-44f8-a886-ad46bfce1db1" />


**PART 11: Save Models**
--

<img width="323" height="33" alt="image" src="https://github.com/user-attachments/assets/153a4d1b-a0a3-4cb4-9a02-8a44f4374e41" />


**PART 12: Performance Comparison Table**
--

<img width="525" height="435" alt="image" src="https://github.com/user-attachments/assets/fdc05ccb-c035-4f1f-944d-b07a16a0e7f7" />


**GUIDE QUESTIONS (FINAL REFLECTION)**
--
**A. Model Performance**

1. Which pre-trained model achieved the highest accuracy? Why?
DenseNet121 achieved the highest test accuracy (0.9833).
 Likely because it uses dense connections that improve feature reuse and gradient flow, leading to better learning.

2. Which model had the lowest performance? What could be the reason?
EfficientNetB0 performed the worst (Test Accuracy 0.0493, F1-score 0.05).
 Possible reasons:

- Poor training (underfitting or wrong hyperparameters)
- Data mismatch or preprocessing issues
- Model not properly fine-tuned

3. How did loss values compare across models?

Best models (DenseNet121, MobileNetV2): Low loss (~0.12–0.13 test loss)
Worst model (EfficientNetB0): Very high loss (~2.96)
Lower loss = better learning; high loss = model failed to learn patterns.
B. Evaluation Metrics

4. Why is accuracy not enough to evaluate a model?
 Accuracy ignores class imbalance and does not show:

- False positives
- False negatives
- A model can have high accuracy but still perform poorly on important classes.

5. Which model had the best F1-score? What does it indicate?
DenseNet121 (F1 = 0.99)
Indicates excellent balance between precision and recall.

6. How did Precision and Recall differ across models?

- DenseNet121: Balanced (0.99 / 0.99)
MobileNetV2: Balanced (0.97 / 0.97)
- 2nd Model: Slight imbalance (0.82 precision / 0.89 recall)
- EfficientNetB0 & 1st Model: Near zero → failed predictions

 Good models maintain balance; weak models collapse to zero.
 
**C. Confusion Matrix Analysis**

7. Which classes were frequently misclassified?
 Not explicitly shown, but based on low recall/precision:

EfficientNetB0 and 1st Model misclassified most classes.

8. What patterns did you observe in the confusion matrix? Likely patterns:

- Strong models: predictions concentrated on diagonal (correct)
- Weak models: scattered predictions (high misclassification)
- Some confusion between visually similar classes

  
**D. ROC and AUC**

9. Which model had the highest AUC score?
DenseNet121 and MobileNetV2 (AUC = 1.00)

10. What does AUC tell us about model performance?
AUC measures the model’s ability to distinguish between classes.

1.0 = perfect classifier
Higher AUC = better separability

**E. Explainability (Grad-CAM)**

11. What did Grad-CAM reveal about model decision-making?
It showed which image regions influenced predictions.

12. Did the model focus on relevant image regions?

- Strong models (DenseNet121, MobileNetV2): Yes
- Weak models: Likely focused on irrelevant areas

13. Which model produced the most meaningful heatmaps?
DenseNet121 (most accurate → most reliable focus areas)

**F. Model Comparison & Improvement**

14. Which model would you recommend for deployment? Why?
DenseNet121
Highest accuracy, F1-score, AUC, and balanced metrics.

15. How can you further improve your best-performing model?

- Data augmentation
- Hyperparameter tuning
- More training data
- Regularization (dropout, weight decay)
- Ensemble methods
  
**G. Real-World Application**

16. How can your model be applied in real-world scenarios?
 Depends on use-case, but examples:

- Medical image diagnosis
- Object detection/classification
- Quality inspection systems

17. What are the risks of deploying an inaccurate model?

- Wrong predictions → serious consequences (e.g., medical errors)
- Loss of trust
- Financial or safety risks

18. How can this system be integrated into a mobile/web app?

- Convert model (e.g., TensorFlow Lite / ONNX)
- Backend API (Flask, Laravel, Node.js)
- Frontend uploads image → API returns prediction
- Display results + confidence + Grad-CAM visualization

