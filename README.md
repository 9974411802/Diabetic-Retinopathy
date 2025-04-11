# Diabetic Retinopathy Lesion Segmentation Using the IDRiD Dataset

This project implements a deep learning-based segmentation model to identify diabetic retinopathy (DR) lesions from retinal fundus images using the U-Net architecture. The model targets five classes: microaneurysms (MA), haemorrhages (HE), hard exudates (EX), soft exudates (SE), and the optic disc (OD).

## ⚙️ Technical Approach

The dataset poses a significant **class imbalance problem**, as small lesions like microaneurysms occur far less frequently than the background or optic disc regions. To address this, the training uses a **combined weighted loss function** consisting of:
- **Weighted Dice Loss**
- **Focal Loss**

This combination helps the model focus on underrepresented classes and learn from hard-to-classify examples more effectively.

**Note:** No data augmentation techniques were used during training to highlight the core model performance.

## 📊 Results

After training for 120 epochs, the model achieved the following evaluation metrics:

- **Dice Coefficient:** `0.6059`
- **Intersection over Union (IoU):** `0.5326`
- **Pixel Accuracy:** `0.9973`

### Training Curves

![Training Metrics](/Training loss curve)

Plots above show the training progression for:
- Loss
- Dice Coefficient
- Intersection over Union (IoU)
- Pixel Accuracy

## 📁 Dataset Info

- **Name:** Indian Diabetic Retinopathy Image Dataset (IDRiD)
- **Challenge:** [IEEE Dataport DR Segmentation Challenge – ISBI 2018](https://ieee-dataport.org/open-access/indian-diabetic-retinopathy-image-dataset-idrid)

> The IDRiD dataset is the first Indian population-based DR dataset with pixel-level lesion annotations, making it ideal for developing clinical-grade DR screening tools.

---

Feel free to explore, fork, or contribute to this repository to enhance the model or explore new training strategies!
