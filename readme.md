# React useState and Javascript Objects 

Description 
--------------
Write an application which uses useState React hook and save an object 

1. store the data in localStorage 
2. Show again if we relad the page show the data
3. Read and write into local storage and use useState React hook 
4. Delete Record 
5. Edit Record 


```sh
   obj = { 
         name:"Qasim",
         age :31,
         email: "syedqasim8888@gmail.com"
   }

```

## Java script objects defination and examples 
  In JavaScript, an object is a collection of properties, where each property is a key-value pair. Here's an example of how to define an object in JavaScript:
  ```sh
  const person = {
  name: 'John',
  age: 30,
  address: {
    street: '123 Main St',
    city: 'Anytown',
    state: 'CA',
    zip: '12345'
  }
};
  ```
  In the example above, person is an object that has three properties: name, age, and address. The address property is itself an object with four properties: street, city, state, and zip.

Here are a few more examples of JavaScript objects:
```sh
const car = {
  make: 'Toyota',
  model: 'Corolla',
  year: 2022,
  features: ['backup camera', 'Bluetooth', 'keyless entry']
};

const book = {
  title: 'To Kill a Mockingbird',
  author: 'Harper Lee',
  year: 1960,
  genres: ['fiction', 'coming-of-age', 'southern gothic']
};

const employee = {
  name: 'Jane Smith',
  jobTitle: 'Software Engineer',
  salary: 100000,
  department: {
    name: 'Engineering',
    manager: 'John Doe'
  }
};

```

## Localstorage in browsers how to access them in JS 
   In web browsers, local storage is a feature that allows you to store key-value pairs in the user's web browser. Local storage is specific to each domain, meaning that one website cannot access the local storage of another website. Here's how you can access local storage in JavaScript:

1. Saving data to local storage:
To save data to local storage, you can use the localStorage.setItem() method. This method takes two arguments: the name of the key, and the value you want to save.
```sh
localStorage.setItem('name', 'John');
```
2. This will store the value John with the key name in the local storage.

Retrieving data from local storage:
To retrieve data from local storage, you can use the localStorage.getItem() method. This method takes one argument: the name of the key you want to retrieve.
```sh
const name = localStorage.getItem('name');
console.log(name);

        This will retrieve the value stored with the key name from the local storage and store it in the name variable.
```
3. Removing data from local storage:
To remove data from local storage, you can use the `localStorage.removeItem()` method. This method takes one argument: the name of the key you want to remove.
```sh
localStorage.removeItem('name');
        This will remove the data stored with the key name from the local storage.
```
4. Checking if a key exists in local storage:
To check if a key exists in local storage, you can use the localStorage.getItem() method. If the key does not exist, the method will return null.
```sh
const name = localStorage.getItem('name');
if (name === null) {
  console.log('Name not found in local storage');
} else {
  console.log(`Name found in local storage: ${name}`);
}
```

