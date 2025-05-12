Number Plate Detection using OpenCV and EasyOCR
This project detects vehicle number plates from images using Haar Cascades and extracts text from the plates using OCR with EasyOCR.

Features
Detects number plates in images using Haar Cascade classifiers.

Extracts and reads text from detected plates using EasyOCR.

Visualizes detected plates and OCR results on the image.

Designed for Google Colab or Jupyter Notebook environments.

Dependencies
pip install opencv-python easyocr
How to Use
Prepare the Image:

Place the input image (e.g., np1.webp) in your working directory.

Run the Script:

Load the image and the Haar cascade file.

The model will detect number plates and perform OCR to extract text.

Output:

The image will be displayed with bounding boxes and recognized text over the plates.

Detected text will also be printed to the console.

Example
image_path = 'np1.webp'
plate_cascade = cv2.CascadeClassifier('haarcascade_russian_plate_number.xml')
Detected text might look like:
Detected Plate Text: TN09CA1234
Notes
This implementation is optimized for use in Google Colab using cv2_imshow for displaying images.

For local use, replace cv2_imshow with cv2.imshow and add cv2.waitKey(0) and cv2.destroyAllWindows() as needed.

Author
Created by: Bala Preethi M
Contact: balapreethi1615@gmail.com
GitHub:https://github.com/preethi-1615
