# 1. leap_year

This short and simple Kata should be performed in pairs using Test Driven Development (TDD).

Acceptance Criteria:

1. All years divisible by 400 ARE leap years (so, for example, 2000 was indeed a leap year),
2. All years divisible by 100 but not by 400 are NOT leap years (so, for example, 1700, 1800, and 1900 were NOT leap years, NOR will 2100 be a leap year),
3. All years divisible by 4 but not by 100 ARE leap years (e.g., 2008, 2012, 2016),
4. All years not divisible by 4 are NOT leap years (e.g. 2017, 2018, 2019).


# 2. Cupcake 

Write a program that can build many cakes with many toppings like : "🧁 with 🍫 and 🥜 and 🍓". Each cake is composed of a base cake and zero or more toppings (order matters). Using the same topping multiple times is not allowed, any topping occurring more than once is silently ignored except its first instance.

The different bases are:
* Cupcake (Text is "🧁", price is 1.00€)
* Shortcake (Text is "🍰", price is 2.00€)

The toppings are:
* Chocolate (Text is "🍫", price is 0.10€)
* Nuts (Text is "🥜", price is 0.20€)
* Strawberry (Text is "🍓", price is 0.15€)

Write a function that returns the name of cake and a function that returns the price of cake. The price is composed of the base cake price and topping prices.

### Example in pseudocode

```
var myCake = Strawberry(Nuts(Chocolate(Cupcake())))
myCake.name() // returns "🧁 with 🍫 and 🥜 and 🍓"
myCake.price() // returns 1.45
```

### Possible test cases for the name function

    The name function should return "🧁"
    The name function should return "🍰"
    The name function should return "🧁 with 🍫"
    The name function should return "🍰 with 🍫"
    The name function should return "🍰 with 🍫 and 🥜"
    The name function should return "🍰 with 🥜 and 🍫"

### Possible test cases for the price function

    The price function should return 1€ for "🧁"
    The price function should return 2€ for "🍰"
    The price function should return 1.1€ for "🧁 with 🍫"
    The price function should return 2.1€ for "🍰 with 🍫"
    The price function should return 2.2€ for "🍰 with 🥜"
