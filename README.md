# Flicker-B-Gone
WIP software to remove flicker from buggy screencaps, like Shadowplay.
The way it works is by copying and pasting frames from an input, to an output. But whenever the script detects a flicker, it instead copy/pastes the last viable frame (frame that isn't a flicker). It does this by simply reading colour information of a few pixels. If they are all the exact same colour, it's most likely a flicker.

"Before and after" video example to showcase effectiveness:

https://www.youtube.com/watch?v=wcOYoetzUnw

# Instructions:
// Current version is a simple python script, which requires you to have python installed.

// Besides that, all you have to do is prove the script with the file location of the video you want to fix.
If you don't have an IDE, you can simply edit the code using a text editor.

// If you get an error about missing codec, look at this:
https://coding.horje.com/example/137550-failed-to-load-openh264-library:-openh264-1.8.0-win64.dll-code-example

// If your input video is using a different codec, you can manually change the "fourcc" variable to: fourcc = cv2.VideoWriter_fourcc(*'X264')
And then follow the steps in the link above.

// The output video will not have any audio, so you will have to splice it back in with your original footage. There shouldn't be any desync, since no frames are actually removed, only duplicated
  
If you have any questions, feel free to ask. I'm using this as an exercise and will be making the script much more user friendly over time.
