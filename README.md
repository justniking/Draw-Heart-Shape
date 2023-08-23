# DrawHeartShape
from turtle import *

def draw_heart():
    penup()
    goto(0, -200) # Start from the bottom of the heart
    pendown()
    begin_fill()
    fillcolor("violet")
    left(140)
    forward(224)
    circle(-112, 200) # Left side of the heart
    setheading(60)    # Set direction for the right side
    circle(-112, 200) # Right side of the heart
    forward(224)
    end_fill()

def write_text():
    penup()
    goto(0, -30) # Centered position for the text
    pendown()
    color("aqua")
    write("I Luv AI", align="center", font=("Arial", 30, "bold"))

bgcolor("paleturquoise")
pensize(0)
draw_heart()
write_text()
hideturtle()
done()
