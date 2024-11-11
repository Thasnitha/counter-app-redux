                  REDUX
---------------------------------------------------------------------------------------
-it is js library
-REDUX consist two packages - npm install react-redux,npm install @reduxjs/toolkit
  1) React redux : official react bindings for redux

  2) Redux toolkit :The official, opinionated, batteries-included toolset for efficient Redux development

3.Importand API used in Redux :-
   configureStore():This method is used to create store for Redux 
   -Step to create Redux store in React Application 
   1) create a folder redux logic in src folder
   2)Inside redux folder create a js file for creating redux--here we define steps logic to create redux store.call configure store method and use reducers to hold the state to be shared
  - To provide store to our react app use 'provider' component of react-redux library.
   Provider component has 'store' attribute using it we can provide our store to react app.Inorder to do that make provider component as the root   component of our react app.Give these steps in main.js file

-createReducer(): used to create reducers where we can store updated state inside store.action output comes here .so first we should create actions

createAction(): used to create action where we can define logic to update state ,output of action automatically return to its reducer.
createSlice(): used to combine action and reducer in a single file.return action and reducer. it accepts initial state ,slice name 
  steps to create slice :
    1) create a js file for defining slice 
    2)createSlice method call where we have to define reduceres as object,its key act as actions and its value act as reducer function.it has minimum one argument which gives slice state .

4.Hooks used in component for managing state using redux
useSelector(state=>state.reducer-name)used to select state from store in a component

-useDispatch (): this hook is used to execute an action from an component.This hook will return a function that is capable of dispatching an action as its argument when we call the function.
- action without argument : dispatch-function(action-name())
- action with argument :dispatch-function(action-name(arg1,...)), access arg of action in slice  reduce function  it uses its secont argument which is an object with 2 key payload and type . payload





Props drilling-passing props from one component in to another .it increases the coupling .
to avoid props drilling - REDUX-create a store to access equally for all global .it is js Library it is used to manage state .
install - react-redux
redux -toolkit
how to create store :
   configureStore()
values storing 
  - reducers : hold updated state .it available inside store
  - action: output automattically go to  reducers,logic to update state ,
  -To execute action using useDispatch
  - useselector-to access datas in store by component
  -Provider, it provide store globally
