# mu-new-project
Building an AI Project
# image to speech converter

@app. route ('/image speech')def img_speech ():
video = cv2.VideoCapture(0)
check, Image= video. Read () cv2.imshow("Colored", Image)key = cv2.waitKey(1) if key == Ord('s'):
cv2.imwrite("web.jpg", Image)img = Image. Open('web.jpg') result=pytesseract.image_to_string(img)
print(result)
my obj = gTTS (text=result, lang='en', slow=False)myobj.save("1.mp3")
mixer. init () mixer.music.load("1.mp3") mixer.music.set_volume (0.5)mixer.music.play () time.sleep(10) mixer.music.stop ()
break
key = cv2.waitKey(1)if key == Ord('q'):

video. Release ()
render template("home.html")if	name	== " main ":
app.run()

Above code for Describes that Image to speech conversion using Open cv2 Tool is used that Firstly define image to speech declaration then video capture its all by installing open cv2 toolit means show the image Infront of cv2 that captures and checks image in that it will checks colored image and it will convert to grey scale image text then after conversion to run the program it hold textual content image,we   have   added   button  key  as   ―s‖   for  captures   image   then   for   quit   the   image  we  had implemented the‖ key in keyboard then also that image will be stores in web.jpg format and the to extract text from image that we used Ocr tool that will extract text and detect text and for speech and for  quit purpose we added  ―Q‖ key in a keyboard.  Conversion we added the  GTTS tool in code that will converts the text to speech form and engine will wait and run for process and the speaker set to 0.5 range  value after speech conversion we added  ―q‖ key in the code that  will help  for quit  the  module then video will be release and stop the audio.
