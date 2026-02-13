# N5-Assignment
import random

counter = 0
decision = "yes"

mysteryFruit = ["apple" "banana" "blueberry" "kiwi" "mango" "orange" "peach" "pineapple" "raspberry" "strawberry"]

userFruits = []

while decision == "yes" and counter <6:
    # 5. get and store valid fruit selection (input validation)
    userInput = input("please enter the fruit name: ")
    while len(userInput) <4:
        print("incorect fruit name length")
        userInput = input("please enter the fruit name: ")
    # 6. add 1 to counter
    counter = counter +1
    # 7. get and store decision regarding entering another fruit
    decision = input("do you wnat to enter another fruit: ")

number = random.randit(0,9) # if you are using random, remember to "import random"

print("the fruits you entered were.")

for index in range(counter):
    print(userFruits[index])

print("the mystery fruit is ", mysteryFruit[number])

counter = counter + 1

if counter <3:
    # 15. display milkshake message
    print("milkshake")

elif counter ==3 or counter == 4:
    # 17. display smoothie message
    print("smoothie")

else:
    print("fruit juice")