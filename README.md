# Listen-And-Repeat
Website built in javascript using the jsPsych library to present audio files one at a time.
A running example of the most recent version of this script can be found here: https://azrzkeyduw.cognition.run/?sequence=Demo 

This script requires:
jsPsych 6.1, which can be downloaded here: https://github.com/jspsych/jsPsych/releases/tag/v6.1.0

If you want to run this program locally you will need to run a local web server so the GET requests for the sequence and audio files are not blocked.  I use the Web Server For Chrome app for debugging purposes, but you may want to do some research and decide what program works best for you. When testing participants, we use a version of this program hosted on cognition.run

Once you have downloaded jsPsych 6.1, the ListenAndRepeat.html file, the five demo .wav files, and the Demo.txt experiment sequence, you can open the website in a web browser through your server and it should bring up task instructions.

The demo task we include plays five digit lists.  Two are in sequential order from 1 - 9, one is a short list of two digits, one is an intermediate list of five digits, and one is a long list of 9 digits.  These stimuli were previously used in Bosen and Barry, 2020 JSLHR. Any auditory stimuli can be used here, and we often use this interface to play word and sentence stimuli.

This script plays audio files one at a time. After each file is played the program waits for the participant to click 'Click to play the next word'. If you aren't playing words you may want to edit the experiment instructions (lines 55-59) and the button prompt (line 89) to better describe your stimuli. The order of audio files is defined in the Experiment Sequence file (Demo.txt is included here), with each line naming a single sound file to play on that trial. In our lab, we use this task in conjunction with a recorded video call so we can record verbal responses to each trial and score them offline.  Our lab also has specific procedures for recording and scoring data, which we will share on request (adam.bosen@boystown.org).
