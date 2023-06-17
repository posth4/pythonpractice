# Chapter 4 Exercises

## Algorithm Workbench 1 
In this excersise, we are asked to write a while loop that lets a user enter a number that can be multiplied by 10 with the result being assigned to the variable named product, this product though should not produce a product above the number 100. 


```python
product=0

while product < 100:
    number= int(input('Enter a number:'))
    product=number * 10
    print ('Product:', product)
print('Product is larger than zero, now we exit this loop')q
                

```

    Enter a number: 5


    Product: 50


    Enter a number: 10


    Product: 100
    Product is larger than zero, now we exit this loop


The problem above represents a while loop, this is a statement where the loop is tested for a value that is either true or false to the value, as long as the statement is true then the loop will continue. For this question, the loop will end when the statement is above the value of 100. I showed that entering the value 5 will produce the value of 50, which allows this while loop to continue. When I entered the number 10, it showed the product being 100, which will end this loop.

## Algorithm Workbench 3
For this exercise, we are asked to represent a for loop that displays numbers added by 10 each time from zero to a thousand. 


```python
for number in range (0, 1001, 10):
    print (number)

```

    0
    10
    20
    30
    40
    50
    60
    70
    80
    90
    100
    110
    120
    130
    140
    150
    160
    170
    180
    190
    200
    210
    220
    230
    240
    250
    260
    270
    280
    290
    300
    310
    320
    330
    340
    350
    360
    370
    380
    390
    400
    410
    420
    430
    440
    450
    460
    470
    480
    490
    500
    510
    520
    530
    540
    550
    560
    570
    580
    590
    600
    610
    620
    630
    640
    650
    660
    670
    680
    690
    700
    710
    720
    730
    740
    750
    760
    770
    780
    790
    800
    810
    820
    830
    840
    850
    860
    870
    880
    890
    900
    910
    920
    930
    940
    950
    960
    970
    980
    990
    1000


The above code represents the for loop that adds by 10 each time to get to one thousand. I was able to figure out this problem by using the range function to go from 0 to 1000 in incrimintes of 10. I had to include the starting number, which was 0, the end value, being 1001 because the code will exclude the last value of the number, and the size of number the code moves, being the number 10. The code then runs using the print statement and results in the above code.

## Programming Exercise 1 - Bug Collector 
In this exercise, we refer to a bug collector who collects bugs every 5 days, we are asked to write a program that keeps a running total of the number of bugs collected during the five days.


```python
NUMBER_0F_DAYS = 5
dailyCollection = 0
total5DayCollection = 0
message = ''

for day in range(NUMBER_0F_DAYS):

    dailyCollection = int(input("How many bugs collected on day " + format(day + 1) + ': '))

    while dailyCollection < 0:
        dailyCollection = int(input("Error. Enter a positive number: "))

    total5DayCollection += dailyCollection

message = 'Total number of bugs collected for 5 days = ' + format(total5DayCollection);

print(message)
```

    How many bugs collected on day 1:  5
    How many bugs collected on day 2:  10
    How many bugs collected on day 3:  7
    How many bugs collected on day 4:  11
    How many bugs collected on day 5:  12


    Total number of bugs collected for 5 days = 45


To describe how I solved the coding problem above first I set the variables to a specific number, Number of days equal to 5, daily collecetion equal to zero, total 5 day collection equal to zero, and the empty message. Second, I created a for loop in correlation to the 5 days of collection. Then I formatted the days of collection using the correct input. Following this I created a while loop for the daily collection that tells us to always keep the product a positive number and to end at the 5 day mark. Then the message statement describes how to format the given strings and the print statement allows the code to print the final message. 
