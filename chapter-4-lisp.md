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

#### Quote

* quote
* '
* 避免compiler將 \( ambiguous

-

## 語法

assign data

### setq

* setquote
* \(setq \[name\] \[value\]\)

### let

* 一次assign 多個變數
* 其中變數為local

### value

* \(values :this :that\)

* 多重賦值

--

FUNCTION

#### lambda

* 沒辦法被 reuse

#### defun

* \(defun \[function\_name\] \[parameters\] \[operand\]\)

--

CONDITION

##### boolean value

* T
* NIL

=&gt; predicate

\(numberp x\)

\(stringp x\)

\(listp x\)

\(symbolp x\)

\(atom x\)

\(null x\)

##### IF

##### cond



