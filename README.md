# German Traffic Sign Recognition

A deep learning project for classifying German traffic signs using CNN in Google Colab.

## 🚦 Overview

This Colab notebook implements a CNN model to recognize and classify 43 different types of German traffic signs from the GTSRB dataset using TensorFlow/Keras.

## 📓 Notebook

Open the notebook in Google Colab and run all cells sequentially:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Enesbicer/german-traffic-sign-recognition/blob/main/traffic_sign_recognition.ipynb)

## 🎯 What This Notebook Does

1. **Downloads GTSRB dataset** from Kaggle automatically
2. **Loads and preprocesses** 43 classes of traffic signs
3. **Builds and trains** a CNN model with:
   - 3 Convolutional blocks
   - Batch normalization
   - Dropout regularization
   - Early stopping
4. **Visualizes results** with accuracy/loss graphs
5. **Provides inference function** for new predictions

## 🚀 How to Run

1. **Open in Colab**: Click the badge above or upload the `.ipynb` file
2. **Set Runtime**: Go to Runtime → Change runtime type → GPU
3. **Upload Kaggle Key**: When prompted, upload your `kaggle.json` file
4. **Run All Cells**: Runtime → Run all (or Ctrl+F9)

## 📊 Results

- **43 Traffic Sign Classes** including speed limits, warnings, and regulatory signs
- **Training Visualizations** showing accuracy and loss curves
- **Test Accuracy** displayed after training
- **Inference Function** ready to use: `predict_traffic_sign()`

## 🔧 Key Features

- ✅ **Fully automated** - just run the cells
- ✅ **GPU optimized** for faster training
- ✅ **Complete pipeline** from data download to inference
- ✅ **Visualization tools** for data exploration and results
- ✅ **Model saving** - downloads trained model
- ✅ **Ready-to-use inference** function

## 💡 Usage After Training

```python
# The notebook provides this function:
predicted_class, class_name, confidence = predict_traffic_sign('path/to/image.jpg', model)
print(f"Predicted: {class_name}")
print(f"Confidence: {confidence:.2f}")
```

## 📋 Requirements

- Google Colab account
- Kaggle account and API key (`kaggle.json`)
- GPU runtime (recommended)

## 📁 Files Generated

- `traffic_signs_model.h5` - Trained model (auto-downloaded)
- Training history plots
- Performance metrics

## 🎮 Traffic Sign Classes

The model recognizes 43 German traffic signs:
- Speed limits (20-120 km/h)
- Warning signs (curves, pedestrians, etc.)
- Regulatory signs (stop, yield, no entry)
- Informational signs (directions, conditions)

## 🤝 Contributing

Fork this repository and improve the notebook! Pull requests welcome.

## 📄 License

MIT License - feel free to use and modify!
