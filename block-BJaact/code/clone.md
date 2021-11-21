1. Write the output with reason

```js
const person = {
  firstName: 'John',
  lastName: 'Doe',
};

let person2 = person;

person.firstName = 'Arya';

console.log(person2.firstName); // output will be Arya becoz person2 = person hence person2.firstName will be value Arya.
console.log(person.firstName); // output will be Arya becoz below the code has declear (person.firstName = 'Arya';).
console.log(person.lastName); // output will be Doe because lastName is 'Doe'.
console.log(person == person2); // output will be true because person and person2 has same value.
console.log(person === person2); // output will be true because person and person2 has same value.
console.log(person.lastName === person2.lastName); // output will be true because person.lastName and person2.lastName has same value.
```

2. Write the output with reason:

```js
let person = {
  firstName: 'John',
  lastName: 'Doe',
  address: {
    street: 'North 1st',
    city: 'San Jose',
    state: 'CA',
    country: 'USA',
  },
};

let personTwo = { ...person };

person.firstName = 'Arya';
person.city = 'Navada';

console.log(personTwo.firstName); // output will be John because decler below the code personTwo = person and person = firstName is 'John'.
console.log(person.firstName); // output will be Arya becoz the (person.firstName) is the second value will be 'Arya'.
console.log(personTwo.lastName); // output will be Doe.
console.log(person.firstName === personTwo.firstName); // output will be false because the both value are no same.
console.log(person == personTwo); // output will be false because the spret oparator will be firstName and  lastName.
console.log(person === personTwo); // output will be false because the spret oparator will be firstName and  lastName.
console.log(person.address === personTwo.address); // output will be true because the new update personTwo.address is the same value of person.address.
console.log(person.address == personTwo.address); // output will be true because the new update personTwo.address is the same value of person.address.
console.log(personTwo.address.city); // output will be San Jose.
console.log(person.address.city); // output will be San Jose. 
console.log(person.address.city == personTwo.address.city); // output will be true.
```

3. Write the output with reason:

```js
let person = {
  firstName: 'John',
  lastName: 'Doe',
  address: {
    street: 'North 1st',
    city: 'San Jose',
    state: 'CA',
    country: 'USA',
  },
};

let personTwo = { ...person, address: { ...person.address } };

person.firstName = 'Arya';
person.city = 'Navada';

console.log(personTwo.firstName); // output will be John.
console.log(person.firstName); // output will be Arya because the name will be update.
console.log(personTwo.lastName); // output will be Doe.
console.log(person.firstName === personTwo.firstName); // output wll be false.
console.log(person == personTwo); // output will be false.
console.log(person === personTwo); // output will be false.
console.log(person.address === personTwo.address); // output will be false
console.log(person.address == personTwo.address); // output will be false
console.log(personTwo.address.city); // output will be San Jose.
console.log(person.address.city); // output will be San Jose.
console.log(person.address.city == personTwo.address.city); // output will be true.
```

4. Clone the `blogs` variable into a new variable named `clonedBlogs`

```js
let blogs = [
  {
    id: 1,
    title: 'Post #1',
    body: 'My first blog post',
  },
  {
    id: 2,
    title: 'Post #2',
    body: 'My second blog post',
  },
  {
    id: 3,
    title: 'Post #3',
    body: 'My third blog post',
  },
];

// Your code goes here

let clonedBlogs = [{ ...blogs[0] }, { ...blogs[1] }, { ...blogs[2] }];
```

5. Clone the `question` variable into a new variable named `questionClone`

```js
var questions = [
  {
    prompt: 'Why is the sky blue?',
    responses: [
      'Because the color blue was on sale at Wallmart',
      'Because blue is the prettiest color',
      'Because the air molecules difract blue light more than any other color',
    ],
  },
  {
    prompt: 'Why are leaves usually green?',
    responses: [
      'So green caterpillars can hide better.',
      'Because leaves can more easily make energy with green light',
      "Because leaves absorb red and blue light so it's green that is reflected",
    ],
  },
];

// Your code goes here

let questionClone = [{ ...questions[0]}, { ...questions[1]}];
```

6. Clone the `allBlogs` variable into a new variable named `allBlogsClone`

```js
var allBlogs = {
  id: 1,
  title: 'Alamofire JSON Serialization',
  body: 'All about serialization in Alamofire...',
  author: {
    id: 1,
    fullName: 'Jeff Potter',
    username: 'jpotts18',
  },
  comments: [
    {
      id: 1,
      body: 'Thanks for the help Jeff, this saved me hours',
    },
    {
      id: 2,
      body: 'Your welcome. I am happy to help!',
    },
  ],
};

// Your code goes here


let allBlogsClone = { ...allBlogs, 
author: { ...allBlogs.author}, 
comments: [{ ...allBlogs.comments[0]}, { ...allBlogs.comments[1]}] ,};

```

7. Clone the `person` variable into a new variable named `clonedPerson`

```js
let person = [
  {
    input: { name: 'Ryan' },
    output: { name: 'Ryan' },
  },
  {
    input: { name: { first: 'Ryan', last: 'Haskell-Glatz' } },
    output: { firstName: 'Ryan', lastName: 'Haskell-Glatz' },
  },
  {
    input: { name: 'Ryan', age: 24 },
    output: { name: 'Ryan', age: 24 },
  },
  {
    input: {
      name: { first: 'Ryan', last: 'Haskell-Glatz' },
      birthday: { year: 1993, month: 'Nov' },
    },
    output: {
      firstName: 'Ryan',
      lastName: 'Haskell-Glatz',
      birthdayYear: 1993,
      birthdayMonth: 'Nov',
    },
  },
];

// Your code goes here

let clonedPerson = [{ ...person[0]}, { ...person[1]}, { ...person[2]}, { ...person[3]},
output: { ...person.output}
 ,]
```

8. Write a function named `cloneObject` that accepts an object and returns the clone of the object

```js
function cloneObject() {
  // your code
}

// Run the test below to check your function

let user = {
  name: 'John',
  house: 'Stark',
  sisters: ['Arya', 'Sansa'],
};
let cloned = cloneObject(user);

let person = {
  firstName: 'John',
  lastName: 'Doe',
  address: {
    street: 'North 1st',
    city: 'San Jose',
    state: 'CA',
    country: 'USA',
  },
};

let clonedPerson = cloneObject(user);

console.log(
  `The user object is ${
    user == cloned ? `not clone` : `cloned successfully 😁👑`
  }`
);
console.log(
  `The person object is ${
    person == clonedPerson ? `not clone` : `cloned successfully 😁👑`
  }`
);
```

