# useReducers Hook

- userReducer is a hook that is used for state management

- It is an alternative to useState

- What's the difference?
  - useState is built using useReducer
- When to useReducer vs useState?

# Hooks so far

- useState - state
- useEffect - side effects
- useContext - context API
- useReducer - reducers

# JS reduce Function

```js
const array1 = [1, 2, 3, 4];

// 0 + 1 + 2 + 3 + 4
const initialValue = 0;
const sumWithInitial = array1.reduce(
  (accumulator, currentValue) => accumulator + currentValue,
  initialValue
);

console.log(sumWithInitial);
// Expected output: 10
```

# reduce vs useReducer

<table>
  <thead>
    <tr>
      <th>reduce</th>
      <th>useReducer</th>
    </tr>
   </thead>
   <tbody>
     <tr>
       <td>array.reduce(reducer, initialValue)</td>
       <td>useReducer(reducer, initialValue)</td>
     </tr>
     <tr>
       <td>singleValue = reducer(accumulator, itemValue)</td>
       <td>newState = reducer(currentState, action)</td>
     </tr>
     <tr>
       <td>reduce method returns a single value</td>
       <td>useReducer returns a pair of values. [newState, dispatch]</td>
     </tr>
  </tbody>
</table>

# useReducer Summery

- useReducer is a hook that is used for state management in React
- useReducer is related to reducer functions
- useReducer(reducer, initialState)
- reducer(currentState, action)