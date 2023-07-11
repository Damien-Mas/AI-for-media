# AI-for-media

In this zip file, you will find a folder containing a folder named “
mini_project_hand_gestures”, and another one named “videos”. The “mini_project_hand_gestures”
folder contains the actual mini project, it is a modified project which was introduced to us during
week 3.2 of the AI for Media class, the original project may be found at the following URL:
https://github.com/kinivi/hand-gesture-recognition-mediapipe.

The original project was concerned with hand gesture recognitions and to assign labels to the
gesture which was detected by the program. My idea was to modify this program in order to play
sounds when a gesture would be detected. A couple of cases where such hand gesture recognition
tools when used in conjunctions with sounds may be to understand sign language and transform it
into spoken English, making communication simpler for deaf or hard of hearing persons, or in
music production where hand gesture recognition software may be used to control sound effects and
modify sound samples, allowing musicians to produce distinctive and expressive performances.

The exact files which I have modified are named “app.py” for folders “hand-gesture-recognition-
mediapipe-main_modified_v0”, “hand-gesture-recognition-mediapipe-main_modified_v1” and
“hand-gesture-recognition-mediapipe-main_modified_v2”. This file may be found at the root of
each folder.

I have also modified the files “keypoint_classifier_label.csv” and “keypoint.csv” for folder “hand-
gesture-recognition-mediapipe-main_modified_v1” and “hand-gesture-recognition-mediapipe-
main_modified_v2”. These files may be found under the “/hand-gesture-recognition-mediapipe-
main_modified_v1/model/keypoint_classifier” folder.

In the version 0 of the submitted project, modifications were made by importing the
"audiosegment" and "play" modules from the pydub library, followed by the creation of a custom
function "play_sound" to facilitate the playback of WAV files using the aforementioned modules.
Subsequently, the objective was to locate the exact location in the original program responsible for
detecting hand gestures. This was achieved by removing the lines of code responsible for
associating hand gestures with labels, and replacing it with a detection mechanism designed to play
a sound instead. It is important to note that at this stage, gesture detection in association with sound
was hard-coded into the program, indicating that the classifier was not retrained.

Upon successful completion of the initial, "buggy" program, work was initiated on version 1 of the
project. The "threading" library was imported, and another custom function "play_sound_threaded"
