1. Forgot to add a semicolon after the name
   Main.java:4: error: ';' expected
   String name = "Said"
   ^
   1 error
   Since Java requires every statement to conclude with a semicolon, stopping at line 4 without one left the compiler completely confused about where the command actually finished.
2. Tried to use a variable without assigning a value first (int a; instead of int a = 12;)
   Main.java:9: error: variable a might not have been initialized
   System.out.println("a + b = " + (a + b));
   ^
   1 error
   Even though I created the variable a, I forgot to actually store a number inside it, and Java simply won't let me do math with an empty variable.
3. Attempted to save text inside an int (int b = "thirty";)
   Main.java:6: error: incompatible types: String cannot be converted to int
   int b = "thirty";
   ^
   1 error
   Because I set up b as an int, it is strictly reserved for numbers; wrapping the word "thirty" in quotes makes it a String, and Java refuses to magically convert that text into a number for me.