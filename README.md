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
## Part 4: Bug table


| Bug | The line | Why it is wrong | My fix |
|---|---|---|---|
| 1 | String _brand; and int _battery; | They have no starting values. | Add empty string and zero. |
| 2 | SmartPhone(String brand, int battery, String system) | It does not call the parent constructor. | Add super(brand, battery). |
| 3 | @override void restart() | The parent class has no restart method. | Add restart() in Phone. |
| 4 | Missing battery setter in Phone | We cannot change battery without a setter. | Add a setter from 0 to 100. |
| 5 | print(p.battery()); | Getter is not a method. | Remove the parentheses. |


### Not a bug

Phone p = new Phone('Tecno', 50);

The new keyword is allowed in Dart. It creates an object.

### Fixed output

100


## Part 5

My prediction:

The output will be:

1
5

Why?

For Bag, add() increases items to 1.
The value -5 is rejected because it is negative.

For BigBag, each add() increases items by 2.
After two calls, items becomes 4. Then we add 1, so the result is 5.
