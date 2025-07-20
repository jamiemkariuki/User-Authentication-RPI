# User-Authentication-RPI
# Fingerprint Authentication System

## Problem
Students at St Nicholas face issues when it comes to arriving at school. The need to write names inside a book can be very lengthy and cause long queues. There is a need for a faster way, a way that only with a slight movement you are okay to go and no need to write your name. Students also like to cause trouble sometimes by writing false names which also raises the need for a way to stop this problem and allow for precise, accurate data to be automatically sent without the need for proofreading.

## Goal
To create a user authentication system that uses a fingerprint module and forms hosted on a web server. The user should be able to enter their name, age, and email address into the form. The user should then be prompted to input their fingerprint into the circuit. User data will then be stored, and on a recognized fingerprint scan, their name, age, and email address will be printed onto an LCD screen. The user should be able to delete their account on the web server and have a dashboard to customize what should be printed onto the LCD screen upon fingerprint scan. The user should also be able to store this data somewhere (e.g., Mzizi) to allow for automatic checking instead of writing names.

## Technologies Used
- **Python** (using RPi.GPIO and pyserial) for controlling Raspberry Pi GPIO pins and serial communication
- **Tinkercad** for circuit design and testing
- **GitHub** for version control

## Plan
A web server should be hosted on the Raspberry Pi using PHP to display a form . Form data will then be sent to the backend. Upon form completion, a buzzer will ring for 10 seconds, signifying that the fingerprint needs to be put. Once the fingerprint is placed by the user, it will be stored in the MySQL database together with the form data, and the LCD screen will print "Sign Up successful!".

When a fingerprint is input, the program will read the database and check for a matching fingerprint. If one is found, the form data associated with it is printed on the LCD screen, with buttons to turn it off or on.

There should also be a dashboard where users can delete their information from the database or customize the message displayed on the LCD screen upon scanning their fingerprint again.

The circuit will be planned and designed on Tinkercad to ensure minimal errors and will be available in the GitHub repository as both a .brd file and an image
