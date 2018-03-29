## LISP

functional programming

* data type 
  * atoms
  * lists

-

substitution model

\(operator operand1 operand2\)

| C | LISP |
| :--- | :--- |
| 1 + 2 + 3 | \(+ 1 2 3\) |
| 3 + 4 \* 5 | \(+3 \(\* 4 5\)\) |
| factorial\(9\) | \(factorial 9\) |
| \(a==b\)&&\(c!=0\) | \(and\(= a b\)\(not \(= c 0\)\)\) |
| \(low &lt; x\)&&\(x &lt; high\) | \( &lt; low x high\) |
|  |  |
| if\(a==0\) return f\(x,y\) | \(if\(= a 0 |
| else return g\(x,y\) | \(f x y\) |
|  | \(g x y\)\) |

-

Quote

* quote
* '
* 避免compiler將 \( ambiguous


