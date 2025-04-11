# frequencyandemotion
Play around with frequency audio and emotional states

FEATURES
1. Feel the frequency
A random frequency gets played and the user can input what they are feeling. 
The reward is a comparison of user feelings and collective feelings for that frequency
 
2. Generate frequency for current mood
The user inputs how they feel
The reward is a sound that in aligned with their current mood
 
3. Generate emotion
The users inputs how they want to feel 
The reward is a sound that is most likely to make them feel that way

4. Frequency/emotion graph
The feelings are graphed against the frequencies
 

ARCHITECTURE X.0

1. Frontend (User Interface)
Tool: Tkinter (Pythons built-in GUI library)
Purpose: Displays buttons, input fields, and graphs; plays sounds.

Components:
Main Window: Buttons for each feature (e.g., “Play Random Frequency,” “Input Mood”).
Input Fields: Text boxes for users to enter feelings or desired emotions.
Output Area: Shows comparisons (e.g., “You felt calm, 60% of users felt the same”).
Graph Canvas: Displays frequency vs. emotion data

2. Backend (Logic and Data)
Language: Python—handles logic, file I/O, and basic data processing.

Components:
Frequency Generator: Uses PyDub or NumPy + PyGame to create and play frequencies.
Data Storage: A simple CSV file or SQLite database to store user inputs and collective feelings (e.g., frequency, user_feeling, timestamp).
Emotion Mapping: A dictionary or basic ML model (later) to link frequencies to emotions (e.g., 432 Hz → “calm”).
Comparison Logic: Calculates stats (e.g., % of users feeling X at Y Hz).

3. Audio Handling
Tool: PyGame (for playback) + NumPy (to generate sine waves for frequencies).
Purpose: Plays random or mood-based frequencies through your Mac speakers.

4. Data Visualization
Tool: Matplotlib—Pythons plotting library, integrates with Tkinter.
Purpose: Graphs frequencies (x-axis) vs. emotions (y-axis, encoded as numbers or categories).


ARCHITECTURE 1.0

1. Feel the frequency: a random youtube link is shared with the user, and the user can input feelings seperated by commas, the app then shows what words overlap with previously known words and which did not
2. Generate frequency: the user inputs how they feel, the app then give a youtube link that is the best match with that input. 
3. Generate emotion: the user inputs how they want to feel, the app then gives a youtube link that is the best match with that input (same as 2)
4. Frequency/emotion graph: the user input the hertz frequency, the app then gives the most likely emotions that are associated with that frequency
? the matching of frequencies and emotions probably needs to some type of match scoring system


