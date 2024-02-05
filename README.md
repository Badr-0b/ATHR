# ATHR
ATHR (Alt + Tab Hand Recognition)

this code utilizes the mediapipe, keyboard and cv2 libraries to recognize the human hand and stumilate the required keys

upon the recognition of a human hand appearing on screen, the left alt + tab key combo is stimulated simultaneously ONCE
thus as a result switching from whatever program i have active currently on screen and opening a different tab altogether

useful for when pretending to study but parents walk in and you cant read the alt tab key's on time.

anyways, heres the flowchart i made using plantUML for this code.

![alttabonce](https://github.com/Badr-0b/ATHR/assets/66253861/98acfc79-ca17-4e72-83bf-de74e50bdb81)

so basically a quick run down of whats going on:
uses mediapipe to access the webcam and create a window to show what the computer sees
now reads the frames from webcam, if read properly it draws a green box (THIS DOESNT SHOW ON THE SCREEN BECAUSE I DIDNT LABEL THE THICKNESS OF THE GREEN BOX, also too lazy to do it anyways now)
if hand marks have been detected on the screen then stimulate alt tab key combo and changes the boolean value for key_pressed function to true and does alt tab

also, for quick exit of the program, just press the esc key, doing so makes the program stop its access to webcam and shuts the window down and the program essentially kills itself

there was this older version i made that did the same thing except it would rapidly stimulate the tab switch keys with no end so it would basically make the tabs flicker in and out, im sure i could put it to some use in some other form, perhaps as a visually guided autoclicker, but for now im just glad i finished this project

enjoy 👍
