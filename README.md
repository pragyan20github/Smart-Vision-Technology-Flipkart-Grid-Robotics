# Smart-Vision-Technology-Flipkart-Grid-Robotics
## Use Cases Addressed:
Image Recognition and Classification |
Image Preprocessing, Text Extraction, and Feature Extraction |
Counting Number of Objects Present in the Image |
Predicting Shelf Life of Vegetables and Fruits

## Resources Used:
Image Recognition and Classification: InceptionV3  
Text Extraction and Feature Analysis: PaddleOCR, spaCy, Regex  
Counting Model: CountGD  
Freshness Prediction: MobileNetV2 with TensorFlow/Keras

## Final Workflow
1. Input Image
2. The process begins by taking an image as input.
3. Image Classification:
  The image is classified into one of the following categories:
    Fruits and Vegetables |
    Clothing |
    Footwear |
    Snacks |
    Miscellaneous Household Items
5. Text Extraction (if applicable):
  If the image contains text, it is processed by:
  OCR (Optical Character Recognition): Reads the text from the image.
  spaCy and Regex: Interprets the extracted text to provide details like:
    Brand |
    Pack Size |
    Manufacturing Date |
    Expiry Date |
    MRP (Maximum Retail Price)
5. Counting Process:
  The image is sent to CountGD for counting the number of products in the image.
7. Freshness Prediction (for Vegetables):
  If the image is identified as a vegetable:
    It undergoes counting procedures.
    It is also processed by the best_fruit_freshness_model.keras to predict
    freshness and shelf life.
