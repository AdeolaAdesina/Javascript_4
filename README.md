# Arrays

Organizing and storing data is a foundational concept of programming.

One way we organize data in real life is by making lists. Let’s make one here:

```
New Year's Resolutions:

1. Keep a journal 
2. Take a falconry class
3. Learn to juggle
```

Let’s now write this list in JavaScript, as an array:

```
let newYearsResolutions = ['Keep a journal', 'Take a falconry class', 'Learn to juggle'];
```

## Class work

```
let newYearsResolutions = ['Keep a journal', 'Take a falconry class', 'Learn to juggle'];

console.log(newYearsResolutions);
```

Run the code to see what is logged to the console.


# Create an Array

One way we can create an array is to use an array literal. An array literal creates an array by wrapping items in square brackets ```[]```.

Remember from the previous exercise, arrays can store any data type — we can have an array that holds all the same data types or an array that holds different data types.

![Screenshot_197](https://user-images.githubusercontent.com/29931071/201892721-02ddb42c-8505-401f-9d23-94337b05616e.png)


Let’s take a closer look at the syntax in the array example:

- The array is represented by the square brackets ```[]``` and the content inside.
- Each content item inside an array is called an element.
- There are three different elements inside the array.
- Each element inside the array is a different data type.


We can also save an array to a variable. You may have noticed we did this in the previous exercise:

```
let newYearsResolutions = ['Keep a journal', 'Take a falconry class', 'Learn to juggle'];
```


## Class work

1. Declare a variable using ```const``` named ```hobbies``` and set it equal to an array with three strings inside of it.

2. Use console.log() to print hobbies to the console.

Output:

![Screenshot_198](https://user-images.githubusercontent.com/29931071/201893606-2b9c6310-1048-460f-8cf9-1c29d1e19c86.png)


# Accessing Elements

Each element in an array has a numbered position known as its index. We can access individual items using their index, which is similar to referencing an item in a list based on the item’s position.


Arrays in JavaScript are zero-indexed, meaning the positions start counting from 0 rather than 1. Therefore, the first item in an array will be at position 0. Let’s see how we could access an element in an array:

![Screenshot_199](https://user-images.githubusercontent.com/29931071/201895515-8b437f6c-adb5-4e72-80eb-339de5dbf64a.png)


In the code snippet above:

- cities is an array that has three elements.
- We’re using bracket notation, [] with the index after the name of the array to access the element.
- cities[0] will access the element at index 0 in the array cities. You can think of cities[0] as accessing the space in memory that holds the string 'New York'.


## Class work

1. Individual elements in arrays can also be stored to variables.

Create a variable named listItem and set it equal to the first item in the famousSayings array using square bracket notation ([]).

Then use console.log() to print the listItem variable to the console.

2. Now, console.log() the third element in the famousSayings array using bracket notation to access the element.

Do not save the element to a new variable before you log it.

3. Awesome, you can access each element in an array using the index. But what happens if you try to access an index that is beyond the last element?

Try to log the item at index [3] of famousSayings to the console. What is logged to the console?


Output:

![Screenshot_200](https://user-images.githubusercontent.com/29931071/201896217-a9624100-e36b-4acc-aac4-2c69bbae0d0e.png)


# Update Elements

In the previous exercise, you learned how to access elements inside an array or a string by using an index. Once you have access to an element in an array, you can update its value.

```
let seasons = ['Winter', 'Spring', 'Summer', 'Fall'];
 
seasons[3] = 'Autumn';
console.log(seasons); 
//Output: ['Winter', 'Spring', 'Summer', 'Autumn']
```

## Class work

```
let groceryList = ['bread', 'tomatoes', 'milk'];
```

Change the second element of the array groceryList to 'avocados'.


Output:

![Screenshot_201](https://user-images.githubusercontent.com/29931071/201896890-f2bc35e9-a11b-4939-9097-18363d56e9f4.png)


# Arrays with let and const

You may recall that you can declare variables with both the let and const keywords. Variables declared with let can be reassigned.

Variables declared with the const keyword cannot be reassigned. However, elements in an array declared with const remain mutable. Meaning that we can change the contents of a const array, but cannot reassign a new array or a different value


## Class work

```
let condiments = ['Ketchup', 'Mustard', 'Soy Sauce', 'Sriracha'];

const utensils = ['Fork', 'Knife', 'Chopsticks', 'Spork'];
```

1. Below the two existing arrays, re-assign the element in index 0 of condiments to 'Mayo'.

Log the updated array, condiments, to the console.

2. Below your code from Step 1, reassign condiments to be a new array that contains a single string ['Mayo']

Log the result to the console.

Notice that you can re-assign elements in an array and re-assign an entire new array to a variable declared using the let keyword.

3. Below your code from Step 2, re-assign the last item from the utensils array to 'Spoon'.

Log the updated array to the console.

Output:

![Screenshot_202](https://user-images.githubusercontent.com/29931071/201897577-c1e24a87-700c-47b3-a00d-7017382444a5.png)



# The .length property

One of an array’s built-in properties is length and it returns the number of items in the array. We access the .length property just like we do with strings. Check the example below:

```
const newYearsResolutions = ['Keep a journal', 'Take a falconry class'];

console.log(newYearsResolutions.length);
// Output: 2
```

## Class work

```
const objectives = ['Learn a new language', 'Read 52 books', 'Run a marathon'];
```

Find the length of the objectives array and log it to the console.

Output:

![Screenshot_203](https://user-images.githubusercontent.com/29931071/201898157-14f946ff-b299-4dd6-b27d-2767dffe56dc.png)


# The .push() Method

Let’s learn about some built-in JavaScript methods that make working with arrays easier. These methods are specifically called on arrays to make common tasks, like adding and removing elements, more straightforward.

One method, .push(), allows us to add items to the end of an array. Here is an example of how this is used:

```
const itemTracker = ['item 0', 'item 1', 'item 2'];
 
itemTracker.push('item 3', 'item 4');
 
console.log(itemTracker); 
// Output: ['item 0', 'item 1', 'item 2', 'item 3', 'item 4'];
```


## Class work

```
const chores = ['wash dishes', 'do laundry', 'take out trash'];
```

1. Add two elements to the chores array using .push().

2. Use console.log to print your chores array to make sure your items were added.


Output:

![Screenshot_204](https://user-images.githubusercontent.com/29931071/201898750-75595049-2cb6-4156-a7fe-dc08a3c846ae.png)


# The .pop() Method

Another array method, .pop(), removes the last item of an array.

```
const newItemTracker = ['item 0', 'item 1', 'item 2'];
 
const removed = newItemTracker.pop();
 
console.log(newItemTracker); 
// Output: [ 'item 0', 'item 1' ]
console.log(removed);
// Output: item 2
```


# More Array Methods

There are many more array methods than just .push() and .pop(). You can read about these array methods on the Docs entry for JavaScript Arrays.

Some arrays methods that are available to JavaScript developers include: .join(), .slice(), .splice(), .shift(), .unshift(), and .concat() amongst many others. Using these built-in methods make it easier to do some common tasks when working with arrays

## Class work

```
const groceryList = ['orange juice', 'bananas', 'coffee beans', 'brown rice', 'pasta', 'coconut oil', 'plantains'];
```

1. Use the .shift() method to remove the first item from the array groceryList.

Log the new groceryList to the console

2. Under the code added in step 1, use the .unshift() method to add 'popcorn' to the beginning of your grocery list.

After calling .unshift() on groceryList, log groceryList to the console.

You may wish to delete the console.log() statement from the previous step.

3. You’re in a hurry so you decide to ask a friend to help you with your grocery shopping. You want him to pick up the 'bananas', 'coffee beans', and 'brown rice'.

Under the code you added for step 2, use .slice() to provide your friend with a list of these three things.

Log this part of the list to the console. Unlike the two previous checkpoints, you should do both of these steps in one line.

4. Let’s find the index of a particular element in groceryList using .indexOf().

Call .indexOf() on groceryList to find the index of the element 'pasta' and save the returned value to a const variable named pastaIndex.

Then log pastaIndex to the console. (You may remove the other console.log() statements to declutter the terminal.)


Output:

![Screenshot_205](https://user-images.githubusercontent.com/29931071/201899930-8275ee2f-f6f4-49c3-b675-da485ac5ba26.png)


# Arrays and Functions
Throughout the lesson we went over arrays being mutable, or changeable. Well what happens if we try to change an array inside a function? Does the array keep the change after the function call or is it scoped to inside the function?

Take a look at the following example where we call .push() on an array inside a function. Recall, the .push() method mutates, or changes, an array:

```
const flowers = ['peony', 'daffodil', 'marigold'];
 
function addFlower(arr) {
  arr.push('lily');
}
 
addFlower(flowers);
 
console.log(flowers); // Output: ['peony', 'daffodil', 'marigold', 'lily']
```


Let’s go over what happened in the example:

- The flowers array that has 3 elements.
- The function addFlower() has a parameter of arr uses .push() to add a 'lily' element into arr.
- We call addFlower() with an argument of flowers which will execute the code inside addFlower.
- We check the value of flowers and it now includes the 'lily' element! The array was mutated!


# Class work

```
const concept = ['arrays', 'can', 'be', 'mutated'];

function changeArr(arr){
  arr[3] = 'MUTATED';
}
```

1. Underneath the function call, log concept to the console to check if this reassignment mutated the array.

2. Let’s double check what happens if we mutate an array using a built-in method inside a function.

Under the console.log() statement, define another function named removeElement that takes a parameter of newArr. Inside the function body call .pop() on newArr.

3. Call removeElement() with an argument of concept.

4. After calling removeElement(concept), check the value of concept by logging it to console.

Notice that in both cases, the change to the array was maintained outside of the function!


Output:

![Screenshot_206](https://user-images.githubusercontent.com/29931071/201901256-6197c531-0d82-4834-8602-9026f1b72496.png)


# Nested Arrays

Earlier we mentioned that arrays can store other arrays. When an array contains another array it is known as a nested array. Examine the example below:

```
const nestedArr = [[1], [2, 3]];
```

To access the nested arrays we can use bracket notation with the index value, just like we did to access any other element:

```
const nestedArr = [[1], [2, 3]];
 
console.log(nestedArr[1]); // Output: [2, 3]
```

Then, if we wanted to access the elements within the nested array we can chain, or add on, more bracket notation with index values.

```
const nestedArr = [[1], [2, 3]];
 
console.log(nestedArr[1]); // Output: [2, 3]
console.log(nestedArr[1][0]); // Output: 2
```

