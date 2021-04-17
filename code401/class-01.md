# Class 1 - Map, Reduce, Promises & Callbacks

1. Describe (in plain English) what Array.map() does
    - The map method returns a new modified array by iterating through each item in the array the method is called on, and modifying each item based on the changes you want.
2. Describe (in plain English) what Array.reduce() does
    - The reduce method "reduces" an array to a single value. This happens by setting a starting value. The method iterates through each item in the array and then modifies the starting value based on that item and how you want that item to change the starting value. The reduce method could be used to find the sum of an array, by setting the starting value to 0 and then adding each number in the array. Other examples could include concatenating strings of an array.
3. Provide code snippets showing how to use superagent() to fetch data from a URL and log the result
With normal Promise .then() syntax
Again with async / await syntax

    ```javascript
    superagent.get('https://api.themoviedb.org/3/discover/movie')
      .then(results => {
        console.log(results)
      })
      .catch((err) => {
        console.error('tmdb error');
      });

    async function getMovie() {
      const movie = await superagent.get('https://api.themoviedb.org/3/discover/movie');
      console.log(movie);
    }
    ```

4. Explain promises as though you were mentoring a Code 301 level student
    - A Promise can be seen as a function that has the possibility of returning two things, either as a resolve or as a reject. When you call this function and it satisfies the coditions set by the function then it will return in the form of a resolve containing a value defined by the Promise, other wise it will return something in the form of a reject. When you call this promise function, it is a callback and you will have to wait for an answer from that function. This is where you can use async await, or .then().catch() to handle the promise.
    - See [https://replit.com/@cgantt/Promises#index.js](https://replit.com/@cgantt/Promises#index.js) for an example on using promises.
5. Are all callback functions considered to be Asynchronous? Why or Why Not?
    - All callback functions are not considered asynchronous. Callback functions can be handled asyncronously but this is not always the case and is not always necessary. Simple callbacks that do not rely on waiting for something can be added to the callstack and then taken off once they are handled, and this does not necessarily need to be done asyncronously.

[<== Back](../README.md)
