# magic-8ball

import random
import time

list = ["Yes, most definitely!", "The chances are high!", "Not likely!", "May the odds be ever in your favor.", "You got no shot, kid.", "Try it out and see!", "99.9% success rate", "Congratulations, yes!", "Ask again later", "It's better if you don't know my answer", "Cannot predict now", "Concentrate and ask again", "Don't count on it", "YASSS buddy YASSS!", "NAHHH!"]

def userinput():
        question = 'Enter your question:'
        print(question)
        stuff = input(">1")
 
        print("\nThinking..\n")
        time.sleep(3)
        print(random.choice(list))
       
        final()
       
def final():
        print("Would you like to ask another question?")
        user_reply = input('> ')
        while(input):
                if user_reply == "yes" || “YES” || “Yes”:
                        userinput()
                else:
                        print("Thanks for playing!")
                        break
print("Welcome to the Magic 8 Ball!")
userinput()
