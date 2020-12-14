# Infotc1000-final-project
## by Ian McCormick
 *Hello*  **everyone**, I am a freshman student at the University of Missouri. 
 
 I am planning to obtain some business degree. But, I am unsure of which one yet.
 
 I would like to share some of my coding experience with a project I created using python. This program will take users input for rate, time, initial position, and acceleration. Then the program will calculate the distance traveled.
 ```python
def calculate():
    
    bad_input = True

    #while bad_input is True the loop will continue to execute
    while bad_input:
        try: 
            #ask user for input: distance and time

            r = float(input("Enter the rate: "))
            t = float(input("Enter the time: "))
            x_0 =float(input("Enter the initial position: "))
            a =float(input("Enter the acceleration: "))
            
        except ValueError:
            print("The value you entered is invalid. Only numerical values are valid")
            continue

        #if the user enters a negative number go back to the beginning of the loop
        if  t < 0:
            print("Values for rate and time must be 0 or greater.")
            print("Please enter input again\n")
            continue

        #calculate the distance
        distance = x_0 + r*t + 0.5*a*(t**2)

        #print distance to use
        print("The distance is", distance)

        #Set bad_input to False if all previous code in the try block executes successfully
        #Setting bad_input to False will cause the while loop to end
        bad_input = False
        
        

def main():
    while True:
        calculate()

        do_again = input("Would you like the program to continue? Y/y: ")
        if do_again != "Y" and do_again != "y":
            print("Thank you and goodbye.")
            break

           
        


#call main to begin the program
main()


 ```
 Here is another project that I did using python. This project used turtle graphics to draw a random image. I had mine draw lines in random directions and using multiple different colors
 
 ```Python
 import random 
from turtle import Turtle
def recursive_random(turtle, angle, length):
    colors = ["green", "red", "blue", "yellow","purple"]
    color = random.choice(colors)
    turtle.color(color)
    turtle.right(angle)
    turtle.forward(length)
    length = length + 2
    angle = angle + 56
    if (length > 0):
        recursive_random(turtle, angle, length)

    

def main():
    ANIMATION_SPEED = 0
    turtle = Turtle()
    turtle.speed(ANIMATION_SPEED)
    recursive_random(turtle, 0, 73)
    
    
main()

```
Lastly, this python asks the user for sq of wall space to be painted and the price of paint per gallon. Then it will calculate the total cost including paint and labor.

```python
import math
print("This program asks for sq of wall space to be painted and the price of paint per gallon")
do_calculation = True
while(do_calculation):
    while (True):
        try:
            space = float(input("\nEnter the square feet of wall space to be painted: "))
            if(space < 0):
                print("negative values aren't allowed")
                continue
        except ValueError:
            print("The value entered is invalid please enter numerical values only");
        else:
            break
        
    while (True):
        try:
            price = float(input("\nEnter the price of paint per gallon: "))
            if(price < 0):
                print("negative values aren't allowed")
                continue
        except ValueError:
            print("The value entered is invalid please enter numerical values only");
        else:
            break
    p = space/350
    labor = 62.25 * (p * 6)
    gal = math.ceil(p)
    paint = price * gal
    cost = labor + paint

    print("Total cost of labor: $",format(labor,".2f"))
    print("Total cost of paint: $", paint)
    print("gallons of paint required", gal)
    print("Hours of Labor required", format(p * 6,".1f"))
    print("Total cost of paint job: $", cost)

    another_calculation = input("\nDo you want to perform another calculation? (y/n): ")
    if (another_calculation != "y"):
        print("Goodbye")
        
        do_calculation = False
```
 I would also like to share a bit about myself.
 ### Hobbies
 
 
 #### Video Games
 I love to play video games. I have played them since I was in elementary school. Starting with website flash games and now I currently play on my Playstation 4. And I will probably contiinue to play them for the rest of my life. Here are some of my favorite games:
 
 - Red Dead Redemption 
 - Red Dead Redemption 2
 - Grand Theft Auto IV
 - Battlefield 1
 - Mafia
 - Mafia 2
 - Mafia 3
 - Call Of Duty Black Ops Cold War  
 I like to play a mix of Story based games as well as multiplayer games. I really love the story and protagonists in the above games. Red dead Redemption 1 and 2 as well as Grand Theft Auto IV are made by Rockstar games. I will leave a link to their website here. [Rockstar Games](https://www.rockstargames.com) 
 
 My favorite game by Rockstar is Red Dead Redemption 2. I won't spoil anything, but its about a gang of outlaws in America during 1899. It tells the story of Arthur Morgan and later John Marston and the gang to which they call their family. It serves as a prequel to the first Red Dead Redemption. It is an amazing story with great gameplay with hours of side quests and challenges as well as online mode.
 
 Compared to Rockstar games the mafia series is less known, but its plot is amazing. The first game which came out in 2000 was recently remastered a few months ago. It tells the story of Italian immigrant Tommy Angelo. A cab driver in 1930's lost heaven. (a fictional American city based off of Chicago) A straight edge man at first, but after a run in with the mob he realizes the rewards of organized crime are too big to ignore.
 
 Battlefield 1 is a multiplayer first person shooter set during World War One. The gameplay is amazing and is my favorite multiplayer game of all time.
  
  
  
  
  
  
  
  ### Guns
  I am very enthusiastic about guns, gun history, as well as our second amendment. Before I came to Mizzou I shot at ranges back home. Once I have my own place I can hopefully start buying my own guns. I have a list of guns I want to own. I will leave links to images of these guns and their history below.
  
  [Colt M1911](https://en.wikipedia.org/wiki/M1911_pistol)
  
  [AK-47](https://en.wikipedia.org/wiki/AK-47)
  
  [Remington 870](https://en.wikipedia.org/wiki/Remington_Model_870)
  
  I have a few reasons for choosing these guns. The Colt M1911 and the AK-47 have a lot of historic value and are 2 of the most well known firearms. With the AK-47 being the most produced gun in the world. The Soviet made AK-47 is also a symbol of revolution it can even be found on the flag of Mozambique. The American Colt M1911 was also very important and saw a lot of usage from WW1 until the 1980s until NATO called for American to have their armed forces use the M9 Beretta instead. I choose the Remington 870 because I feel that it is a very good choice for home defense. Any home intruder will be instantly scared off by the racking of this gun. These guns are for recreational purpsoes as I love to go to the range and shoot it is very fun and I would recommend it to anyone. But they are also for safety/personal defense.
  
  
  
  
  
  
  ### TV Shows/Entertainment
  My favorite tv shows are South Park and Family Guy. These shows always leave me laughing at their ridiculous shock humor. Eric Cartman is my favorite character from South Park. He is a manipulative mastermind who always gets what he wants. He constantly uses everyone around him to get what he wants and he is very entertaining to watch. Peter Griffin is my favorite character from Family Guy. He is very funny and always has crazy shenanigans that gets him and his friends/family in trouble. I also love Family Guy for their infamous cutaway gags.Both shows have been around for a long time. South park has been running since 1997 and Family Guy has been running since 1999. Besides TV I also love to watch Youtube. I will leave some of my favorite channels below.
  
  [MrBeast](https://www.youtube.com/user/MrBeast6000)
  
  MrBeast whom you might have a good chance of knowing already is a philanthropist who gives away a lot of money through challenges and also has very other entertaining videos on his channel.
  
  [Luna](https://www.youtube.com/user/AustinFFA)
  
  I've watched him for a while he does storytime videos about his life with gameplay in the background.
  
  [Brewstew](https://www.youtube.com/user/brewstewfilms)
  
  This guy tells stories about his life, but has it in a crude animated formant. His sense of humor is very funny.
  
  [Poofesure](https://www.youtube.com/user/Poofesure) 
 
 This guy runs a gaming channel and he is very funny because whenever he does poorly (which is pretty often) he will rage and scream and it is very entertaining to watch.
 
 
 
 
 ## Other things to know 
 
 I am learning Chinese and have been since middle school. Besides Chinese, I also love to learn about other countries and cultures in general. I find learning about other cultures/countries to be very intriguing and it also allows me to have a different perspective on America. And just like anyone else I love to have fun with my friends.
  
  
  

