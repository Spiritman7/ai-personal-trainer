# AI Personal Trainer 



## Preface :key: :memo:

Welcome to my [AI Personal Trainer v1 !](https://ai-personal-trainer.herokuapp.com/)

This is a computer vision project which focuses on monitoring human body movement during specific workouts in order to differentiate between good/bad reps.

Reps performed with good workout form are flagged as good reps (i.e. incrementally added to "total reps count") and reps with bad workout form are currently ignored (i.e. not added to "total reps count"). 





## Approaches :heavy_plus_sign: :heavy_minus_sign: :heavy_multiplication_x: :heavy_division_sign:

* Pose estimation - an AI method for identifying human orientation by detecting their primary skeletal joints. 
* Trigonometry - used for calculating angles from 3 body joints   




## Technologies :alien:




- [**mediapipe**](https://github.com/google/mediapipe) - for accessing Google's pose estimation algorithm 
- [**open-cv**](https://github.com/opencv/opencv) - for computer vision resources 
- [**numpy**](https://github.com/numpy/numpy) - for mathematical computation  
- [**time**](https://github.com/PaulStoffregen/Time) -  for calculating metrics associated with time (seconds, mins, hrs)
- [**json**](https://github.com/nlohmann/json) -  for deserializing JSON formatted data
- [**requests**](https://github.com/psf/requests) - for processing HTTP requests 
- [**streamlit**](https://github.com/streamlit/streamlit) - for quick web app prototyping 
- [**streamlit_lottie**](https://github.com/andfanilo/streamlit-lottie) - for embedding Lottie animations into Streamlit  



## Tools   :hammer_and_wrench:

To be able to use the AI personal trainer, you need (a):

- camera/laptop webcam (for live streaming)
 

## Exercises :muscle:

Here are the workouts included in v1 release:


### 1. Bicep curls 

#### Workout Tips 

            - Curl dumbbell towards the region between your chest and bicep
            - Curl back down to starting position and repeat motion 
            - Keep shoulder and elbow locked to your side through out the exercise
            - Squeeze biceps tight through out the exercise

#### Landmarks

1. **Right side**

- Shoulder: 12
- Elbow: 14
- Wrist: 16

2. **Left side**

- Shoulder: 11
- Elbow: 13
- Wrist: 15


#### Angles

- **Starting pose:** If angles formed by selected landmarks is **greater than** 160 degrees
- **Ending pose:** If angles formed by selected landmarks is **less than** 30 degrees



### 2. Push-ups 

#### Workout Tips 

            - Keep a straight spine from start to finish
            - Slowly dip your body towards the ground then push the ground away from you
            - Clench your core as tight as if you're about to get punched in the stomach through out the workout


#### Landmarks

1. **Right side**

- Shoulder: 12
- Elbow: 14
- Wrist: 16

2. **Left side**

- Shoulder: 11
- Elbow: 13
- Wrist: 15



#### Angles

- **Starting pose:** If angles formed by selected landmarks is **greater than** 170 degrees
- **Ending pose:** If angles formed by selected landmarks is **less than** 45 degrees




### 3. Squats 

#### Workout Tips 


            - Keep your feet shoulder-width apart
            - Keep your back straight through out exercise
            - Focus on dipping until your hip joint is lower than your knee joint
            - Drive back up with your chest


#### Landmarks

1. **Right side**

- Hip: 24
- Knee: 26
- Ankle: 28


2. **Left side**

- Hip: 23
- Knee: 25 
- Ankle: 27



#### Angles

- **Starting pose:** If angles formed by selected landmarks is **greater than** 170 degrees
- **Ending pose:** If angles formed by selected landmarks is **less than** 60 degrees





### 4. High knees

#### Workout Tips 

            - Align your feet the same distance apart as your hips
            - Maintain a straight back through out workout
            - Raise each knee above your hip joint 
            - Pump your arms with each knee raise to get the heart rate high  

#### Landmarks

1. **Right side**

- Shoulder: 12
- Hip: 24
- Knee: 26


2. **Left side**

- Shoulder: 11
- Hip: 23
- Knee: 25


#### Angles

- **Starting pose:** If angles formed by selected landmarks is **greater than** 120 degrees
- **Ending pose:** If angles formed by selected landmarks is **less than** 70 degrees


## Development Goals

Future release(s) will focus on: 

* More advanced AI algorithms/techniques e.g. MoveNet, YOLOv5, MobileNet
* Sharpening pose estimation accuracy of current model
* Enhancing user interface features (e.g. converting app into a more robust SPA)


## Conclusion  :closed_lock_with_key:

The 2nd release will address the "open-cv" bug that currently prevents webcam activating on certain machines after selecting a workout and clicking on "Start Workout" checkbox.

Feel free to reach out to me via [LinkedIn](https://www.linkedin.com/in/stephen-david-williams-860428123/) or [email](mailto:stephenodavidwilliams@gmail.com) if you have any thoughts or suggestions regarding the app and I will get to them as soon as possible :muscle: :space_invader: