3/22

## Lexical and Syntax Analysis

### syntax analysis

* lexical analyzer - low-level
* syntax analyzer \( parser \) - high-level

-

* 為什麼要將Lexical 和 Syntax analysis 分開進行
  * Simplicity
  * Efficiency
  * Portability

#### Lexical Analysis

lexemes -&gt; tokens

* table-drive
* state \(transition\) diagram
  * finitie automata
  * recognize regular language
  * ![](/assets/state-diagram.png)
* state + table-driven 

-

lexical analysis 實用的工具

* getChar
* addChar
* getNonBlank
* lookup

---

### Parser

* purpose
  * 找到syntax error，提供錯誤訊息
  * 為syntactically coreect progrm 建立parsing tree，或trace parsing tree

-

* 兩種形式的parser
  * top-down parser
  * bottom-up parser

-

* grammar 的 notation
  * terminal symbols \( lexemes \)
    * a,b,....
  * nonterminal symbols \( abstractions \)
    * A,B,...
  * Termianls or nontermianls
    * W,X,Y,Z
  * strings or termianls \( sentence \)
    * w,x,y,z

-

* problem
  * Top-down parsers
    * LL parsers
    * implementation
      * Recursive descent parser
      * table driven
  * Bottom-up parsers
    * LR family
  * Complexity of parsing
    * O\($$x = y$$\), when parser works for ambiguous

#### Recursive-Descent Parsing

##### Top Down

* disjoint
  * left factoring

##### Bottom up



