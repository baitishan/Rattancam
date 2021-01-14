# Rattancam
Here are notes to the rattancam 2021. 
Used hardware: ESP32-CAM, Arduino UNO, wires
I folled the tutorial of TechStudyCell on 01.01.2021: 
https://www.youtube.com/watch?v=q-KIpFIbRMk
A further helpful tutorial is from robotzer.one:
 https://www.youtube.com/watch?app=desktop&v=U5uvl6kDFJY&list=PLbDvGAjwWTEymhiLuoQwheQZLmE78iM8b&index=1
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

# LED rings

on pin 3 and pin 6 of the UNO I attached rings with 60 and 12 LED's. 
I included the Adafruit_NeoPixel.h library and opened the NeoPixel example. I copied the void setup() and renamed the strip in strip1 and strip2. 
In the loop I copied and renamed the display procedure. Some of the  commands I allocated to strip1, some to strip2. 
