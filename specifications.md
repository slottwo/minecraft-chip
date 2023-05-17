# Architecture 8-bits

## Instruction set

> Instruction name: `syntax` <=> 0000 0000

0. Interact with memory: 000o xxxi

   | bits | value | info         |
   | ---- | ----- | ------------ |
   | 3b   | 000   | instruction  |
   | 1b   | 0/1   | if lw or sw  |
   | 3b   | xxx   | reg dest id  |
   | 1b   | 0/1   | if immediate |

   1. Load from mem to reg:

      `lw $reg immediate|0` <=> `0000 xxxi (IIIIIIII)`

   2. Save in mem from reg:

      `sw $reg immediate|0` <=> `0001 xxxi (IIIIIIII)`

1. Jumping:

   0. Jump to immediate address:

      `j immediate` <=> `0010 0 001 IIIIIIII`

   1. Jump to address on register:

      `jr $reg` <=> `0010 1 xxx`

   2. Branch to immediate address if register equals zero

      `beq $reg` <=> `0011 0 xxx IIIIIIII`

   3. Branch if ...

      ...

2. .
   
3. .

4. .

5. .

6. .

7. .

> Required functionalities:
>
> > Load and Save from memory
>
> > Branch If
>
> > Jump
>
> > Set less then

## Registers

0. `000` |
1. `001` |
2. `010` |
3. `011` |
4. `100` |
5. `110` |
6. `101` |
7. `111` |

# Architecture 16-bits