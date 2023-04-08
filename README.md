# Array Cardio 🏁

This project demonstrates the use of built-in JavaScript Array methods to manipulate arrays of objects. The code is contained within an HTML file that includes a JavaScript code block.

## Data

The code defines two arrays of objects:

```
const people = [
  { name: 'Ibim', year: 1988 },
  { name: 'Tari', year: 1986 },
  { name: 'Nengi', year: 1970 },
  { name: 'Dami', year: 2015 }
];

const comments = [
  { text: 'Love this!', id: 523423 },
  { text: 'This is great', id: 823423 },
  { text: 'You are the best', id: 2039842 },
  { text: 'Jollof rice is my fav food ever', id: 123523 },
  { text: 'Well done oooo!', id: 542328 }
];
```

The `people` array contains objects representing individuals with their names and birth years, while the `comments` array contains objects representing comments with their text content and unique IDs.

## Array Manipulations

The JavaScript code block performs the following array manipulations:

### `Array.prototype.some()`

Checks if at least one person in the `people` array is 19 years or older using the `some()` method. It does so by comparing the current year with the birth year of each person in the array. The result is stored in the `isAdult` variable, which is logged to the console.

```
const isAdult = people.some(person => ((new Date()).getFullYear()) - person.year >= 19 );
console.log({isAdult});  
```

### `Array.prototype.every()`

Checks if every person in the `people` array is 19 years or older using the `every()` method. It does so by comparing the current year with the birth year of each person in the array. The result is stored in the `allAdults` variable, which is logged to the console.

```
const allAdults = people.some(person => ((new Date()).getFullYear()) - person.year >= 19 );
console.log({allAdults});
```
### `Array.prototype.find()`

Finds the comment object in the `comments` array that has an ID of 823423 using the `find()` method. The result is stored in the `comment` variable, which is logged to the console.

```
const comment = comments.find(comment => comment.id === 823423);
console.log(comment);
```

### `Array.prototype.findIndex()`

Finds the index of the comment object in the `comments` array that has an ID of 823423 using the `findIndex()` method. The result is stored in the `index` variable, which is logged to the console.

```
const index = comments.findIndex(comment => comment.id === 823423);
console.log(index);
```

## Conclusion

This code demonstrates some common array methods in JavaScript and how they can be used to manipulate arrays in various ways.
