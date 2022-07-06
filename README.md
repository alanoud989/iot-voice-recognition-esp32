# iot-voice-recognition-esp32
A web page for voice recognition and converting it into text in Arabic , Algorithm steps to run the esp32

# voice-recognition using html:
    <!DOCTYPE html>
    <htmllang="ar">
    <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Voice Recognition</title>

# voice-recognition using css:
    <style>
    h1 {
    color: white;
    text-align: center;
    }
    input[type=text]{
    width:80%;
    padding: 50px 50px;
    box-sizing: border-box;
    border: none;
    background-color: white;
    margin-right: 80px;
    margin-left: 80px;
    color: #008CBA;
    text-align: right;
    font-size: 20px;
    }
    button {
    position: absolute;
    top: 260px;
    right: 720px;
    width: 100px;
    height: 50px;
    background-color: #008CBA;
    border: none;
    color: white;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
  
     }
     body {
     background-color: lightblue;
     }

    </head>
    </style>


# voice-recognition using Javascript:
      <script>
        function record() {
            var recognition = new webkitSpeechRecognition();
            recognition.lang = "ar-SA";

            recognition.onresult = function(event) {
                // console.log(event);
                document.getElementById('speechToText').value = event.results[0][0].transcript;
            }
            recognition.start();

        }
    </script>
    <!-- end of script -->


# algorithm steps to the run wasdom esp32 piece.

1. Download Arduino IDE
2. Run Arduino IDE
3. Then we take important steps to run eps32 click on a file and then choose preferences
4. A box opens in which we put the package link to the esp32 piece, which is
http://dL.espressif.com/dL/package_esp32_index.json
Then press OK
5. Click on the tools, then choose the Arduino panel, then the panel manager.
6. A type screen appears in the ESP32 dialog box and then press the installation process.
7. Click on the tools, then choose the Arduino panel, then see the piece added named ESP32 Arduino.
8. We connect the piece to the USB cord to the computer, so the esp32 piece shows us two lights, which are fixed red and blue.
9. Click on the tools, then choose the Arduino panel, then see the piece added named ESP32 Arduino, then choose the WEMOS D1 MINI ESP32 controller.
10. Click on Tools, then choose "port" COM3, then press it, choose the right sign at COM3.
11. We want to turn on the ESP32 lighting.
12. In order to turn on the lighting, we go to click on a file, then choose examples, then choose basic, then choose blink.
13. Then a page press an arrow tick appears in the address bar on the left side of the upload process.
14. The blue light begins to point quickly or at medium speed.

![image](https://user-images.githubusercontent.com/95648490/177235272-90770f8b-d83d-4d6f-8bf9-3284241d8bb6.png)

# esp32 flow chart:
![image](https://user-images.githubusercontent.com/95648490/177235272-90770f8b-d83d-4d6f-8bf9-3284241d8bb6.png)
