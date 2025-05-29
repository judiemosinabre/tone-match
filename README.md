# ToneMatch: Identifying Lip Product Undertones for Personalized Beauty

**ToneMatch** helps users find lip products that match their skin undertone, enhancing natural beauty and avoiding mismatched shades.  
It uses **YOLOv11** to classify lipsticks and glosses into four undertone categories:

- Warm  
- Cool  
- Neutral to Warm  
- Neutral to Cool

Trained on a custom dataset of 200+ images under various lighting conditions, the model detects undertones based on visual cues.  
By automating this classification, ToneMatch simplifies product selection for beauty shoppers and professionals, promoting confident, personalized choices in cosmetics.

## 🗂 Dataset & Model

Due to file size and privacy constraints, the custom dataset and trained model used in this project are **not included** in this repository.

If you'd like to test or extend ToneMatch:

- Use your **own custom image dataset** of lip products.
- Annotate the dataset using **Label Studio** (recommended) for bounding boxes and labels.
- Replace the dataset path in the notebook with your own.
- Train a YOLOv11 model using the provided training code.
- Update the model path accordingly.

📬 *Feel free to open an issue if you'd like help reproducing the setup.*

---

### 📸 Sample Output

---

## 🛠 Tools & Technologies

- Python  
- Google Colab (for training and experimentation)  
- [Ultralytics YOLOv11](https://github.com/ultralytics/ultralytics)  
- [Label Studio](https://labelstud.io/) (for image annotation)  
- Custom dataset of lip products 
- NVIDIA GPU with CUDA 12.4 support *(for local training)*


To install PyTorch with CUDA 12.4 support:
```bash
pip install --upgrade torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124