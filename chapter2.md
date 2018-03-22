3/15

## Syntax and Semantics

1. lexical analyzer \[ lexical unit \]
2. Syntax analyzer \[ parsing tree \]
3. Semantic analyzer \[ intermediate code \]
4. \(optimzation\)
5. code generator

#### Terminology

* lexeme \( word \)

* token = lexeme type

  * e.g. identifier, init\_literal, plus\_op ...

* sentence = lexeme + lexeme + ...

* language = sentence + sentence + ...

#### Language

* Generators
* Recognizers

##### Regular Language

M = \(Q, Σ, δ, q0, F\)

#### Grammar

* Context-Free Grammar, CFG
* Backus-Naur Form, BNF
  * metalanguage - 描述語言的語言
  * abstraction
    * non-terminal symbol
    * terminal symbol
* Derivation
  * Parse Tree
    * ambiguity
    * Associativity \(+\) - overflow
* Extended BNF \(EBNF\)

  * optional parts

  * altermative parts

  * repetitions

#### Static Semantics

* type checking, declaration... 等等的辨識 用 BNF 會太大 -&gt; context-sensitive 



