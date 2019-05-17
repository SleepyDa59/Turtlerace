# Turtlerace
# basic turtle race
from turtle import *
from random import randint

k = {}
raceList = []

turtle1 = (input('enter name for turtle 1: '))
turtle2 = (input('enter name for turtle 2: '))
turtle3 = (input('enter name for turtle 3: '))
turtle4 = (input('enter name for turtle 4: '))


speed(10)
penup()
goto(-140, 140)

for step in range(15):
    write(step, align='center')
    right(90)
    forward(10)
    pendown()
    forward(150)
    penup()
    backward(160)
    left(90)
    forward(20)

turtle1 = Turtle()
turtle1.color('red')
turtle1.shape('turtle')

turtle1.penup()
turtle1.goto(-160, 100)
turtle1.pendown()

turtle2 = Turtle()
turtle2.color('blue')
turtle2.shape('turtle')

turtle2.penup()
turtle2.goto(-160, 70)
turtle2.pendown()

turtle3 = Turtle()
turtle3.color('green')
turtle3.shape('turtle')

turtle3.penup()
turtle3.goto(-160, 40)
turtle3.pendown()

turtle4  = Turtle()
turtle4.color('pink')
turtle4.shape('turtle')

turtle4.penup()
turtle4.goto(-160,10)
turtle4.pendown()


for turn in range(108):
    turtle1.forward(randint(1, 5))
    turtle2.forward(randint(1, 5))
    turtle3.forward(randint(1, 5))
    turtle4.forward(randint(1, 5))

#for order in range(105):

k=input("press close to exit")
