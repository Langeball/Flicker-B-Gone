# Flicker-B-Gone
WIP software to remove flicker from buggy screencaps, like Shadowplay

# Instructions:
// Current version is a simple python script, which requires you to have python installed.

// Besides that, all you have to do is prove the script with the file location of the video you want to fix.
If you don't have an IDE, you can simply edit the code using a text editor.

// If you get an error about missing codec, look at this:
https://coding.horje.com/example/137550-failed-to-load-openh264-library:-openh264-1.8.0-win64.dll-code-example

// If your input video is using a different codec, you can manually change the "fourcc" variable to: fourcc = cv2.VideoWriter_fourcc(*'X264')
And then follow the steps in the link above.
  
If you have any questions, feel free to ask. I'm using this as an exercise and will be making the script much more user friendly over time.
