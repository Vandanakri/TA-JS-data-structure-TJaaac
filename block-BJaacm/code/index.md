```js
let user = {
  name: 'Arya',
  sibling: ['Robb', 'Ryan', 'John'],
};
let allBrothers = ['Robb', 'Ryan', 'John'];
let brothersCopy = user.sibling;
let usename = user.name;
let newUser = user;
```

1. Memory representation

- Create the memory representation of the above snippet on notebook.
- Take a photo/screenshot and add it to the folder `code`

<!-- To add this image here use ![name](./hello.jpg) -->

2. Answer the following with reason:

- `user == newUser;` // output will be true because the both value will be same and store in same address.
- `user === newUser;` // output will be true because the both value and data type will be same.
- `user.name === newUser.name;` // output will be true because the both value and data type will be same.
- `user.name == newUser.name;`// output will be true because the both value will be same.
- `user.sibling == newUser.sibling;` // output will be true because the both value will be same.
- `user.sibling === newUser.sibling;` // output will be true because the both value and data type will be same.
- `user.sibling == allBrothers;` // output will be false because the value will be not same.
- `user.sibling === allBrothers;` // output will be false because the value will be not same.
- `brothersCopy === allBrothers;` // output will be false because the value will be not same.
- `brothersCopy == allBrothers;` // output will be false because the value will be not same.
- `brothersCopy == user.sibling;` // output will be true because the both value will be same.
- `brothersCopy === user.sibling;` // output will be true because the both value will be same.
- `brothersCopy[0] === user.sibling[0];` // output will be true because the both value will be same.
- `brothersCopy[1] === user.sibling[1];` // output will be true because the both value will be same.
- `user.sibling[1] === newUser.sibling[1];`// output will be true because the both value will be same.


