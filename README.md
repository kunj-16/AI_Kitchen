# AI_Kitchen
#Customized AI Kitchen for India

PROBLEM STATEMENT: Customized AI Kitchen for India

DELIVERABLES:

Come up with an AI model with Training to cook users’ choice of dishes, including ingredient and quantity selection.
Programming option to detect right utensils and to raise request to get the utensils from Washing Machine automatically.
Indication of raw materials required, and notify if they are not present.
Give a Non Microwave Oven option, and come up with requirements to integrate that with the AI Kitchen model.
TECHNOLOGIES USED:

Machine Learning and AI 
TensorFlow 
pandas
Computer vision 
OpenCV
YOLOv3
Notification System
Twilio


Hardware Integration
Arduino Uno


Data Handling
CSV Files


AI Model for Cooking
-The AI model is developed using TensorFlow with LSTM layers to handle sequential data. 
-Pandas is used to preprocess the recipe data, separating features (X) and labels (y). 
-The trained model is saved as ai_kitchen_model.h5.

Utensil Detection and Management 
-YOLOv3 with OpenCV for real-time object detection to identify utensils in the kitchen.
-Configuration and weights (yolov3.cfg and yolov3.weights) are loaded using OpenCV's DNN module.
-A custom mapping (utensil_mapping) is used to map detection class IDs to human-readable utensil names.
-The detect_utensils function processes images to detect and list utensils present.

Raw Material Management 
-Pandas is used to read the inventory data from inventory.csv. 
-The check_ingredients function compares required ingredients for a recipe with available stock, identifying missing items.

Notification System 
-Twilio API is used to send SMS notifications.
-The send_notification function sends alerts about missing ingredients to the user's phone number. 
-Twilio account credentials (account_sid and auth_token) are required for API initialization.


Link of HARDWARE SIMULATION:
https://www.tinkercad.com/things/gek5J6TVgj2-aikitchen/editel


IMPORTANT: For the successful execution of the code you need one more file named"yolov3.weights" which I am not able to upload in the repository due to its size.

