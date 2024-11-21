References:
* Installing: https://cs3110.github.io/textbook/chapters/preface/install.html
* Cornell OCaml course: https://youtube.com/playlist?list=PLre5AT9JnKShBOPeuiD9b-I4XROIJhkIU&si=HLfPdTSO4VUKaaR-
* The Value of Values talk by Rich Hickey: https://youtu.be/-6BsiVyC1kM?si=D_Zv1W7ySNu3dpDW
  * Slides and trascript: https://github.com/matthiasn/talk-transcripts/blob/master/Hickey_Rich/ValueOfValues.md
* CS 51, Programming Well: https://book.cs51.io/pdfs/abstraction.pdf
  
Expressions (a value is an expression that does need any further evaluation)

Interesting way to introduce recursion, well it's not really but we are kind of defining `b` in terms of `a` so the outer scope value is called in the inner scope:
```ocaml
utop # let a = 2 in (let b = a in a + b);;
- : int = 4
```
Which is the same as:
```ocaml
utop # let a = 2 in a + a;;
- : int = 4
```


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





