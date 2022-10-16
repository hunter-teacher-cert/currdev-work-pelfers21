## Assignment
* title: **04_langauge.md**
  * Select one of the languages that were discussed in the breakout rooms that you feel would be a good fit for a course that you currently teach or would like to teach. (If it is reasonable, pick a language other than one you currently teach.)
  * Answer the following prompts:
    - What is the course? (grade level, student experience)
    - What is the language?
    - How does one write & run code in this language?
    - Rate the complexity of the syntax?
    - Strengths
    - How would you utlilize the strengths in the class?
    - Weaknesses
    - How would you mitigate the weaknesses in the class?
    - Why did you select this language for this class?


    ## Processing
    
    Processing would be a good fit for adding to my P5 course.  8th graders are learning web design currently and will be learning P5 to add to the curriculum.
    I'd like to teach some Processing with P5 to demonstrate the similarities in the languages.  The students will be adding some of the Processing projects to 
    their web pages that they are creating in P5 and this will give them experience with both languages.  Both languages are involved with creating visual 
    arts and much more.  In Processing, the syntax is fairly similar, if not, 
    mostly interchangeable, that the students should be able to master the syntax fairly readily.  The students will compare the differences of the languages
    to be able to switch between the two and this will help with any issues that they are having trouble with.  There is a reference page in P5 that will help 
    with general coding and http://Processing.org itself has a library that can be used for help as well.
    
    One huge benefit to processing is the ability to download the program to the computer and be able to still have access to programming if the Internet 
    is not accessible.  One of the major differences in the program is that it uses "void" instead of "function".  Most of the other characters used are the 
    same including the syntax.  Both need to be "set up" and "draw" to start the programs.  This is where they create the canvas and decide what they will 
    draw.  Other functions can be created with variables, conditionals, loops, etc as well.  The language is fairly straight forward and will enable to students
    to get a good understanding of text-based language to ready them for high school.
    
    Here's how an example looks in Processing vs P5:
    
    Processing:
    /**
 * Hue. 
 * 
 * Hue is the color reflected from or transmitted through an object 
 * and is typically referred to as the name of the color such as 
 * red, blue, or yellow. In this example, move the cursor vertically 
 * over each bar to alter its hue. 
 */
 
int barWidth = 20;
int lastBar = -1;

void setup() {
  size(640, 360);
  colorMode(HSB, height, height, height);  
  noStroke();
  background(0);
}

void draw() {
  int whichBar = mouseX / barWidth;
  if (whichBar != lastBar) {
    int barX = whichBar * barWidth;
    fill(mouseY, height, height);
    rect(barX, 0, barWidth, height);
    lastBar = whichBar;
  }
}

    
    See below for a slight difference in creating the same drawing:
    
    P5
    
    barWidth = 20;
    lastBar = -1;

function setup() {
  createCanvas(640, 360);
  colorMode(HSB, height, height, height);  
  noStroke();
  background(0);
}

function draw() {
   whichBar = mouseX / barWidth;
  if (whichBar != lastBar) {
    barX = whichBar * barWidth;
    fill(mouseY, height, height);
    rect(barX, 0, barWidth, height);
    lastBar = whichBar;
  }
}
    
    
