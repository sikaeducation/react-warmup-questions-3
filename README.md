## What is a hook?

## What is a side-effect?

## How are side-effects handled in React?

## What is `useEffect` for?

## What are the parameters of `useEffect`?

## How is SPA routing different from regular routing?

## What is React Router?

## What is conditional rendering in React components?

## What is the role of the `<Router>` component in React Router?

## What is the role of the `<Switch>` component in React Router?

## What is the role of the `<Route>` component in React Router?

## What does this render if `isOverdue` is `false` and `daysRemaining` is 3?

```jsx
{
  isOverdue
    ? <span className="alert badge">Overdue!</span>
    : <span className="badge">{daysRemaining} days remaining</span>
}
```
## What is the role of the `<Link>` component in React Router?

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
