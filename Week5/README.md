# DGL104 Process Portfolio | Week 5

Ryan Paranich | DGL104 | Winter 2021 | North Island College

---

## 0501

> Write a summary that outline the main similarities and differences between MVC, MVP and MVVM. You can use a list to make the distinctions clear, but you should write at least a brief paragraph describing when you might choose to use one over the other.

## Similiarities

In each of these architectures, the model remains essentially the same. The model contains business logic, state, and data. It is not tied to the view, controller, presenter, or view-model and because of this it is resuable in many contexts.

## MVC
### The View
The view is the representation of the model. It renders the UI and communicates to the controller. The view only communicates to the controller, and bcause of this, never interacts directly with the model.
### The Controller
The controller is the brains of the operation. It effectively "does" everything in our program. It talks to/from the model and view, and is the middle man, handling everything control related within our app.

## MVP
### The View
The view in an MVP architecture now implements a view interface. Here there is a java file that handls the view related methods. Good practice is to have the Activity implement a view interface so that the presenter has an interface to code to. This eliminates coupling it to any specific view and allows simple unit testing with a mock implementation of the view.

### The Presenter
This is much like the controller in MVC except that it's not at all tied to the view, just an interface. This, too, is more testable than the previous MVC architecture. Some coders would argue that the presenter should never have any references to any Android APIs or code.

## MVVM
### The View
The view binds to observable variables and actions exposed by the viewModel in a flexible way. Because we haven't really delved into this yet, I'm not certain I'd be able to describe it any differently than it's been described to me in the textbook thusfar.

### The ViewModel
The View Model is responsible for wrapping the model and preparing observable data needed by the view. It also provides hooks for the view to pass events to the model without being tied to the view.


---

## 0502

> Consider a recent (or current) programming project that uses global variables, or that contains 'coupled' code (i.e. method chaining, or multiple responsibilities). Consider what you would need to do to fix the code and write a brief strategy for your approach (you do not need to write new code here, but consider instead what you might do to 'decouple' your code).

---

## 0503

> Visit CodeWars.com and attempt at least two katas. Ideally you should finish both - so choose something that is within your level of programming expertise.