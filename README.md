# Smart-Vision-Technology-Flipkart-Grid-Robotics

## Project Description:
This project focuses on leveraging machine learning and computer vision techniques to enhance the quality control and inventory management processes for e-commerce platforms, specifically targeting Flipkart, one of the largest e-commerce platforms in India. With the rapid growth of online retail, ensuring accurate product quality assessments, efficient inventory management, and minimizing waste in the shipment of perishable goods has become a critical challenge.

Our solution addresses these issues through a combination of **image recognition**, **object counting**, **text extraction**, and **freshness prediction models**, designed to streamline the quality assurance workflow for Flipkart and similar platforms.

## Use Cases Addressed:
- Image Recognition and Classification  
- Image Preprocessing, Text Extraction, and Feature Extraction  
- Counting Number of Objects Present in the Image  
- Predicting Shelf Life of Vegetables and Fruits  

## Resources Used:
- **Image Recognition and Classification:** InceptionV3  
- **Text Extraction and Feature Analysis:** PaddleOCR, spaCy, Regex  
- **Counting Model:** CountGD  
- **Freshness Prediction:** MobileNetV2 with TensorFlow/Keras  

## Project Objectives:
- **Image Recognition and Classification:**  
   Develop a system that classifies images of products into predefined categories (e.g., fruits, clothing, footwear, snacks, household items). This enables automated sorting and processing of products.

- **Image Preprocessing and OCR (Optical Character Recognition):**  
   Enhance the quality of images through preprocessing techniques, followed by the use of OCR to extract essential information such as brand, expiry date, and MRP, which supports better inventory tracking and product verification.

- **Product Counting:**  
   Implement counting algorithms that accurately detect and count items in images, ensuring proper inventory management and reducing human error in stock counting.

- **Freshness Prediction of Perishables:**  
   Develop a model capable of predicting the freshness and remaining shelf life of fruits and vegetables, helping reduce waste by providing accurate assessments of perishable goods.

## Final Workflow:
1. **Input Image:**  
   The process begins by taking an image as input.

2. **Image Classification:**  
   The image is classified into one of the following categories:
   - Fruits and Vegetables  
   - Clothing  
   - Footwear  
   - Snacks  
   - Miscellaneous Household Items  

3. **Text Extraction (if applicable):**  
   If the image contains text, it is processed by:  
   - **OCR (Optical Character Recognition):** Reads the text from the image.  
   - **spaCy and Regex:** Interprets the extracted text to provide details like:
     - Brand  
     - Pack Size  
     - Manufacturing Date  
     - Expiry Date  
     - MRP (Maximum Retail Price)  

4. **Counting Process:**  
   The image is sent to **CountGD** for counting the number of products in the image.

5. **Freshness Prediction (for Vegetables):**  
   If the image is identified as a vegetable, it undergoes counting procedures and is processed by the **best_fruit_freshness_model.keras** to predict freshness and shelf life.

## Conclusion:
This project integrates advanced computer vision techniques and machine learning models to automate key aspects of the e-commerce quality control process. By leveraging state-of-the-art solutions for **image recognition**, **object counting**, **text extraction**, and **freshness prediction**, our approach not only improves operational efficiency but also helps reduce waste and ensure better product quality for end consumers.
