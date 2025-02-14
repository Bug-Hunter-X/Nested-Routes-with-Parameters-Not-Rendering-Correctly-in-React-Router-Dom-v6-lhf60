# Nested Routes with Parameters Not Rendering Correctly in React Router Dom v6

This repository demonstrates a bug in React Router Dom v6 where nested routes with parameters do not render correctly.  The nested route component doesn't receive the expected parameters from the parent route. This issue can occur when using nested routes with dynamic segments. The solution involves using the `useParams` hook within the nested component to correctly access the parameters.

## Bug Description

The provided code shows a simple application with nested routes.  When navigating to a nested route with a parameter, the nested component does not display the parameter. This problem often occurs when nested routes are combined with dynamic segments within the route paths.  The solution focuses on correctly using the `useParams` hook in the nested component to access the route parameters passed down from the parent route.

## Solution

The bug is resolved by correctly using the `useParams` hook in the nested component. This hook allows the nested component to access the parameters from its parent route. The `useParams` hook provides an object containing the key-value pairs of the dynamic segments.