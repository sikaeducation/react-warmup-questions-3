## What is a hook?

A function that lets you control state and other React features without having to write extra code. They allow you to "hook" into react lifecycle events.

## What is a side-effect?

Anything that effects something outside the scope of the function.

* Network
* Rendering

## How are side-effects handled in React?
## What is `useEffect` for?

* `useEffect`
  * For API calls, logging, etc.

## What are the parameters of `useEffect`?

1. A function with side effects
2. Array of values to track

```jsx
useEffect(fn, dependencies)

// Every time
useEffect(() => {
  // Some side-effect
})

// Once
useEffect(() => {
  // Some side-effect
}, [])

// Every time name changes
useEffect(() => {
  // Some side-effect
}, [name])

// Every time name or url changes
useEffect(() => {
  // Some side-effect
}, [name, url])
```

## How is SPA routing different from regular routing?

* Reloading the entire page, HTML comes from server
* Update the virtual DOM, compare it to the real DOM, render the difference

## What is React Router?

React way to handle SPA routing, offers components such as `<Switch>` to make routing easier

## What is conditional rendering in React components?

Display JSX based on a condition

* `&&` - `if`
* `? :` - `if` / `else`

Needs to be expressions!

## What is the role of the `<Router>` component in React Router?

* Contains link and switch, works as a container

## What is the role of the `<Switch>` component in React Router?

* Which route are you trying to pick?
* Conditional logic
* Wraps the actual route definitions
* That's where the component will render when a route matches

## What is the role of the `<Route>` component in React Router?

* Define the path for each page
* Define the JSX it should render

## What does this render if `isOverdue` is `false` and `daysRemaining` is 3?

```jsx
{
  isOverdue
    ? <span className="alert badge">Overdue!</span>
    : <span className="badge">{daysRemaining} days remaining</span>
}
```

## What is the role of the `<Link>` component in React Router?

* Where you define the link
* Change the URL
* Prevents regular routing

## What does this render if `isOverdue` is `true` and `daysRemaining` is 3?

```jsx
{
  isOverdue
    ? <span className="alert badge">Overdue!</span>
    : <span className="badge">{daysRemaining} days remaining</span>
}
```

## What does this render if `isOverdue` is `true`?

```jsx
{
  isOverdue && <span className="alert badge">Overdue!</span>
}
```

## What does this render if `isOverdue` is `false`?

```jsx
{
  isOverdue && <span className="alert badge">Overdue!</span>
}
```
