# DeepLC
 
In order to use DeepLC to predict the retention time of non-canonical peptides, we first predicted the effect of the model for canonical peptides of the same project.

All canonical peptides are divided into ten parts, nine for model calibration and one for prediction. I used two calibration model methods. At the same time, the direct prediction method of uncalibrated model is also used. Here are the results of the predicted canonical peptide.

### pygam_calibration
command：deeplc --file_pred can1.csv --file_cal can9.csv --plot_predictions
![can1_deeplc_predictions](https://user-images.githubusercontent.com/83333440/218061182-2f28b887-e4cc-499e-b261-c118ad8b2902.png)
### legacy_calibration
command：deeplc --file_pred can1.csv --file_cal can9.csv --plot_predictions --legacy_calibration
![can1_deeplc_predictions](https://user-images.githubusercontent.com/83333440/218061300-4d052787-25e4-41d0-add2-fe4faf716cfa.png)
### no calibration
command: deeplc --file_pred can1.csv --plot_predictions
![image](https://user-images.githubusercontent.com/83333440/218063568-0b5c5838-3876-4e46-96f0-0f220c8c40f2.png)



