# 📌 What is Python?
Python is formally **interpreted** language.

An interpreted language is a programming language where the code is executed line-by-line by another program called an **interpreter**, instead of being compiled all at once into machine code.

Imagine you’re giving a speech in English to an audience that only understands Japanese.

You have a live translator standing next to you.

- You speak one sentence

- The translator immediately translates it

- The audience acts on it

- Then you speak the next sentence

That’s an interpreted language. Thats how Python work

Now imagine you write the entire speech, hand it to a professional translator before the event, and they translate the whole thing into Japanese.

- Errors are found before the speech

- Once translated, you can speak very fast

- No translator needed during the event

That’s a compiled language.

Your computer cannot understand Python, JavaScript, or any human-readable code directly.It only understands machine language (0s and 1s).

👉 When you write code, some other program must read your code and talk to the computer on your behalf.

That “other program” is the interpreter.  

You write this Python code:
```python
print("Hello")
```
What actually happens:

1) You double-click / run the Python file

2) The Python interpreter starts running (this is a real program installed on your PC)

3) The interpreter:
 
  - Reads print("Hello")

  - Understands what print means

  - Converts it into machine instructions

  - Tells the CPU: “Display Hello on the screen”

So:

Your code is NOT executed directly

The interpreter executes it for you

## Where is the interpreter?
Python → python.exe
If you uninstall Python, your Python code won’t run — because the interpreter is gone.

While the interpreter can be used interactively, a programmer defines a series of commands in advance and saves their commands in a plain text known as **source code** or a **script**. For python, source code is stored in a file named with **.py** suffix

On the most operating systems, the python interpreter can be started by typing *python* in the command line.

Commands from a predefined script saved in a file(e.g., demo.py) are executed by invoking the interpreter with the filename as an argument (e.g., python demo.py) or using an additional -i flag in order to execute the script and then enter interactive mode (e.g., python -i demo.py)


### What python.exe actually is?
python.exe is a normal program installed on your computer, just like:

-Chrome.exe

-notepad.exe

-vscode.exe

But its job is special:

Its job is to read .py files and execute them.

So:

Your .py file ❌ is not a program

python.exe ✅ is the program

### What happens when you run a Python file?
When you type:
```python
print('Hello')
```
Here’s the real chain of events:

1) Windows runs python.exe

2) python.exe opens hello.py as a text file

3) It reads your code line by line

4) Converts each instruction into machine-level operations

5) CPU executes those operations

So technically:

You are not running hello.py ❌

You are running python.exe, passing hello.py as input ✅

## How compiled languages avoid this?

Compiled languages avoid an interpreter at runtime by converting your code into a native machine-code program before you run it.

1) You write code (human-readable)
  ```c
  #include <stdio.h>

int main() {
    printf("Hello\n");
    return 0;
}
```
2) You compile it

You run:
```nginx
gcc hello.c
```
What happens:

- The compiler reads your entire code

- Checks syntax & types

- Translates EVERYTHING into machine code

- Creates an executable file (e.g. a.exe or a.out)

📦 Output: a binary file full of 0s and 1s

3) You run the program
  ```bash
  ./a.exe
  ```
Now:

The CPU runs the machine code directly

❌ No interpreter

❌ No line-by-line translation

That’s how compiled languages “avoid this”.
