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


# esp32 flow chart:
![image](https://user-images.githubusercontent.com/95648490/177235272-90770f8b-d83d-4d6f-8bf9-3284241d8bb6.png)
