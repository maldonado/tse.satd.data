# Labeling Self-Admitted Technical Debt Comments

## Theory

### Source code comments

Source code comments are a useful tool that most programming languages supports. Source code comments are identified by a programing language specific syntax. For example, one possible way to make a source code comment in Java is by using "\\". Any text entered as a source code comment does not interfere in how the implementation behaves. Therefore, source code comments allows developers to document, clarify and express concerns about the implementation in an informal manner that does not impact the functionality of the program. 

### Technical debt

Technical debt is a metaphor coined to express the trade off between productivity and quality. For example, when developers take shortcuts or perform quick hacks. These non-optimal solutions may help the project to move faster at first, but they mostly like will hinder the development in the long run. In other words, "interest" will be paid in the project in the form of effort because of the technical debt took beforehand.

### Self-admitted technical debt

Self-admitted technical debt is technical debt admitted by the developer through source code comments. Different types of technical debt are used to provide more insightful description of the non-optimal solution.

**Self-admitted design debt:** These comments indicate that there is a problem with the design of the code. They can be comments about misplaced code, lack of abstraction, long methods, poor implementation, workarounds or a temporary solution. The following source code comments are examples of self-admitted design debt:

* “TODO: - This method is too complex, lets break it up” - [from ArgoUml]
* “/* TODO: really should be a separate class */” - [from ArgoUml]
* “// I hate this so much even before I start writing it. // Re-initializing a global in a place where no-one will see it just // feels wrong. Oh well, here goes.” - [from ArgoUml]
* “//quick & dirty, to make nested mapped p-sets work:” - [from Apache Ant]
* “// probably not the best choice, but it solves the problem of // relative paths in CLASSPATH” - [from Apache Ant]
* “//I can’t get my head around this; is encoding treatment needed here?” - [from Apache Ant]

**Self-admitted defect debt:** In defect debt comments the author states that a part of the code does not have the expected behavior, meaning that there is a defect in the code.

* “// Bug in above method” - [from Apache Jmeter] 
* “// WARNING: the OutputStream version of this doesn’t work!” - [from ArgoUml]

**Self-admitted documentation debt:** In the documentation debt comments the author express that there is no proper documentation supporting that part of the program.

* “// FIXME This function needs documentation” - [from Columba]
* “// TODO Document the reason for this” - [from Apache Jmeter]

**Self-admitted requirement debt:** Requirement debt comments express incompleteness of the method, class or program as observed in the following comments:

* “/TODO no methods yet for getClassname” - [from Apache Ant]
* “//TODO no method for newInstance using a reverse-classloader” - [from Apache Ant]
* “TODO: The copy function is not yet * completely implemented - so we will * have some exceptions here and there.*/” - [from ArgoUml]

**Self-admitted test debt:** Test debt comments are the ones that express the need for implementation or improvement of the current tests. As shown in the examples below, test debt comments are very straight forward in their meaning. 

* “// TODO - need a lot more tests” - [from Apache Jmeter]
* “//TODO enable some proper tests!!” - [from Apache Jmeter]

For more details you can refer to our paper on the subject:
*E. d. S. Maldonado and E. Shihab, “Detecting and quantifying different types of self-admitted technical debt,” in Proceedings of the 7th International Workshop on Managing Technical Debt, 2015, pp. 9–15.*

## Your task

1. Check if you received the URL that hosts the labeling web application in your email.
2. Access the URL and select your name from the drop down list.
3. The tool will present to you one source code comment at a time. After carefully reading it, you should select what type of self-admitted technical debt the source code should be classified as. To do this, just click in one of the five labeled bottoms in the screen (i.e, Design, Defect, Documentation, Requirement and Test). In addition, if you consider that there is not self-admitted technical debt in the source code comment, you should click in the button labeled as "without technical debt". If you misclassified a source code comment you can use the "back" button to reload the previous source code comment.
4. After classifying a source code comment the next source code comment from the sample will appear on your screen, repeat the process until finished. The process bar will show at all times how close you are to finish your task.
5. There is no time limit to complete your task. If you desire to pause the classification process you can close your web browser and restart your work later by repeating steps 1 and 2.

