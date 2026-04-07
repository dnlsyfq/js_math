```
parseInt(readLine(),10) 
```

Decimal / Float
```
floatVar.toFixed(int) // set decimal places , return string 
```
Convert string to No.
```
Number(floatVar.toFixed(2)) // convert string to no.
```


```
Math.random() // Random no. between 0 and 1
Math.random() * 50 // Random no. between 0 and 50
Math.round(floatVar)
Math.floor(float)
Math.ceil(float)
isNaN(var) // check whether a value is NaN , not a number
```

```
if( isNaN(var) || isNaN(var) ){
  throw Error('Both arguments must be numbers.')
}
```


```
Number.isInteger(value)
```

```
5**3 // exponent
100 % 3 // remainder
```

```
let attempts = 10;
attempts--;
attempts++;
```

```
let x = 5;
console.log(x++); // 5
console.log(x); // 6

let x = 5;
console.log(++x);//6
```


```

function calculateSubtotal(price, quantity) {
    if (price < 0 || quantity < 1) {
        return "Invalid price or quantity";
    }
    return price * quantity;
}
function calculateShipping(subtotal, international = false) {
    if (international) {
        return subtotal > 100 ? 15 : 25;
    }
    return subtotal > 50 ? 0 : 10;
}
function calculateTotal(price, quantity, international = false) {
    let subtotal = calculateSubtotal(price, quantity);
    let shipping = calculateShipping(subtotal, international);
    let total = subtotal + shipping;
    
    console.log("Subtotal: $" + subtotal);
    console.log("Shipping: $" + shipping);
    console.log("Total: $" + total);
}
// Test orders
calculateTotal(25, 2);           // Domestic order
calculateTotal(25, 2, true);     // International order

```
