# Tailwind CSS @apply Directive with Undefined Class

This repository demonstrates a common error when using Tailwind CSS's `@apply` directive: applying a class that hasn't been defined in your configuration.

## The Problem

The `@apply` directive is a powerful tool for reusing styles, but it relies on the existence of the classes you're applying.  If you accidentally use a class name that's not defined in your `tailwind.config.js` (or equivalent), Tailwind will simply ignore it, resulting in no styling being applied.

## Reproducing the Bug

1. Clone this repository.
2. Run `npm install` to install the necessary dependencies (if any).
3. Open `bug.js` to see the code that causes the error.  Note the use of `nonExistentClass`. 
4. Open the corresponding HTML file and observe that the `<div>` element has no styling applied because of this error. 

## Solution

The solution is straightforward: make sure all classes used within the `@apply` directive are correctly defined in your Tailwind CSS configuration.  Correct configuration will ensure that the style is applied appropriately.

## Running the Solution
1. Open `bugSolution.js` to observe that the nonExistentClass is defined in the tailwind.config.js, making the `@apply` directive work correctly.
2. Re-run the application to see the style applied correctly.