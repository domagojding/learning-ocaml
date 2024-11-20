Expressions (a value is an expression that does need any further evaluation)

```ocaml
3110;;
- : int = 3110
```
The way to read `- : int = 3110` is from right to left. 
```ocaml
true;;
- : bool = true

3110 > 2110;;
- : bool = true

"hello";;
- : string = "hello"

"hello" ^ " world";;
- : string = "hello world"

2.0 *. 3.14;;
- : float = 6.28
```
Writing type annotations with:
- so this is not like a typecast that you might be familiar from other languages, it's a type annotation, it's an additional constraint that you are asking the typechecker to verify for you.
```ocaml
(3110 : int);;
- : int = 3110
```
if then else
```ocaml
if "batman" > "superman" then "yay" else "boo";;
```
(Because strings are ordered lexicographically). A part of the **if** expression that's called the **guard** that occurs between the *if* and the *then* keywords. That's called a boolean. It evaluates to either *true* or *false*. If it evaluates to *true* the *then* branch is evaluated.

Syntax: **if e1 then e2 else e3**





