---
layout: posts
title: My first drawing with Python
---

- I wrote some code.
- I used turtle module.
- There is it's code:
import turtle
turtle.setheading(90)
turtle.bgcolor("lightblue")

def tree(l,a,s):
    if l>30:
        turtle.pensize(s)
        turtle.forward(l)
        turtle.left(a)
        tree(l*0.7,a,s-1)
        turtle.right(2*a)
        tree(l*0.7,a,s-1)
        turtle.left(a)
        turtle.backward(l)
    else:
        turtle.color("green")
        turtle.begin_fill()
        turtle.circle(10)
        turtle.end_fill()
        turtle.color("#8B4513")
    




def cloud(x,y):
    c=turtle.Turtle()
    c.penup()
    c.setpos(x,y)
    c.color("white")
    c.begin_fill()
    c.circle(40)
    c.end_fill()
    c.pendown()

def sun(x,y):
    c=turtle.Turtle()
    c.penup()
    c.setpos(x,y)
    c.color("yellow")
    c.begin_fill()
    c.circle(100)
    c.end_fill()
    c.pendown()
    

def grass():
    g=turtle.Turtle()
    g.color("green")
    g.penup()
    g.goto(-500,-350)
    g.begin_fill()
    for i in range(2):
        g.forward(1000)
        g.left(90)
        g.forward(50)
        g.left(90)
    g.end_fill()


turtle.penup()
turtle.setheading(90)
turtle.speed(0.1)
turtle.setpos(0,-300)
turtle.pendown()
turtle.color("#8B4513")
# sky()
tree(180,20,10)
turtle.penup()
turtle.setheading(90)
turtle.speed(0.1)
turtle.setpos(-100,-300)
turtle.pendown()
turtle.color("#8B4513")
tree(100,20,10)
turtle.penup()
turtle.setheading(90)
turtle.speed(0.1)
turtle.setpos(-200,-300)
turtle.pendown()
turtle.color("#8B4513")
tree(150,20,10)
turtle.penup()
turtle.setheading(90)
turtle.speed(0.1)
turtle.setpos(100,-300)
turtle.pendown()
turtle.color("#8B4513")
tree(100,20,10)
turtle.penup()
turtle.setheading(90)
turtle.speed(0.1)
turtle.setpos(200,-300)
turtle.pendown()
turtle.color("#8B4513")
tree(70,20,10)
turtle.penup()
turtle.setheading(90)
turtle.speed(0.1)
turtle.setpos(260,-300)
turtle.pendown()
turtle.color("#8B4513")
tree(150,20,10)
grass()
cloud(290,280)
cloud(260,270)
cloud(320,270)
cloud(30,270)
cloud(0,260)
cloud(60,260)
cloud(-30,270)
cloud(-60,260)
sun(-350,200)

turtle.mainloop()


# this is a header

<iframe width="560" height="315" src="/assets/images/image2.png" title="Drawing" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

