# Dart OOP Assignment: Kigali Bus Card

**Name:** Mohamed Hamedalnel
**Student ID:** 26857

## My numbers
- D = 57
- L = 7
- Starting balance = 1570 RWF
- Bus fare = 257 RWF
- Student discount = 17%

## Part 1: Why no setter for balance?

Because it protects the balance. The user cannot change it directly. The balance can only change using topUp() or pay().



## Part 2: What does ~/ do?

The / operator gives the normal division result.
The ~/ operator gives an integer result and removes the decimal part.

237 * 17 / 100 = 40.29
237 * 17 ~/ 100 = 40

## Output of main.dart

```text
Error: name too short
Owner: Mohamed | Balance: 1570 RWF
Owner: Mohamed Hamedalnel | Balance: 1570 RWF
Error: top-up must be 500 to 50000 RWF
Topped up 2000 RWF
Paid 257 RWF
Paid 257 RWF
Owner: Mohamed Hamedalnel | Balance: 3056 RWF
Student discount: 43 RWF
Paid 214 RWF
Owner: Mohamed Hamedalnel | Balance: 1356 RWF
Student card: 17% off
```
