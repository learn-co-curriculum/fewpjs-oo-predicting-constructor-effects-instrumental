# Predicting Constructor Effects

## Questions

```js
class Rectangle {
  constructor(sideA, sideB) {
    this.sideA = sideA;
    this.sideB = sideB;
    this.area = sideA * sideB;
    this.perimeter = sideA * 2 + sideB * 2;
  }
}
```

1.  Given the example `class` above, what will all four properties be
    if `let rectangle = new Rectangle(2,4)` is run?

2.  What if `let rectangle = new Rectangle(10,-4)` is run?

```js
class Book {
  constructor(title, author) {
    this.title = this.titleize(title);
    this.author = this.titleize(author);
  }

  titleize(string) {
    let words = string.split(' ');
    for (let n = 0; n < words.length; n++) {
      words[n] = words[n].charAt(0).toUpperCase() + words[n].slice(1);
    }
    return words.join(' ');
  }
}
```

3.  What would the resulting instance look like if we ran
    `new Book("Shawshank Redemption", "Stephen King")`?

4.  What about `new Book("all the pretty horses", "cormac mccarthy")`?

```js
class Transaction {}
```

5.  What would happen if
    `let transactions = new Transaction(14.50, new Date(), "Subway tickets")` was run?
