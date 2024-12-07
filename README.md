# Heart Disease Prediction Using Machine Learning

### Abstract
Heart disease remains a leading cause of death worldwide, making early detection critical for saving lives and reducing healthcare costs. This study leverages the UCI Heart Disease dataset (n=303) with 14 clinical features to predict heart disease (0 = no, 1 = yes). 

We implemented and fine-tuned five machine learning models—Logistic Regression, Random Forest, XGBoost, K-Nearest Neighbors, and Support Vector Machines—evaluated using k-fold cross-validation. While Random Forest and XGBoost performed well individually, they struggled with edge cases and feature variability. To address this, we developed a hybrid model combining Random Forest and XGBoost using a soft-voting classifier. 

The hybrid model achieved:
- **Accuracy**: 90.16%
- **Precision**: 93.33%
- **AUC-ROC**: 94.40%

This hybrid approach reduced false negatives and positives compared to individual models, demonstrating the potential of ensemble models to enhance heart disease detection and enable timely interventions.

---

### Conclusion and Future Directions
Our research explored machine learning methods for heart disease prediction. While Random Forest and XGBoost were strong individual models, their limitations in handling edge cases highlighted the need for a hybrid approach. By combining these models through soft voting, the hybrid model balanced strengths, improving predictive performance and robustness.

**Key Drawbacks:** The hybrid model required longer training times compared to individual models. To address this, parallel processing with distributed libraries (e.g., TensorFlow) can optimize hyperparameter tuning without compromising accuracy.

**Future Improvements:**
1. **Dataset Expansion**: Include more diverse clinical populations to improve generalization for underrepresented groups.
2. **Advanced Features**: Add clinical risk scores and temporal patterns to enrich domain insights.
3. **Sequential Modeling**: Incorporate RNNs to analyze changes in health metrics over time, identifying early warnings.
4. **Scalability**: Embed models into wearable devices for real-time health monitoring and early detection of heart anomalies.

By integrating tools like SHAP and LIME for interpretability, clinicians can better understand model predictions. These improvements would help scale machine learning solutions for real-world clinical use, addressing healthcare challenges such as limited accessibility, rising costs, and resource shortages while improving patient outcomes.

---

### Repository Overview
- `heart-disease-prediction`: Scripts for preprocessing, model building, and evaluation.
- `Project_Report_Hanzhen_Zhu.pdf`: Detailed study report covering methods, results, and insights.
- `README.md`: Project overview and key takeaways.

---

### Highlights
- **Best Model**: Hybrid ensemble (Random Forest + XGBoost) with an AUC-ROC of 94.40%.
- **Innovation**: Combined and balanced complementary algorithms in the hybrid ensemble model to handle edge cases and feature variability.
- **Impact**: Scalable, interpretable models for timely interventions and better healthcare outcomes.

For more information, see the [Project Report](Project_Report_Hanzhen_Zhu.pdf).
