#first task:
# convert-speech-to-text
in this task , i designed the user interface for speesh to text application using programing language html and css and i used bootstrap site to ease the designing prosses how to make it support arabic language when i speak with.
# use html language
1-  first of all , i created file namd index.html

2- to make it support arabic langauge i added the command <html lang= "ar"
and for direction dir= "rtl" 

3- i created the title of the page  , textarea to see what i said  ,and button that when user click on the start button the recognition API is begun and will listen for input from the user

4- when you press the button , your browser will request the permission to use your microphone.

# using java script and css 
1- We have SpeechRecognition for understanding human voice and turning it into text 

2-  set up a couple of event handlers. Most of them simply listen for changes in the recognition status.when the user speak or stop of talking
recognition.onstart = function() {

 instructions.text("Voice Recognition is On")

}

recognition.onspeechend = function() {

 instructions.text("No Activity")
 
 3-a special onresult event that is very crucial. It is executed every time the user speaks a word or several words in quick succession, giving us access to a text transcription of what was said.

capture something with the onresult handler save it in a global variable and display it in a textarea

4-$('#start-record-btn').on('click', function(e) {
  recognition.start();
});
This will prompt users to give permission. If such is granted the device's microphone will be activated , and receive the words from user.


