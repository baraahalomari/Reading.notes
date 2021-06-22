## Describe (in plain English) what Array.map() does 

**Array. Map()** is used to create a new array by calling a function on each element of the passed array and  calls the provided function once for each element in an array, in order.


## Describe (in plain English) what Array.reduce() does

**Array.reduce** iterates over the array and invokes the callback on each element. it returns whatever the final invocation of the callback returns.

reduce takes as its arguments a callback function and an initial value, and the callback takes the previous result .

## Provide code snippets showing how to use superagent() to fetch data from a URL and log the result

### With normal Promise .then() syntax


.get('/search')

   .then(res => {

        // res.body, res.headers, res.status

         })

         .catch(err => {

              // err.message, err.response

              });


### Again with async / await syntax


async function name() {

    try {

        const res = await axios.get(API);

        // res.body

        } catch(err){

        // err.message

        }

        }



## Explain promises as though you were mentoring a Code 301 level student

This lets asynchronous methods return values like synchronous methods: instead of immediately returning the final value, the asynchronous method returns a promise to supply the value at some point in the future.


A pending promise can either be fulfilled with a value or rejected with a reason (error). When either of these options happens, the associated handlers queued up by a promise's then method are called. If the promise has already been fulfilled or rejected when 
a corresponding handler is attached, the handler will be called, so there is no race condition between an asynchronous operation completing and its handlers being attached.

## Are all callback functions considered to be Asynchronous? Why or Why Not?

taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous. 

For a function to be asynchronous it needs to perform an asynchronous operation. It needs to incorporate the argument callback in handling the results of this asynchronous operation. Only this way the function becomes asynchronous.
