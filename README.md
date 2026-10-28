# vibe

A programming language where the only token is the word `vibe`.

You don't need the exact number of vibes. Just roughly right.

## the eleven instructions

| vibes | instruction | notes |
|-------|-------------|-------|
| 1 | PUSH | next line's count is the value (exact) |
| 2-3 | POP | |
| 4-6 | ADD | |
| 7-10 | SUB | |
| 11-16 | DUP | |
| 17-24 | EMIT | ASCII character |
| 25-35 | PRINT | number |
| 36-44 | SWAP | |
| 45-55 | JZ | jump if zero (next line = target, exact) |
| 56-70 | JNZ | jump if not zero (next line = target, exact) |
| 71+ | HALT | |

The more consequential the operation, the more vibes it takes.
And the more vibes it takes, the more room you have to be sloppy.

Values after PUSH are exact. Jump targets are exact. Everything else is a vibe.

Zero-vibe lines are comments. Write whatever you want. The English is for you. The vibes are for the computer. Neither needs to understand the other.

**Warning:** the word `vibe` in a comment counts as a vibe. The language's own name is a live token.

## example

```
the simplest possible program
three plus four

vibe
vibe vibe vibe
push three

vibe
vibe vibe vibe vibe
push four

vibe vibe vibe vibe vibe
add them together

vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe
print

vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe vibe
halt
```

Output: `7`

## build and run

```
cc -std=c99 -o vibe vibe.c
./vibe examples/add.vibe
./vibe examples/countdown.vibe
./vibe                          # REPL
```

## tools

- `gen.c` -- generate `.vibe` files from strings: `./gen "hello" > hello.vibe`
- `dbg.c` -- disassemble `.vibe` files: `./dbg program.vibe`

## try it in the browser

Open `docs/index.html`. The interpreter runs client-side in JavaScript. Turn on sound and every EMIT becomes a note on a pentatonic scale.

## why

> "I said, 'dinosaurs look sad,' you said, 'just stop thinking'"
>
> -- Hollerado

---

by [bonchicbongenre](https://github.com/bonchicbongenre)
