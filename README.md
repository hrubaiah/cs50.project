TomoPomo
Video Demo:  <URL HERE>
Description: For my final project, I created a simple pomodoro timer using HTML, CSS, and JavaScript. The purpose of a pomodoro timer is to help increase your focus and productivity by completing tasks in small intervals. I chose this because I use pomodoro all the time, including with this course, and thought it’d be cool to create and utilize my own pomodoro timer. As I’m still a beginner, I hope to continue to work on this project and improve it as my skill set increases. 

I first created an HTML file called index.html. In this file, I created my HTML structure with title, header, and main div which includes the timer-circle, and the control buttons. There are four buttons: restart, which restarts the timer, choose time, which allows you to choose how long you want the timer to be, and resume/pause button, which allows you to pause the timer and resume it as well. I included a viewport meta tag which controls how the website is viewed on other devices, such as mobiles or tablets. I also linked my CSS file which controls the design of the website, and my JavaScript file which makes the website dynamic. 

Using CSS, I designed the website. I chose the colors using https://www.w3schools.com/cssref/css_colors.php. Using this website I found colors that compliment each other and included their HEX codes in the file. The colors I chose were inspired by one of my favorite characters, Xiao, in a game called Genshin Impact. His main colors are white and various shades of blue/green. I opted out of using white instead chose a cream like color since white seemed too plain. In the body tag, I aligned all the text in the center, choose the font family and font size of the text, and chose the background color #fefbd8. Display: flex made it easier to design without using position properties. For the remainder of the file, I styled main, the timer circle, the control buttons, and added hover which changed the color of the button when you hover over it. I chose the size and color of the border, the size of the text, and aligned all text to the center. 

I then created the JavaScript file which was the most important part. I first created my variables, timer, minutes, seconds, isPaused, and enteredTIme. I then created my first function, startTimer. This function basically starts the countdown and uses the setInterval method to call a function every 1000 milliseconds (1 second). 
I then created my updateTimer function. This updates the time displayed every second with formatTime. I then implement an if-else statement which basically says if the minutes display 0 and the seconds display 0, meaning time has run out, then it stops the timer and alerts the user saying “Time is up! Take a break :D”. Else, then continue to decrement. 

Then, I have my formatTime function which formats the timer as minutes, seconds: 15:00.
 
Following that function is my togglePauseresume function. The purpose of this function is to either pause the timer or resume the timer. The const pauseResumeButton will take in the querySelector, and inside of that is .control-buttons button. This will pause the timer and fill the isPaused variable from false to true. I then include an if-else statement which checks the condition that if paused then it pauses the timer and changes the button to resume, and if the button is clicked again and the timer will continue and the button will change to pause. 

The fifth function is restartTimer. This function is basically going to restart the timer. It’s going to clear the interval and reset the time. It’s going to stop the timer and reset to the original time that was entered or the default which is 15, and the timer will start again. 

The last function is the chooseTime function. When the button is selected, it will prompt you: ‘Enter new time in minutes: ‘. The number you insert must be greater than 0, If you enter 0, it will result in an error: ‘Invalid input. Please enter a valid number greater than 0’. You can input any time you want whether it be 1 minute, 5 minutes, 10 minutes, or even 100 minutes. 

That is all for my final project. Thank you so much edX and David Malan and the CS50 staff for teaching me and the rest of the CS50 community the building blocks we need to enter the real world. 
