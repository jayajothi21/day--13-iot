# day--13-iot
First TFLite Micro Inference – Deploy a small .tflite model on ESP32 using TensorFlow Lite Micro and predict a class from a sample input.




# SIG-03 AUTOMATRIX – First TFLite Micro Inference

## Objective

Deploy a small TensorFlow Lite (`.tflite`) model on an ESP32 using TensorFlow Lite Micro and predict a class from a sample input.

## Classes

The model classifies the input into three categories:

* LOW
* MEDIUM
* HIGH

## Workflow

```text
Training Data
      ↓
TensorFlow Model
      ↓
TFLite Conversion
      ↓
model.tflite
      ↓
ESP32 + TensorFlow Lite Micro
      ↓
Sample Input
      ↓
Class Prediction
```

## Sample Input

```text
0.85
```

## Expected Output

```text
Sample Input: 0.85
Predicted Class: HIGH
Confidence: ...
```

## Files

* `SIG-03-AUTOMATRIX-TFLite-Micro.ipynb` – Google Colab notebook containing the model training and TFLite conversion code.
* `model.tflite` – Converted TensorFlow Lite model.
* `model_data.h` – TFLite model converted into a C/C++ header format for ESP32.
* `README.md` – Project documentation.

## Tools Used

* Google Colab
* Python
* TensorFlow
* TensorFlow Lite
* ESP32
* TensorFlow Lite Micro

## Result

The trained TensorFlow model was successfully converted into a `.tflite` model. The model can be deployed on ESP32 using TensorFlow Lite Micro to classify a sample input into LOW, MEDIUM, or HIGH.

