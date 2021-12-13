# Understanding the Shebang Line

Notes:
- **Sh** comes from the **#** (ha**sh**) sign
- **bang** comes from the **!** (**bang**) sign
- **Shebang lines only matter in linux**, but are considered best practice for python code

If you want to run a script in linux with the syntax of `./myscript.sh` or `./myotherscript.py`, you will want to use a shebang line.

That is because when you try to run a script with that syntax, you will be asking the shell (**bash**) to run the script.

So when you run:

`./mypyscript.py`

Bash will read the first line of the script. If it is a shebang line, bash will read what program should be executing the rest of this script.

Otherwise, Bash will be the program executing the script. No bueno for scripts written for python to run.

So either, run your script with python directly:

`python3 myscript.py`

OR put a shebang line as the first line of your script.

`cat myscript.py`

```python
#!/usr/bin/env python3
print("It worked!")
```

Also, your script must be **executable** in order to use the "dot-slash" syntax.

`chmod u+x myscript.py`

**NOW you can safely run your script:**

`./myscript.py`

```
It worked!
```




