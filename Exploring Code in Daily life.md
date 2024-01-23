
# - Code that specifies when an alarm clock should start making audible sounds.
### Link:
https://github.com/ROSHAN-KHANDAGALE/Alarm-Clock

### Which lines from which files:
Main.py
lines 6-8
def set_alarm():
    alarm_time = InputAlarm.get()
    LocalTime = time.strftime("%H:%M:%S")

### Why?
creates a function to input a time for the alarm to go off 

# - Code for a rocket targeting system.

### Link: 
https://github.com/abnsl0014/Missile-Guidance-System
### Which lines from which files
Trajectory.py
1-38
### Why?
This section creates the trajectory for a missle 

# - File compression utility algorithm.

### Link: 
https://github.com/dropbox/lepton/blob/master/CMakeLists.txt
### Which lines from which files
CMakeLists.txt whole file
### Why?
This whole file can help compress arbiratry file types into smaller items

# - Weather forecasting algorithm.

### Link: 
https://github.com/Prati5/WeatherPrediction/blob/master/weatherPrediction.ipynb
### Which lines from which files
weatherPrediction.ipynb

In [6]
from sklearn.model_selection import train_test_split 
xtrain, xtest, ytrain, ytest = train_test_split( x, y, test_size=1/3, random_state=0 )
### Why?
These lines are used to start the training for a forecasting algorithm
the entire file then goes through and does some very complicated math that I dont fully understand to help calculate the weather forcast based on the inputs
# - E-commerce checkout system process.

### Link: 
https://github.com/Riadz/E-commerce/blob/master/checkout.php
### Which lines from which files
Checkout.php, the whole file
### Why?
 this entire file goes through and specifies the webapage for a ecommerce checkout system process

# - Social media post scheduler.

### Link: 
https://github.com/allenheltondev/social-media-scheduler/blob/main/state-machines/schedule-social-post.asl.json
### Which lines from which files
state-machines/schedule-social-post.asl.json
11-19
"StartAt": "Has Reference Number?",
        "States": {
          "Has Reference Number?": {
            "Type": "Choice",
            "Choices": [
              {
                "Variable": "$.detail.referenceNumber",
                "IsPresent": true,
                "Next": "Move up reference number"
### Why?
This entire file goes through creating the schedules, also has multiple bug correctors, like checking if there is a duplicate schedule before proceeding
I was struggling with this one to find specific lines to quote, each file interacts with each other in different ways 
# - Fitness app calorie counter.

### Link: 
https://github.com/s-shemmee/Calories-Calculator-Python/blob/main/clr_calculator.py
### Which lines from which files
def main():
    welcome()
    gender = sex()
    weight = get_weight()
    height = get_height()
    age = get_age()
    rest_bmr = calculate_bmr(gender, weight, height, age) 
    total_calculation(rest_bmr)
### Why?
This is the closest I could find that I was able to understand, this uses python to calculate your BMI from your input

# - Online voting system mechanics.

### Link: 
https://github.com/shah-deep/Online-Voting-System/blob/main/registerVoter.py
### Which lines from which files
registerVoter.py
9-20
def reg_server(root,frame1,name,sex,zone,city,passw):
    if(passw=='' or passw==' '):
        msg = Message(frame1, text="Error: Missing Fileds", width=500)
        msg.grid(row = 10, column = 0, columnspan = 5)
        return -1

    vid = df.taking_data_voter(name, sex, zone, city, passw)
    for widget in frame1.winfo_children():
        widget.destroy()
    txt = "Registered Voter with\n\n VOTER I.D. = " + str(vid)
    Label(frame1, text=txt, font=('Helvetica', 18, 'bold')).grid(row = 2, column = 1, columnspan=2)


### Why?
These lines allow sonmeone to register to vote using this code.
creates a server for registeration to have an account to vode by defininf the reg_server var

# - Automated email response system.

### Link: 
https://github.com/sunborn23/python-email-autoresponder
### Which lines from which files
autoresponder.config.ini
17-25
[mail content settings]
mail.request.from = sender-address@example.com
mail.reply.subject = Message received
mail.reply.body:
    Hi there!

    Thanks for your message.

    The Python Reply-To Autoresponder
### Why?
This section allows you to specify what you want to say in the auto responded message, this would  be very helpful because you can specify what you want it to say
by using the mail.reply.body we can store what we want into this to send
# Personal blurbs

### 1
registration and log in systems
### Link: 
https://github.com/lyushher/Login-System/blob/main/LoginSystem.py
### Which lines from which files
LoginSystem.py
16-27
def register():
    global register_screen
    register_screen = Toplevel(main_screen)
    register_screen.title("Register")
    register_screen.geometry("320x350")

    global username
    global password
    global username_entry
    global password_entry
    username = StringVar()
    password = StringVar()
### Why?
these lines layout the beginning of the registration system for this python script 
starts with setting the username and password to string variables to store the names

### 2
calculator system
### Link: 
https://github.com/AceLewis/my_first_calculator.py/blob/master/my_first_calculator.py
### Which lines from which files
my_first_calculator.py
all lines
### Why?
maybe the worst calculator ive ever seen coded, has seperate lines for each equation instead of just creating a variable, I thought it was funny and wanted to share

### 3
How a calander defines the months
### Link: 
https://github.com/FilaMarek/JavaScript-Calander/blob/master/script.js
### Which lines from which files
script.js
6-22
var tday = new Date().getDate();
var currentMonths = new Date().getMonth();// what month it is
var Months = currentMonths;
var year =  new Date().getFullYear();
var days = new Date().getDate();//day of the month ex 11
var daysOfTheweek = new Date().getDay(); // days of the week ex 6 === sat
var weekNumber = 0;
var tempMonths = Months +1;
var dateobj =  new Date(tempMonths  +" " + 1 + " " + year)
var tempDay = 1;
var tempMonths = Months + 1;
var tempYear = year;
var currentCalMode = 0; // 0 is Month mode, 1 is week mode, 2 is day Mode
var textMonth = " "
var numberOfTotalWeeks = 5;
var d,m,y,scheduleEvent, compareArr,tempVar, tempVar2,divEvent,tdayMonth,Monthchecker,z;

### Why?
these lines start the variables for the different months, days, and years