# Understanding Computer Data Storage - Bits & Bytes

## Bit
A bit is the smallest storage possible in computers that can have two possible states, 'ON' or 'OFF';
Puting this in computer terms, these states can either be '1' or '0'.

## Byte
A byte is a combination of 8 bits. The number value each of the bit in a byte can hold grows from right to left.

0, 0, 0, 0, 0, 0, 0 ,0 => 128, 64, 32, 16, 8, 4, 2, 1 

The possible number hole we can represent using a single byte is 255. To get a number greater than 255, we can combine bytes.

## Signed Numbers Representation
We can achieve the representation of a signed number by sacrificing the leftmoset numberhole in a byte.

Example: To reprsent -35, we can achieve this by following these steps.

- Step 1:
Get the binary representation of 35
00100011 = 35

- Step 2:
Take the complement by making everything that was zero become 1 and everything that was 1 become 0
11011100 = 35 1's complement

- Step 3:
Take the second complement by adding 1 to the value in step 2
11011101 = 35 2's complement

therefore, -35 = 11011101

## Representing Characters
Since we already know how to store numbers, we can store strings or characters by storing many numbers.
For this, an ASCII table was the first table defined to help us achieve this.
The ASCII table can only take one byte and for this reason, it has a size limitation as it can only take upto 128 characters.

To solve the size limitation issue the ASCII table has, the UNICODE table was developed.

with the UNICODE table, we get to decide the number of bytes required to represent whatever character we need. This table
can hold tens of thousands of characters. All of the world's languages and other symbols are included and represented in 
this table.

## Reference
[Link](https://www.youtube.com/watch?v=01jkT5nSgRc)
