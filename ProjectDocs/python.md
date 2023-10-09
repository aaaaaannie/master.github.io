* Random Forests
    - Evaluate the Default Threshold
    ```python
    from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
    y_pred = rf.predict(X_test)
    print("Accuracy:", accuracy_score(y_test, y_pred))
    print("Precision:", precision_score(y_test, y_pred))
    print("Recall:", recall_score(y_test, y_pred))
    print("F1 Score:", f1_score(y_test, y_pred))
    ```
    - Find the Optimal Threshold
    ```python
    import numpy as np
    from sklearn.metrics import f1_score

    y_probs = rf.predict_proba(X_test)[:, 1]

    thresholds = np.arange(0, 1.05, 0.05)
    best_threshold = 0.5
    best_f1 = 0

    for threshold in thresholds:
        y_pred = (y_probs >= threshold).astype(int)
        f1 = f1_score(y_test, y_pred)
        if f1 > best_f1:
            best_f1 = f1
            best_threshold = threshold

    print("Best Threshold:", best_threshold)
    ```
    
