# The input() function

Notes:
- The input() function waits for interaction from the command line (stdin)
- It will **ALWAYS** read whatever is put on the command line as a string type

## Use Input to Wait

This example will just wait around for user input.

`vim ex_input_01.py`

```python
wait = input()
print("done")
```

`python3 ex_input_01.py`

> After you run this, you should see that the program "does nothing". It just waits and waits.

**PRESS ENTER**

And then it will print "done".

## Use Input to Gather Information

More often than just waiting around, you will use input to gather information from a user.

> Note that we are able to have an optional **prompt** put inside the () of the input function. This will be printed to the screen and then wait for the user to put information on the CLI.
 
`vim ex_input_02.py`

```python
myvar = input("What is your favorite color? ")
print(f"You said your favorite color is {myvar}")
```

`python3 ex_input_02.py`

```
What is your favorite color? 
```

> Type a color on the command line, and then press **ENTER**

An example output might be:

```
What is your favorite color? macaroni-yellow
You said your favorite color is macaroni-yellow
```

