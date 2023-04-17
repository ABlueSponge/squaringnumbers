import random
import time
score = 0
average = []
numbers = []
#fix the numbers appearing twice
#add a summary at the end
#add explanation for wrong answers
while True:
    x = 0
    number = random.randint(10,99)
    while True:
        if number in numbers:
            number = random.randint(10,99)
        else:
            break
    answer = number ** 2
    numbers.append(number)
    start = time.time()
    result = input(f"{number}^2: ")
    end = time.time()
    totaltime = end - start
    if int(result) == answer:
        score+=1
        average.append(totaltime)
        for i in average:
            x += i
        averagetime = x/len(average)
        print(f"Correct. Score: {score}. Time: {round(totaltime, 2)}. Average: {round(averagetime,2)}")
    else:
        print(f"Wrong. Correct answer is {answer}")
