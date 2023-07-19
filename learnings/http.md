
# Project - Generate recipes website

## 1. Write code that executes asynchronously
- Writing code that executes asynchronously offers several benefits, especially in scenarios where you have tasks that can run independently without blocking the main thread of execution. Asynchronous code can improve performance, responsiveness, and scalability in various applications. Here are some reasons why in this we consider writing asynchronous code:

 -  **Improved Responsiveness:** Asynchronous code allows applications to remain responsive to user input while performing time-consuming tasks in the background. This prevents the user interface from freezing or becoming unresponsive during long-running operations.

  - **Utilizing Resources Efficiently** Asynchronous code can efficiently use system resources by avoiding idle waiting periods. While one task is waiting for I/O or network operations, the system can execute other tasks concurrently, maximizing resource utilization.

- **Scalability** Asynchronous code is essential for building scalable applications, as it enables handling multiple requests simultaneously without creating a new thread for each request. This way, you can efficiently handle more concurrent users without significant performance degradation.

 - **Non-Blocking I/O** Asynchronous programming is particularly valuable when dealing with I/O-bound operations, such as reading/writing files or making network requests. It allows the application to move on to other tasks while waiting for the I/O operation to complete.

 -  **Parallelism** Asynchronous code can also lead to parallel execution of tasks on multi-core processors, further enhancing performance by utilizing available CPU cores efficiently.

### Here is an example:

```
export const getRecipes = async (searchTerm) => {
  try {
    toogleLoadingSpinner(true)
    const getRecipes = await fetch(
      `${baseUrl}?type=public&q=${searchTerm}&app_id=${appId}&app_key=${appKey}`
    )
    const recipes = await getRecipes.json()

    toogleLoadingSpinner(false)
    return recipes
  } catch (error) {
    console.log(error)
    onApiError()
  }
}
```

1. Asynchronous Fetch Request: The main advantage of using async/await is to make asynchronous fetch requests in a synchronous-looking manner. The await keyword allows you to pause the execution until the fetch operation completes and returns the result. This way, the code reads more linearly and becomes easier to understand.

2. Error Handling: The try...catch block is used to handle any errors that might occur during the asynchronous operations. With async/await, you can handle errors in a more structured and synchronous style, making it easier to catch and manage exceptions.

3. Loading Spinner Control: By using await, you ensure that the loading spinner is toggled on before the fetch request is made and toggled off after the request is completed. This ensures that the spinner accurately reflects the status of the asynchronous operation.

4. Maintainable and Readable Code: The use of async/await simplifies the code and makes it more maintainable. Asynchronous operations can become complex when using callbacks or promises directly. async/await provides a cleaner and more readable way to handle asynchronous tasks, making it easier for developers to work with and debug the codebase.




## 2. Use promises to access values that aren’t available synchronously
  - When working with APIs is important to handle asynchronous operations correctly.
  - Promises use a more linear and structured syntax compared to nested callbacks, making the code easier to read and understand. This readability becomes especially valuable when dealing with complex asynchronous operations.
  - Promises have built-in error handling through the **.catch()** method, allowing you to handle errors from asynchronous operations in a centralized manner. This simplifies error management and prevents callback hell.
  - Chaining: Promises support chaining through the **.then()** method, which allows you to perform multiple operations sequentially. This chaining pattern makes it easy to handle dependencies between asynchronous tasks.
  - Promise Composition: Promises support composition using methods like **Promise.all()** and Promise.race(). This enables you to coordinate multiple asynchronous operations and handle their combined results efficiently.


## 3. Use the fetch method to make HTTP requests and receive responses

```
export const getRecipeById = async (recipeId) => {
  const getRecipe = await fetch(
    `${baseUrl}/${recipeId}?type=public&app_id=${appId}&app_key=${appKey}`
  )
  const recipes = await getRecipe.json()
  return recipes
}
```
The given code exports an asynchronous function getRecipeById that fetches a recipe by its ID from a remote server using the provided recipeId, appId, and appKey. It then parses the fetched data into JSON format and returns the resulting recipes object.

## 4. Configure the options argument of the fetch method to make GET and POST requests

## 6. Use the map array method to create a new array containing new values

## 7. Use the filter array method to create a new array with certain values removed

## 8. Access DOM nodes using a variety of selectors

## 9. Add and remove DOM nodes to change the content on the page

## 10. Toggle the classes applied to DOM nodes to change their CSS properties

## 11. Use consistent layout and spacing

## 12. Follow a spacing guideline to give our app a consistent feel

## 13. Debug client side JS in our web browser

## 14. Use console.log() to help us debug our code
