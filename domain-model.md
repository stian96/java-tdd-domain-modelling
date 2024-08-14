# Domain model for supermarket shopper

User story:
```
As a supermarket shopper,
So that I can pay for products at checkout,
I'd like to be able to know the total cost of items in my basket.
```

Potential domain model design for the user story above:

| Classes         | Members            | Methods                         | Returns |
|-----------------|--------------------|---------------------------------|---------|
| `Shopper`       | `List<Item> items` | `getTotalCost(List<Item> items)`| `Double`|
| `Item`          | `Integer price`    |                                 |         |

## Domain model for receipt

We can use then previous model and add an extra receipt class and some members.

| Classes         | Members            | Methods                         | Returns |
|-----------------|--------------------|---------------------------------|---------|
| `Shopper`       | `List<Item> items` | `getTotalCost(List<Item> items)`| `Double`|
|                 |                    |                                 |         |
| `Item`          | `Integer price`    |                                 |         |
|                 | `String name`      |                                 |         |
|                 | `Integer quantity` |                                 |         |
|                 |                    |                                 |         |
| `Receipt`       | `Shopper shopper`  | `printReceipt()`                | `void`  |
|                 | `Double totalCost` |                                 |         |



