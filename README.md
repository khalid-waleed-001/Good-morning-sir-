# Good-morning-sir-
Python is one of the most demanded programming languages in the job market, Make a program in python which capable of  greeting you with good morning and good afternoon by using time modules 
import time

# Fetch current time in HH:MM:SS format
timestamp = time.strftime('%H:%M:%S')
print("Current Time:", timestamp)

# Fetch hour, minute, second separately
hour = int(time.strftime('%H'))  # Convert string to integer
minute = time.strftime('%M')
second = time.strftime('%S')

print("Hour:", hour)
print("Minute:", minute)
print("Second:", second)

# Greeting logic (compare integer hour)
if hour < 12:
    print("Good Morning!")
elif hour < 17:  # 12 PM to 5 PM
    print("Good Afternoon!")
elif hour < 21:  # 5 PM to 9 PM
    print("Good Evening!")
else:  # After 9 PM
    print("Good Night!")
