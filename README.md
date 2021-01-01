# Rattancam
Here are notes to the rattancam 2021. 
Used hardware: ESP32-CAM, Arduino UNO, wires
I folled the tutorial of TechStudyCell on 01.01.2021: https://www.youtube.com/watch?v=q-KIpFIbRMk

1. I modyfied the instruction on following steps:  choose at Tools: Board: AI Thinker ESP32-CAM
2. Change the code accordingly to the model of your camera (mine only indicates 8225N V2.0 171026)  
 
// Select camera model
//#define CAMERA_MODEL_WROVER_KIT
//#define CAMERA_MODEL_ESP_EYE
//#define CAMERA_MODEL_M5STACK_PSRAM
//#define CAMERA_MODEL_M5STACK_WIDE
  #define CAMERA_MODEL_AI_THINKER

  #if defined(CAMERA_MODEL_AI_THINKER)
  pinMode(13, INPUT_PULLUP);
  pinMode(14, INPUT_PULLUP);

3. Assign to your own WIFI  

