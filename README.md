# Diabetic Retinopathy Lesion Segmentation Using the IDRiD Dataset

This project implements a deep learning-based segmentation model to identify diabetic retinopathy (DR) lesions from retinal fundus images using the U-Net architecture. The model is designed to segment five key components associated with DR:
- Microaneurysms (MA)
- Haemorrhages (HE)
- Hard Exudates (EX)
- Soft Exudates (SE)
- Optic Disc (OD)

## ⚙️ Technical Approach

A U-Net-based convolutional neural network is used for pixel-wise segmentation of lesions from fundus images. The training is conducted on the IDRiD dataset, which offers high-resolution images with precise pixel-level annotations.

**Note:** This project is still a work in progress. The repository will be updated continuously.

## 📁 Dataset Info

- **Dataset Name:** Indian Diabetic Retinopathy Image Dataset (IDRiD)
- **Access Link:** [IEEE Dataport – IDRiD Dataset](https://ieee-dataport.org/open-access/indian-diabetic-retinopathy-image-dataset-idrid)
- **Challenge:** Diabetic Retinopathy Segmentation and Grading Challenge – ISBI 2018

> IDRiD is the first diabetic retinopathy dataset representative of the Indian population. It contains pixel-level annotations for both pathological lesions and normal anatomical structures, making it ideal for developing AI-based diagnostic tools.

---

Feel free to explore, fork, or contribute to this repository to improve the model, experiment with training techniques, or evaluate new strategies for lesion detection.
