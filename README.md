# Infotc1000-final-project
## by Ian McCormick
 *Hello*  **everyone**, I am a freshman student at the University of Missouri.  
 I would like to share some of my coding experience with a project I created using python. This program will take users input for rate, time, initial position, and acceleration. Then the program will calculate the 
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
 ### Hobbies
 #### Video Games
 I love to play video games. Here are some of my favorite games:
 
 - Red Dead Redemption 
 - Red Dead Redemption 2
 - Grand Theft Auto IV
 - Battlefield 1
 - Mafia
 - Mafia 2
 - Mafia 3
 - Call Of Duty Black Ops Cold War  
 I like to play a mix of Story based games as well as multiplayer games. I really love the story and protagonists in the above games. Red dead Redemption 1 and 2 as well as Grand Theft Auto IV are made by Rockstar games. I will leave a link to their website here. [Rockstar Games](https://www.rockstargames.com)
  
  
  
  
  
  
  
  ### Guns
  I am very enthusiastic about guns, gun history, as well as our second amendment. Before I came to Mizzou I shot at ranges back home. Once I have my own place I can hopefully start buying my own guns. I have a list of firearms I want to own.
  
