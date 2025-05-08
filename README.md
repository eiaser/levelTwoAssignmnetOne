# levelTwoAssignmnetOne
What are some differences between interfaces and types in TypeScript?
| Feature                     | Interface                                | Type                                                                   |
| --------------------------- | ---------------------------------------- | ---------------------------------------------------------------------- |
| Declaration Syntax          | `interface Person { ... }`               | `type Person = { ... };`                                               |
| Extending/Implementing      | `extends` keyword                        | `&` operator for intersections                                         |
| Merging Declarations        | Supports declaration merging             | Does not support declaration merging                                   |
| Flexibility                 | Primarily for object shapes              | More flexible, supports unions, intersections, and other complex types |
| Use Cases                   | Best for defining object shapes, classes | Best for advanced types, unions, intersections, or one-off types       |
| Primitive and Complex Types | Cannot define primitive types or unions  | Can define primitives, unions, intersections, etc.                     |


=======================================================================================================================================================
Explain the difference between any, unknown, and never types in TypeScript.

What is the any Type?
The ANY type in TypeScript is a "catch-all" type that allows a variable to hold any type of value, effectively disabling type checking for that variable. It can be thought of as a way to opt-out of TypeScript's static typing for certain cases.

When to Use any?
any is typically used when dealing with third-party libraries that don’t have type definitions.

What is the unknown Type?
The unknown type is similar to any, but it is more restrictive. With unknown, you cannot perform operations on a value until it has been explicitly checked for a specific type. This makes unknown a safer alternative to any.

When to Use unknown?
unknown should be used when uncertain about the type of a value but still want to enforce type checking before performing operations on it.

What is the never Type?
The never type represents values that will never occur. It is used for functions that either throw an error or have an infinite loop and never return a value.

When to Use never?
Use never for functions that either throw errors or never return.

It is particularly useful for narrowing down types in exhaustive checks with switch statements or if conditions.



