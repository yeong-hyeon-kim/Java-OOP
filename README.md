# π Java OPP(Object Oriented Programming)

* κ°μ²΄μ§ν₯μ νΉμ±μΈ μΆμν, λ€νμ±, μμ, μλμ±μ κ°λκ³Ό μ¬μ© μ΄μ λ₯Ό μμλ΄λλ€.

## π·οΈ λͺ©μ°¨(Index)

1. [μΊ‘μν (Encapsulation)](#μΊ‘μν-(Encapsulation))
2. [μΆμν (Abstraction)](#μΆμν-(Abstraction))
3. [μμμ± (Inheritance)](#μμμ±-(Inheritance))
4. [λ€νμ± (Polymorphism)](#λ€νμ±-(Polymorphism))

### μΊ‘μν (Encapsulation)

* [μΈν°νμ΄μ€(Interface)]("")
  * μλν(Hiding) : κ³΅ν΅λ νΉμ§(νμ)λ§ μ μΈνκ³  κ΅¬μ²΄μ μΈ λ΄μ©μ κ° ν΄λμ€μμ κ΅¬μ²΄ννλλ‘ μ λν©λλ€.
  * λμ¨ν κ²°ν©(Loose Coupling) : νμ νμμΈ κ° ν΄λμ€λ€μ μμ νμμΈ μΈν°νμ΄μ€ νμμ ν¬ν¨λμ΄ μΈν°νμ΄μ€λ₯Ό μμνλ ν΄λμ€λΌλ©΄ νμμ κ΄κ³μμ΄ λ§€κ°λ³μλ‘ λ°μ μ μμ΅λλ€.
    > λ§€κ°λ³μ νμμ΄ νΉμ  ν΄λμ€ νμμ΄ μλλ―λ‘ μμ‘΄μ±μ΄ μ€μ΄λ­λλ€.
* μμ±(Property)
  * `get`, `set`μ μ΄μ©νμ¬ μΈλΆμμ λ°μ΄ν° μ κ·Ό μμ€μ μ§μ ν  μ μμ΅λλ€.
  * κ°μ μΊ‘μν(μλ) ν  μ μμ΅λλ€.

### μΆμν (Abstraction)

* [μΆμ ν΄λμ€, λ©μλ]("")
  * λΈνΈλΆ, μ€λ§νΈν° λͺ¨λ μ»΄ν¨ν°(Computer)λΌκ³  μΌλ°ν(Generalization) ν  μ μλκ² μΆμνμλλ€.
  * ν΄λμ€κ°μ κ³΅ν΅μ μ μ°Ύμλ΄μ κ³΅ν΅μ μ‘°μμ λ§λλ μμμλλ€.
    > λΈνΈλΆ, μ€λ§νΈν°μ κ³΅ν΅ μ‘°μμ μ»΄ν¨ν°μλλ€.
* [μΈν°νμ΄μ€]("")
  * νΉμ  ν΄λμ€κ° κ°μ§λ μμ‘΄μ±μ μΈν°νμ΄μ€λ‘ μ κ±°ν¨μΌλ‘μ¨ μ½λ μ μ°μ±μ λμΌμ μμ΅λλ€.
  * μΈν°νμ΄μ€λ μμ μ΄ μ μν λ©μλκ° μΈν°νμ΄μ€λ₯Ό μμνλ ν΄λμ€μ λ¬΄μ‘°κ±΄ μ‘΄μ¬νλ€λ κ²μ λ³΄μ₯ν©λλ€.
    > ν΄λμ€κ° μΈν°νμ΄μ€λ₯Ό μμλ°μΌλ©΄ κ΅¬ννλ κ±Έ κ°μ νκΈ° λλ¬Έμλλ€.
* [μμ‘΄μ± μ£Όμ(Dependency Injection)]("")
  * μμ‘΄κ΄κ³?
    * Aκ° Bλ₯Ό μμ‘΄νλ€.
    * ν΄λμ€(`A`)κ° νΉμ  ν΄λμ€(`B`) νμμ μ¬μ©νκ³  μμ΅λλ€.
  * λ¬Έμ μ 
    * μΈλΆ ν΄λμ€(`A`)μμ νΉμ  ν΄λμ€(`B`)μ λ©μλ(`M1`)λ₯Ό μ¬μ©νκ³  μμλ ν΄λμ€(`B`)λ₯Ό ν΄λμ€(`C`)λ‘ λ³κ²½νλ©΄ ν΄λμ€(`C`)μ λ©μλ(`M1`) μλ€λ©΄ λμ΄μ λ©μλ(`M1`)λ₯Ό μ¬μ©ν  μ μμ΅λλ€.
  * ν΄κ²°λ°©μ
    * κ³΅ν΅ μμ νμ : [μΈν°νμ΄μ€(Interface)]("")λ₯Ό μμλ°μ `"Aκ° Bλ₯Ό μμ‘΄νλ€."`λ λͺμ λ₯Ό `"Aμ Bλ μΈν°νμ΄μ€λ₯Ό μμ‘΄νλ€."`λ‘ λ°κΏ μμ‘΄μ±μ μ€μΌ μ μμ΅λλ€.
    * λ©μλ(`M1`)λ₯Ό μ μν μΈν°νμ΄μ€λ₯Ό μμνλ ν΄λμ€λΌλ©΄ λ¬΄μ‘°κ±΄ λ©μλ(`M1`)λ₯Ό κ΅¬ν(μ¬μ μ)νλ―λ‘ ν΄λμ€κ° λ³κ²½λμ΄λ μ½λλ₯Ό μμ ν  νμκ° μμ΅λλ€.

### μμμ± (Inheritance)

* [νμ ν΄λμ€]("")
  * μμ ν΄λμ€(κ³΅ν΅ μ‘°μ)λ₯Ό μμλ°μ νμ ν΄λμ€(μμ )μ κ΅¬ν(κ΅¬μ²΄ν, μ¬μ μ), νμ₯νλ μμμλλ€.
  > μ»΄ν¨ν°λ₯Ό λΈνΈλΆ λλ μ€λ§νΈν°μΌλ‘ κ΅¬μ²΄νν  μ μμ΅λλ€.

### λ€νμ± (Polymorphism)

* [μ€λ²λΌμ΄λ(Override)]("")
  * μμ ν΄λμ€μ ν¨μλ λ©μλλ₯Ό μ¬μ μ νλ κ²μ μλ―Έν©λλ€.
  * μ΄λ¦κ³Ό λ§€κ° λ³μλ λμΌνλ κ΅¬μ²΄μ μΈ λ΄μ©μ μ¬μ μ ν©λλ€.

* [μ€λ²λ‘λ©(Overloading)]("")
  * λμΌν μ΄λ¦μ λ§€κ° λ³μλ§ λ€λ₯Έ μ¬λ¬ λ²μ μ λ§λλ κ²μ μλ―Έν©λλ€.
  * μ΄λ¦μ΄ κ°κ³  λ§€κ° λ³μμ κ°μλ νμμ΄ λ¬λΌμΌ ν©λλ€.

* μμ ν΄λμ€ λ©μλλ₯Ό `λ€`μν `ν`νλ‘ μ΄μ©ν  μ μλ `μ±`μ§.
  > λ€μν ννλ‘ μ΄μ©ν  μ μλ μ±μ§ > λ€νμ±
