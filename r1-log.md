# #100DaysOfCode Log - Round 1 - Saurav Uppoor

The log of my #100DaysOfCode challenge. Started on August 18, 2019.

## Goals:
* [ ] Complete Udemy's Complete JavaScript Course
* [ ] Complete FCC Responsive Web Design Certification
* [ ] Build a Portfolio Website
* [x] ~Reach 1200 points on TSEC CodeCell Website~
  * [ ] Complete Easy Level problems of Stack, Array, Queues, Linked List on HackerRank

________________________________________________________________________________________________________________________________
# __Round 1 - Log__
---

### __Day 21: Queues Data Strucutre and String programs in Java__
#### Sept 9, 2019 - Monday

#### Progress: 
* Queues DS implentation (ADT, Arrays, Linked List)
* Strings in java
* Also completed goal __Reach 1200 points on TSEC CodeCell Website__. New Goal updated!

#### Summary:
* __Data Structures__ *approx 1 hour*
 * Queues Data Strucutre:
   * Details about Queues ADT and its operations.
   * Array Implementation of Queues
   * Linked List implementation of Queues
   * Time complexity
   
  * __Java Revision__ *Academics 2 hours*
   * Wrote program for 3 problem statments stated below:
   1. Sorting Strings in lexical way.
   2. Counting the upper, lower, special chars, digits and blank spaces in the entered string.
   3. Menu driven program for understanding various string buffer class methods.

#### Plan of action tomorrow / Thoughts:
* Write programs for linear, circular and priority Queues.
* Implement various searching algorithms.
* HackerRank problem on Queues, time permitting.

#### Link / Screenshots:
<img src = "https://prnt.sc/p3ws4l" width = 800 heigth = 500>
______________________________________________________________________________________________________________________________________

### __Day 20: DS Sorting Techniques and Javafx Gridpane__
#### Sept 8, 2019 - Sunday

#### Progress: 
* Leanrt about Gridpane in javafx
* Created a basic login window with form validation
* Revised the Sorting Algorithms
 * Bubble Sort
 * Insertion Sort
 * Merge Sort
 * Quick Sort
* Solved 2/3 problems of TCC Week 6

#### Summary:
* __Javafx__: *Approx 45 minutes*
 * ```GridPane``` class is a layout type that allows the users to arrange the components in grid format(consisting of rows and columns). While attaching the components we  need to specify the row and column of the grid in which we want to TTch it in.
 * New stuff learned :
  * ```GridPane.setPadding(Insets)``` helps us to set the padding arround the scene and the stage. ```insets``` is an object that takes in 4 integer values that are TRBL padding (just like the HTML one).
  * New components -> ```Label``` and ```TextField```
  * ```setVGap(value)``` sets the vertical gap between the components to the value specified. Usually 8.
  * ```setHGap(value)``` setsthe horizontal gap between the components to the value specified. Usually 10.
  * ```TextFieldname.setPromptText(text)``` is same as ```placeholder``` attribute in HTML.
  * ```TextFieldname.getText()``` returns the data entered in the text field this could be used for sending the data into our DB or for Validations.
  * For Validation, create a private boolean function that checks for each required parameter. ie for each new requirement there would be a new function (like isInt()) that would have the Label as first parameter and the Text entered in the TextField as the second parameter. Inside the function check for the required details and return boolean value.
  ex - 
  ```
  private boolean checkLen(String content) {
        if(content.length() < 8) {
            System.out.println("Password should be greater than 7!");
            return false;
        }
        else {
            System.out.println("Login successful!");
            window.close();
            return true;
        }
    }
   ```
* __Data Structures__ *approx 25 mins*
 * Sorting algos: 
   * Bubble Sort: This algorithm is based on the idea of repeatedly comparing pairs of adjacent elements and then switching their positions if they exist in the wrong order. The complexity of bubble sort is O(n2) in the worst
   * Insertion Sort: The idea behind is that in each iteration, it consumes one element from the input elements, removes it and finds its correct position i.e., where it belongs in the sorted list and places it there. Complexity of Insertion sort is O(n2) .
   * Merge Sort: This sorting algorithm works on the following principle - Divide the array in two halves. Repeatedly sort each half, then merge two halves. complexity of this algorithm will be O( n( log2 n )).
   * Quick Sort: This algorithm is also based on the divide and conquer approach. It reduces the space complexity and removes the use of auxiliary array used in merge sort. The worst case time complexity of this algorithm is O( n2 )

#### Plan of action tomorrow / Thoughts:
* Javafx continued
* Data Structure Searching Algorithm revision
* *Keeping the list short as the college exams are approaching.

#### Link / Screenshots:
* Oracle Javafx Documentation: (https://docs.oracle.com/javase/8/javafx/get-started-tutorial/jfx-overview.htm#JFXST784)
* thenewboston Youtube Channel
* https://www.hackerearth.com/practice/notes/sorting-code-monk/
<img src = "http://g.recordit.co/vnqX2h4vUx.gif" width = 800 heigth = 500>

______________________________________________________________________________________________________________________________________

### __Day 19: DS Hashing and Javafx continued__
#### Sept 7, 2019 - Saturday

#### Progress: 
* Studied various layouts in Javafx (BorderPane, HBox, VBox)
* Embedding H and VBox into BorderPane layout
* In DS:
 * Revised Hashing (Methods, Collision Handling)
 * Introduction to Subset Sum using Backtracking

#### Summary:
* __Javefx__: *Approx 30 minutes*
 * BorderPane layout consists of various sections like top, left, right, centre, bottom. These can be specified during the creation of the components.
 * The ```VBox``` as the name suggests arranges the components in Vertical format. Whereas the ```HBox``` arranges in the horizontal format.
 * These layouts can be embedded together as follows:
   ```
   VBox vertical = new VBox();
   .
   .
   .
   BorderPane layout = new BorderPane();
   BorderPane.setLeft(vertical);
   ```

#### Plan of action tomorrow / Thoughts:
* Javafx - Form creation and validation
* Sorting techniques Revision
* TCC Week 6 problems

#### Link / Screenshots:
* Oracle Javafx Documentation: (https://docs.oracle.com/javase/8/javafx/get-started-tutorial/jfx-overview.htm#JFXST784)
* thenewboston Youtube Channel

_______________________________________________________________________________________________________________________________________

### __Day 18: FCC Applied visual Design (3/n) and Javafx continued__
#### Sept 6, 2019 - Friday

#### Progress: 
* Applied Visual Design - More on colour, gradient, transform property and Shapes
* Multiple window creation and interacting using javafx
* Closing a GUI window the right way

#### Summary:
* __FCC__ : *(Time spent: 51 minutes)*

  * ```hsl()``` stands for hue, saturation and lightness. Hue takes in angle in degree as its a colour wheel, Saturation stands for the amount for gray in the colour with 100% meaning no gray noise and 0% meaning total gray. Lightness is the amount of white or black shade the colour posses. A 100% lightness means full Full white and 0% as full black.
  * CSS gradients can be created using the ```linear-gradient``` property of the ```background``` atrribute. It takes in the below mentioned parameters :
 ```background: linear-gradient(angle, color1, color2,...)``` 
 The angle can be in deg where 90 deg means vertical gradient and 45deg means backslash gradient. colours could be rgb(), hsl() or the normal hex codes. 
 It could also be used to create strip patterns using ```repeating-linear-gradient()``` property which takes in angle and colour stops, For eg -
 ```background: repeating-linear-gradient(
        45deg,
        yellow 0px;
        blue 40px;
        green 40px;
        red 80px;
     )
 ```
   * The ```transform``` property:
 
   * ```scale(1.2)``` is used to enlarge the size of the object ot the desired times size as specified in the parameter passed to the scale function.
   * ```skewX(angle)``` and ```skewY(angle)``` functions are used to tilt the respective edges in the angle specified as the parameter.
  * Created a cardioide shape using the css ```::before``` and ```::after``` properties! Need to research on this topic a bit more so it'd be on my PoAT.
 
 * __Javafx__: 
 
   * Created multiple windows using a different class in java. Then passed the title and the message of the pop-up as parameter to the display method ofthe class. In the method created a total new window and added modality so as to give priority to the new window being opened. Below is the new class code.
   
   ```
   public class AlertBox {
    public static void display(String title, String message) {
        Stage window = new Stage();

        window.initModality(Modality.APPLICATION_MODAL);
        window.setMinWidth(250);
        window.setMinHeight(350);
        window.setTitle(title);

        Button btnClose = new Button("Close the window");
        btnClose.setOnAction(e -> window.close());

        Label label = new Label(message);

        VBox layout = new VBox();
        layout.getChildren().addAll(label, btnClose);
        layout.setAlignment(Pos.TOP_CENTER);

        Scene scene = new Scene(layout);
        window.setScene(scene);
        window.showAndWait();
    }
   }```
  
  * The interactivity can be added by returning a value from the method called and using that value obtained to do the required task. Here is a simple snippet of the code appended to the above one.
  ```
  Button yesBtn = new Button("Yes");
        Button noBtn = new Button("No");

        yesBtn.setOnAction(e -> {
            answer = true;
            window.close();
        });
   ```
   <img src="http://g.recordit.co/PWyVyiunoY.gif" width="700" height="350" />
  
  * Closing a program properly by using multiple windows concept and making sure the user wants to exit!

 
#### Plan of action tomorrow / Thoughts:
* Research on ```::before``` and ```::after``` CSS pseudo elements
* Revise the Udemy JS course current module. So as to not completely lose track of it.
* FCC AVD
* Javafx continued!

#### Link / Screenshots:
* Oracle Javafx Documentation: (https://docs.oracle.com/javase/8/javafx/get-started-tutorial/jfx-overview.htm#JFXST784)
* FreeCodeCamp: https://learn.freecodecamp.org
* thenewboston Youtube Channel

_______________________________________________________________________________________________________________________________________

### __Day 17: Intro to JavaFx__
#### Sept 5, 2019 - Thursday

#### Today's Project(s):
* Basic GUI using Javafx
* FCC AVD (2/n)

#### Progress: 
* Installed *IntelliJ IDEA Community Edition* IDE to work with Javafx
* Created a window with few buttons and implemented switching scenes.
* Applied Visual Design - positioning and color basics

#### Thoughts / Summary:
* Installation and configuration of the *IntelliJ IDEA Community Edition* was a breeze. This is mainly for the upcoming college project. For refernce i used the Oracle documentation on the javafx and the *newboston* channel on Youtube. Here are the list of things i was managed to build in this first day:
  * Create a window with a button on it - just a simple Stage with a button on its scene.
  ```
  public static void main(String[] args) throws Exception {
        launch(args);
    }

    @Override
    public void start(Stage primaryStage)
    {
      //What your window must contain
     }
  ```
  Basic terminologies: __Stage__ is the outer window of our GUI application. __Scene__ is the inner space where we would place our GUI components. __Layout__ is used to give desired position to our components. The 2 types of layouts tested today were the StackPane layout and the VBox layout! More on this next time.
  * Handle the event of *click* - In the first attempt used a event Handler but not as a Lambda expression but by pointing it to a method in class, which in my case was the method in ```Main``` class.
  * Using the Lambda expression to clean the code to some extent - This part was very similar to the Javascript concept of callback functions and the arrow notation in the ES6. 
  ```
  btn1.setOnAction(event -> System.out.println("button click"));
  ```
  Here the ```event``` parameter recognizes that the code following it needs be executed in case the event happens, in short, no need of calling a new Event Handler class. Also its has a benefit that the event always knows whats the source of the Event and  we dont need to specially code for it. (done using the event.```getSource()``` method.
  * Switching scenes using buttons - Just created 2 scenes and on button press set the current scene of window to the desired scene! Worked fine.
  ```
    btn1.setOnAction(event -> window.setScene(scene2));
    btn2.setOnAction(event -> window.setScene(scene1));
  ```
 * __FCC__ : Brief summary:
   * ```float```: left/ right . Mostly used with the width attribute
   * ```z-value```: specifies value in the stack. Higher the value the above it would be on the elements with lower values.
   * ```margin: auto``` to centre the block or the element
   * Colour Theory
 
#### Plan of action tomorrow:
* Continue with the Javafx tutorials and maybe think of some ideas for the project.
* Continue on the FCC AVD
* Research on RGB model for Computers and CYM(K) for printing

#### Link / Screenshots:
* Oracle Javafx Documentation: (https://docs.oracle.com/javase/8/javafx/get-started-tutorial/jfx-overview.htm#JFXST784)
* FreeCodeCamp: https://learn.freecodecamp.org
* thenewboston Youtube Channel

<img src="http://g.recordit.co/lNI30UMWCG.gif" width="800" height="500" />

_______________________________________________________________________________________________________________________________________

### __Day 16: The Deluge__
#### Sept 4, 2019 - Wednesday

#### Today's Project(s):
None

#### Progress: 
None

#### Thoughts:
* Repeat of July 10, 2018 Deluge in Mumbai and MMR. Freak 500mm rainfall in little more than 36 hrs where I stay. It resulted in the whole of the city getting submerged which resulted in 15 hour power cut. So all i could manage to do was study for my college tests.

#### Plan of action tomorrow:
* Start learning JavaFx for one of college projects and try to complete the FCC AVD.

#### Link / Screenshots:

_______________________________________________________________________________________________________________________________________

### __Day 15: FCC Applied Visual Design (1/n)__
#### Sept 3, 2019 - Tuesday

#### Today's Project(s):
* FCC - Applied Visual Design in Responsive Weeb Design

#### Progress: 
* Studied various text-align properties
* box-shadow, opacity, text-transform was used and studied.
* position attricute was analysed

#### Thoughts:
* One of my goals to complete the responsive web designs. I feel it is the best time to complete these fun FCC exercises during the hectic exam week. Might be the norm for the whole week!

#### Plan of action tomorrow:
* Continue with the FCC on AVD.

#### Link / Screenshots:

_______________________________________________________________________________________________________________________________________

### __Day 14: Competitive Coding and Data Strucutre - continued__
#### Sept 2, 2019 - Monday

#### Today's Project(s):
* Continued with my study of DS

#### Progress: 
* Studied the searching algorithms - Linear, Binary
* Sorting algorithms - Insertion, Quick, Merge, Bubble
* Tried solving the remaining 2 CP problems

#### Thoughts:
Mostly academic related stuffs today and again not much JS. However, still a lot of learning!

#### Plan of action tomorrow:
* Continue with the Data Structure and the one remaining problem of the TCC Problem.

#### Link / Screenshots:

_______________________________________________________________________________________________________________________________________

### __Day 13: Competitive Coding and Data Strucutre__
#### Sept 1, 2019 - Sunday

#### Today's Project(s):
* Try to complete the TSEC CodeCell (lets call it TCC) saturday problems

#### Progress: 
* Solved 2 Competitive coding problems
* Studied the Queues Data Structure and its types
* Solved the hour glass DS problem on HackerRank

#### Thoughts:
No JS for today. Studied the Data Structure concept as it'd help cater both the Academic requirements as well as with the competitive coding. 

#### Plan of action tomorrow:
* Continue with the Data Structure and the one remaining problem of the TCC Problem.

#### Link / Screenshots:
---
_______________________________________________________________________________________________________________________________________

### __Day 12: Form Validation__
#### Aug 31, 2019 - Saturday

#### Today's Project(s):
* Building a basic Sign Up page with Form Validations included

#### Progress: 
* Revised on some CSS concepts and ideas
* Created a signup page
* Implemented JS Form Validators
* Solved 2 Competitive coding problems

#### Thoughts:
The form validations done by me were pretty basic but served the purpose of learning and understanding how it functions. Maybe in the fututre project would apply it in a more industry - specific manner.

#### Plan of action tomorrow:
* Since College Internal tests are fast approaching would like to keep it simple and restart doing the FCC 'Responsive Web Designs' Certification course!

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1167860590179577856

_______________________________________________________________________________________________________________________________________

### __Day 11: Installing Babel__
#### Aug 30, 2019 - Friday [Missed 2 days due to legit reasons related to College and academics]

#### Today's Project(s):
* Udemy's JS course continuation.

#### Progress: 
* Installing babel-core, babel-preset-env and babel-loader
* Setup the babel config file '.babelrc'
* Installing babel-polyfill as dependency
* Successfully converted ES6 version of a js code to ES5!

#### Thoughts:
Lots of installations using the ```npm install```. Got to know that Babel helps to convert the JS file from one ES module to ES5 However yet doesnt really know where the real application of it lies. Hopefully will find out by the end of this course!

#### Plan of action tomorrow:
* Learn about form validations and build a simple Login / SignUp Page

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1167499905289641985

_______________________________________________________________________________________________________________________________________

### __Day 10: Running a webpack dev server__
#### Aug 27, 2019 - Tuesday

#### Today's Project(s):
* Udemy's JS course continuation.
* Data structure study on Linked List.

#### Progress: 
* Installing and running file on webpack-dev-server
* Difference between opening an html file using browser vs Running it using server
* Installed webpack-html-plugins
* Learnt the Linked List DS

#### Thoughts:
It has started to make sense now on why do we need all these packages for the web development perspective. Still i need to get better at the Webpack CLI. Studied the data structure of Linked List.

#### Plan of action tomorrow:
* Continue with the Udemy's Javascript course. Babel up next!

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1166411887421972480

_______________________________________________________________________________________________________________________________________

### __Day 9: NodeJS and webpack intro__
#### Aug 26, 2019 - Monday

#### Today's Project(s):
* Udemy's JS course continuation. 

#### Progress: 
* Installing Nodejs, webpack
* Configuring the webpack
* Created a simple js file to export default value and logged it to console by importing it

#### Thoughts:
Today, the learning curve was pretty steep. Instllations were quite smooth but setting up the configuration file and the json file was new to me and had me pretty confused.

#### Plan of action tomorrow:
* Continue with the Udemy's Javascript course. We are moving right into the main stuff!

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1166050520219279361

_______________________________________________________________________________________________________________________________________

### __Day 8: Modern Javascript__
#### Aug 25, 2019 - Sunday

#### Today's Project(s):
* Brief overview about Modern Javascript packages and tools
* TSEC CodeCell Problems

#### Progress: 
* Overview of modern javascript
* Npm packages and tools used
* Basic Command Line operations
* Solved couple of CP problems

#### Thoughts:
Its Sunday so tried solving the coding problems on the TSEC CodeCell Website, a platform for solving CP problems built by our other undergraduate students of our college.

#### Plan of action tomorrow:
* Continue with the Udemy's Javascript course. We are moving right into the main stuff!

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1165682810406891521

_______________________________________________________________________________________________________________________________________

### __Day 7: Project using CSS Variable__ 
#### Aug 24, 2019 - Saturday

#### Today's Project(s):
* Building a mini project that uses CSS Variables concept

#### Progress: 
* declaring CSS variables
* ```data``` attribute in html
* Changing the property of the variables

#### Thoughts:
The concept of CSS variables is so powerful and useful tool that can help build so many tools for the user! Would surely be interested in using these in some future projects!

#### Plan of action tomorrow:
* Continue with the Udemy's Javascript course.

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1165321868624064513

_______________________________________________________________________________________________________________________________________

### __Day 6: A sluggish day__ 
#### Aug 23, 2019 - Friday

#### Today's Project(s):
* Module 9 intro to the last big project in the course.
* HackerRank problems

#### Progress: 
* Started with the last big project in Jonas' JS Course
* Attempted a couple of HackerRank problems
* Browsing random inbuilt functions in Python
* 10 min meditation !

#### Thoughts:
Was tired after a long and tiring day. The big project 'forkify' looks interesting. Hackerrank problems were quite fun and challenging at the same time. The 10 minutes of meditation really helped to continue with the rest of the day.

#### Plan of action tomorrow:
* Next project in the Javascript30 on CSS variables. Had done them in the FCC CSS part but no harm in going over them again.

#### Link / Screenshots:
---
_______________________________________________________________________________________________________________________________________

### __Day 5: AJAX / API__ 
#### Aug 22, 2019 - Thursday

### Today's Project(s):
* ES6 Module of Udemy JS course.
* Covered portion of AJAX and API

##### Progress: 
* Basic idea about AJAX and API.
* Fetching data from an API
* Using CORS in fetching
* Debugging your code 😂

#### Thoughts:
Really excited to learn more about the API and experiment myself!

#### Plan of action tomorrow:
* Continue with the course and move into the next module of the Udemy JS course and build the last BIG project using Asynchronous JS concepts!

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1164586622005981185

_______________________________________________________________________________________________________________________________________

### __Day 4: JS Clock__ 
#### Aug 21, 2019 - Wednesday

#### Today's Project(s):
* Javascript30 second project - building the clock

#### Progress: 
* CSS transform, transform-origin, transition function, cubic bezier curve.
* Revision of DOM manipulation concepts.
* Brief reading on asynchronous javascript from mdn site.

#### Thoughts:
Lots to learn and a fun day(as it always is while building new stuff). Reading on Asynchronous javascript was somewhat overwhelming.

#### Plan of action tomorrow:
* Switch back to the udemy's JS course. AJAX and API intro coming up!

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1164211064910823428

_______________________________________________________________________________________________________________________________________

### __Day 3: CallBacks__ 
#### Aug 20, 2019 - Tuesday

#### Today's Project(s):
* Learnt about Callback, promises in traditional Async JS

#### Progress: 
* Callback Hell in traditional Async JavaScript
* Producing Promises
* Async/Await in Promises(clearly easier way to consume promises)

#### Thoughts:
A pretty good day. Learnt quite a few new concepts.

#### Plan of action tomorrow:
* Switch back to JS30 and build a clock!

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1163819047483396101

_______________________________________________________________________________________________________________________________________

### __Day 2: The DrumKit__
#### Aug 19, 2019 - Monday

#### Today's Project(s):
* Javascript30 'Drum Kit'

#### Progress: 
* Refreshed on few CSS and JS concepts.
* Why doesnt the ```this.classList``` contain the ```playing``` class?

#### Thoughts:
Felt good building something (trash but fun nevertheless). At the end though it was quite exhausting after the console log kept logging unexpected stuff. Did the research but still couldn't figure it out why it happened. (Check the links to find out more)

#### Plan of action tomorrow:
* Work on the Udemy course. Things are getting serious in there!

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1163464444514582534

_______________________________________________________________________________________________________________________________________

### __Day 1.Round 1 Begins!__
#### Aug 18, 2019 - Sunday

#### Today's Project(s):
* Udemy course module on Asynchronous Javascript

#### Progress: 
* Understood what asynchronous javascript means.
* Difference between Asynchronous and Synchronous JS
* How Asynchronous JS works behind the scenes.

#### Thoughts:
Having been doing the Udemy course before starting this challenge, I hope to be more consistent in doing the course works and document everything better. Regarding today's work I was pretty pleased with the code written and had not much to worry or do extra research about since no errors bothered me today. 

#### Plan of action tomorrow:
* Start with #Javascript30 as everyday of the same course would be monotonous.

#### Link / Screenshots:
https://twitter.com/MindianApe/status/1163131126732300288
