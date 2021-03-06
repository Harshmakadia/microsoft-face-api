# Microsoft Face API

- Detect human faces and compare similar ones
- Organise images into groups based on similarity
- Identify previously tagged people in images

> Detect one or more human faces in an image and get back face rectangles for where in the image the faces are, along with face attributes which contain machine learning-based predictions of facial features. The face attribute features available are: Age, Emotion, Gender, Pose, Smile and Facial Hair along with 27 landmarks for each face in the image.


## Sample Face Detection API Response 

```
 [
  {
    "faceId": "7c29f0ca-629a-4026-86d6-2d9faee9bbd7",
    "faceRectangle": {
      "top": 128,
      "left": 459,
      "width": 224,
      "height": 224
    },
    "faceAttributes": {
      "hair": {
        "bald": 0.0,
        "invisible": false,
        "hairColor": [
          {
            "color": "brown",
            "confidence": 1.0
          },
          {
            "color": "blond",
            "confidence": 0.69
          },
          {
            "color": "black",
            "confidence": 0.54
          },
          {
            "color": "other",
            "confidence": 0.31
          },
          {
            "color": "gray",
            "confidence": 0.05
          },
          {
            "color": "red",
            "confidence": 0.04
          }
        ]
      },
      "smile": 0.939,
      "headPose": {
        "pitch": 0.0,
        "roll": -16.9,
        "yaw": 16.7
      },
      "gender": "female",
      "age": 23.4,
      "facialHair": {
        "moustache": 0.0,
        "beard": 0.0,
        "sideburns": 0.0
      },
      "glasses": "ReadingGlasses",
      "makeup": {
        "eyeMakeup": true,
        "lipMakeup": true
      },
      "emotion": {
        "anger": 0.037,
        "contempt": 0.001,
        "disgust": 0.015,
        "fear": 0.001,
        "happiness": 0.939,
        "neutral": 0.001,
        "sadness": 0.0,
        "surprise": 0.007
      },
      "occlusion": {
        "foreheadOccluded": false,
        "eyeOccluded": false,
        "mouthOccluded": false
      },
      "accessories": [
        {
          "type": "glasses",
          "confidence": 0.99
        }
      ],
      "blur": {
        "blurLevel": "low",
        "value": 0.0
      },
      "exposure": {
        "exposureLevel": "goodExposure",
        "value": 0.48
      },
      "noise": {
        "noiseLevel": "low",
        "value": 0.0
      }
    },
    "faceLandmarks": {
      "pupilLeft": {
        "x": 504.8,
        "y": 206.8
      },
      "pupilRight": {
        "x": 602.5,
        "y": 178.4
      },
      "noseTip": {
        "x": 593.5,
        "y": 247.3
      },
      "mouthLeft": {
        "x": 529.8,
        "y": 300.5
      },
      "mouthRight": {
        "x": 626.0,
        "y": 277.3
      },
      "eyebrowLeftOuter": {
        "x": 461.0,
        "y": 186.8
      },
      "eyebrowLeftInner": {
        "x": 541.9,
        "y": 178.9
      },
      "eyeLeftOuter": {
        "x": 490.9,
        "y": 209.0
      },
      "eyeLeftTop": {
        "x": 509.1,
        "y": 199.5
      },
      "eyeLeftBottom": {
        "x": 509.3,
        "y": 213.9
      },
      "eyeLeftInner": {
        "x": 529.0,
        "y": 205.0
      },
      "eyebrowRightInner": {
        "x": 579.2,
        "y": 169.2
      },
      "eyebrowRightOuter": {
        "x": 633.0,
        "y": 136.4
      },
      "eyeRightInner": {
        "x": 590.5,
        "y": 184.5
      },
      "eyeRightTop": {
        "x": 604.2,
        "y": 171.5
      },
      "eyeRightBottom": {
        "x": 608.4,
        "y": 184.0
      },
      "eyeRightOuter": {
        "x": 623.8,
        "y": 173.7
      },
      "noseRootLeft": {
        "x": 549.8,
        "y": 200.3
      },
      "noseRootRight": {
        "x": 580.7,
        "y": 192.3
      },
      "noseLeftAlarTop": {
        "x": 557.2,
        "y": 234.6
      },
      "noseRightAlarTop": {
        "x": 603.2,
        "y": 225.1
      },
      "noseLeftAlarOutTip": {
        "x": 545.4,
        "y": 255.5
      },
      "noseRightAlarOutTip": {
        "x": 615.9,
        "y": 239.5
      },
      "upperLipTop": {
        "x": 591.1,
        "y": 278.4
      },
      "upperLipBottom": {
        "x": 593.2,
        "y": 288.7
      },
      "underLipTop": {
        "x": 597.1,
        "y": 308.0
      },
      "underLipBottom": {
        "x": 600.3,
        "y": 324.8
      }
    }
  }
]
```

Please note I've not added the subscription key here.Though you can generate if from [here](https://docs.microsoft.com/en-us/azure/cognitive-services/computer-vision/vision-api-how-to-topics/howtosubscribe).
