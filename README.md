# Python Lindenmayer(L)-System Parser & Visualizer Home
In this repository, you will find all versions of the **educational showcase** project _Python L-System Parser and Visualizer_.
* [Version 1.0.0](https://github.com/hunterpope03/python-l-system-parser-and-visualizer/tree/main/v1.0.0)

## What is an L-System?
A [Lindenmayer(L)-System](https://en.wikipedia.org/wiki/L-system) is a mathematical model first invented by the Hungarian biologist and botanist [Aristid Lindenmayer](https://en.wikipedia.org/wiki/Aristid_Lindenmayer). An L-System works by repeatedly transforming character(s) in a string into a longer, more complex string of characters. Originally used to model the growth of bacteria and algae, L-Systems have grown to be used in textiles, games, neural networks, and art. 

An L-System is composed of the following two attributes: 
* **Axiom / Seed**: an initial starting value
* **Production / Transformation Rules**: definitions of how to replace each character or string into a more complex string

#### Consider this example: 

###### Axiom = F

###### Transformation rules = F -> F + G and G -> G + H

In the first iteration, the axiom, F, is replaced via the transformation rule for F:
* ###### F -> F + G 

In the following iterations, all of the characters in the resulting string, F + G, are again replaced by the transformation rules for both characters: 
* ###### F + G -> (F + G) + (G + H)

With more more complex axioms and transformation rules and increased iterations, L-System strings can grow to huge lengths. 

##### Consider exploring Paul Bourke's [L-System Manual](https://paulbourke.net/fractals/lsys/), which was integral in my understanding of the concept.

## An L-System Parser & Visualizer Program

A parser, in programming terms, breaks down data into smaller pieces. So, think of each character in an axiom as a piece that represents something larger (a longer string). A parser will apply transformation rules for a given number of **iterations**.

The visualization process is a bit more complex. In a parsed string, there are commonly: 
* **Variables** - values that are changed in each transformation rule (usually letters)
* **Constants** - values that are not changed in a transformation rule, but rather define a geometric action (+ to turn, [ to create a new branch, etc.)

So when a visualizer takes in a parsed string, each character is a command. Some additional requirements for a visualizer might be: 
* **Turn Angle** - defines the angle at which to turn
* **Starting Direction** - defines the angle at which to start the plot; allows for rotation

Using all of this information, a visualizer is fed a parsed string and creates a complex drawing. Changing the axiom, rules, and angles allows for a plethora of possible figures to be created.

Note that some programs may be more or less complex, supporting either more or less commands/features.

## Example Visuals (from v1.0.0)

Here are some examples from my first version of this project: 

##### Dragon Curve, via [Paul Bourke](https://paulbourke.net/fractals/lsys/)
<img width="786" alt="Dragon Curve System" src="https://github.com/user-attachments/assets/8059714b-c948-45b9-86c5-8ea79d283c44" />

##### L-System Bush 2, via [Paul Bourke](https://paulbourke.net/fractals/lsys/)
<img width="786" alt="L-System Bush 2" src="https://github.com/user-attachments/assets/9e480602-16bc-43aa-93d2-da18039eb834" />

##### Pentaplexity, via [Paul Bourke](https://paulbourke.net/fractals/lsys/)
<img width="786" alt="Pentaplexity" src="https://github.com/user-attachments/assets/c85a5640-4eff-46b5-8946-d103826717e6" />

##### Sierpinski Arrowhead, via [Paul Bourke](https://paulbourke.net/fractals/lsys/)
<img width="786" alt="Sierpinski Arrowhead" src="https://github.com/user-attachments/assets/ccfac4b6-90be-49fd-8a82-ae927cdb4e04" />

##### Quadratic Gosper, via [Paul Bourke](https://paulbourke.net/fractals/lsys/)
<img width="786" alt="Quadratic Gosper" src="https://github.com/user-attachments/assets/c5808f2d-6b85-4b3e-86d6-16b12c5b7618" />

