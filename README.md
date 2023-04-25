# Specific
This is my first repository
This  is my first project
import datetime
from playsound import playsound

alarmHour = int(input("Enter the Hour: "))
alarmMin = int(input("Enter the Minutes: "))

alarmAm = input("am / pm: ")

if alarmAm == "pm":
    alarmHour += 12

while True:
    if alarmHour == datetime.datetime.now().hour and alarmMin == datetime.datetime.now().minute:
        print("Playing..")
        playsound("punky.mp3")
        break
        

