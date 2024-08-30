Step 0- I created the repository and included the header files in the main.cpp file.
From what I learned, this file generates macro code and converts some symbolic code.

Step 1- The g++ command compiles c++ source code files. I used the g++ -E command to 
only perform the preprocessing step which handled the #include at the head of 
the file. This code was directed into the main.i file.

Step 2- The g++ -S command processes the code to the assembly stage. This output
was directed into the main.s file and is in assembly code.

Step 3- By using the g++ -c command on the main.s file, the code in the file
was now compiled into an object file but not an executable file. This code is no
longer human readable.

Step 4- Finally, I used the g++ -o command to links the object file to 
necessary libraries and creates an executable file. In this case, it was a.out.

Step 5- I used ./a.out to run the file in my terminal and to my surprise
it produced "Hello World".
