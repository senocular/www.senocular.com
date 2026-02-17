## What's new

### Updates

It's alive! The site is being revived and will start seeing new content again! This will likely consist of JavaScript examples and learning material, starting off with the articles available on https://senocular.github.io.

This will be an ongoing process that will take a while to complete. Thank you for your patience.

Here is some random code:

```js
function updateName() {
    const name = prompt("Enter a new name");
    button.textContent = `Player 1: ${name}`;
}

const button = document.querySelector("button");
button.addEventListener("click", updateName);

const numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9];

// Get the squares of all even numbers
const squaresOfEvenNumbers = numbers.filter((ele) => ele % 2 == 0).map((ele) => ele ** 2);

console.log(squaresOfEvenNumbers); // [0, 4, 16, 36, 64]
```

### Archive

The old blog archive has moved. It is now available [here](/archive).
