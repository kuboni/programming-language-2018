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

#### Semantics

##### Static Semantics

* type checking, declaration... 等等的辨識 用 BNF 會太大 -&gt; context-sensitive 

-

* Attribute Grammars
  * CFG + Attributes + Attribute computation functions + predicate function
  * Def : G = \(S, N, T, P\)
  * type
    * synthesized
    * inherited
  * e.g.

##### Dynamic Semantics

* Operational Semantics
  * 描述機器狀態的變化
  * Natural operational semantics: 只看結果
  * Structural operational semantics: 除結果外也關心過程
* Denotational Semantics
  * 對應域與值域
  * 以數學式表示Semantics
* Axiomatic Semantics
  * 執行前後的狀態
  * Precondition\(P\), Postcondition\(Q\)
  * inference rule
  * e.g.![](/assets/axiomatic.png)
  * 推斷程式的正確性（驗證）



