# Redux - Additional Topics

## Review, Research, and Discussion

### What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.

### When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

That will dispatch the response data to your action which will send the data to the reducer


## Document the following Vocabulary Terms

* **middleware**  Piece of software that takes the request data and modifies it before sending it along to the API.


* **thunk** Middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. The inner function receives the store methods dispatch and getState as parameters.

# Redux Toolkit (RTK) 

> The Redux Toolkit package is intended to be the standard way to write Redux logic.

## Redux Toolkit includes these APIs:

* configureStore()
* createReducer()
* createAction()
* createSlice()
* createAsyncThunk


## RTK Query

**RTK Query is provided as an optional addon within the @reduxjs/toolkit package. It is purpose-built to solve the use case of data fetching and caching, supplying a compact, but powerful toolset to define an API interface layer for your app.**

### RTK Query includes these APIs:

* createApi()
* fetchBaseQuery()
* &lt; ApiProvider />
* 
