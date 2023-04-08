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

The people array contains objects representing individuals with their names and birth years, while the comments array contains objects representing comments with their text content and unique IDs.

## Array Manipulations

The JavaScript code block performs the following array manipulations:

### Array.prototype.some()

Checks if at least one person in the people array is 19 years or older using the some() method. It does so by comparing the current year with the birth year of each person in the array. The result is stored in the isAdult variable, which is logged to the console.

```
const isAdult = people.some(person => ((new Date()).getFullYear()) - person.year >= 19 );
console.log({isAdult});  
```

### Array.prototype.every()

Checks if every person in the people array is 19 years or older using the every() method. It does so by comparing the current year with the birth year of each person in the array. The result is stored in the allAdults variable, which is logged to the console.

```
const allAdults = people.some(person => ((new Date()).getFullYear()) - person.year >= 19 );
console.log({allAdults});
```
### Array.prototype.find()

Finds the comment object in the comments array that has an ID of 823423 using the find() method. The result is stored in the comment variable, which is logged to the console.

```
const comment = comments.find(comment => comment.id === 823423);
console.log(comment);
```

### Array.prototype.findIndex()

Finds the index of the comment object in the comments array that has an ID of 823423 using the findIndex() method. The result is stored in the index variable, which is logged to the console.

```
const index = comments.findIndex(comment => comment.id === 823423);
console.log(index);
```

### Array.prototype.splice()

Deletes the comment object with the ID of 823423 from the comments array using the splice() method. This line is currently commented out.

```
// comments.splice(index, 1);
```

## Create a new Array with slice() and the spread operator

Creates a new array newComments that contains all the comments before and after the deleted comment. The slice() method is used to extract the arrays before and after the deleted comment, which are then combined using the spread operator. However, there is a mistake in this code block as the second slice should end at `index +
