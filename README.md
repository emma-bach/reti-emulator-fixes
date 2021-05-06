# ReTI emulator

Quickly test your ReTI instructions using this emulator.
The only dependency is the Python interpreter.

## Quick start
Simply run the `reti.py` file using Python, passing the path to your instructions as the first argument.
```
python3 reti.py <PATH TO INSTRUCTIONS>
```

Pass `verbose` as a second argument to see all instructions as they get executed.

```
python3 reti.py <PATH TO INSTRUCTIONS> verbose
```

## Available Instructions
All lines starting with `#` are treated as comments and will be ignored.

```
LOAD i
LOADI i
STORE i
ADD i
SUB i
ADDI i
SUBI i
LOADIN j i
STOREIN j i
MOVE s d
JUMP i
JUMPC c i
PRINT i
```

**Notes:**  
- `LOADIN` and `STOREIN` are used as follows: `LOADIN ACC IN1`
- `JUMPC c i` is defined slightly different than in the lecture. Simply pass the conditional as the first argument c.
- `PRINT i` is not defined in the lecture. It can be used to print the value of S[i] from memory to the console.

## Examples / Contributing
The `examples` directory contains a few sample ReTI scripts.  
You are welcome to submit a pull request, adding additional examples or simply improving the code in general.

## Credits
Inspired by Vorlesung Technische Informatik, SoSe 21  
Prof. Dr. Christoph Scholl, Universität Freiburg