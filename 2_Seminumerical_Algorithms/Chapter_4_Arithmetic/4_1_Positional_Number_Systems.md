### Arithmetic  

## Positional Number Systems  

**It is important to make a thorough study of efficient methods for calculating with numbers, since arithmetic underlines so many computer applications.**  

In  this chapter, we shall analyze algorithms for doing arithmetic operations on many types of quantities, such as "floating point" numbers, extremely large numbers, rational numbers, polynomials, and power series; and we will also discuss related topics such as radix conversion, factoring of numbers, and the evaluation of polynomials.   

THE WAY WE DO ARITHMETIC is intimately related to the way we represent the numbers we deal with.   

Positional notation using base b (or radix b) is defined by the rule  

$$(...a_3a_2a_1a_0.a_{-1}a_{-2}...)_b = ... + a_3b^3 + a_2b^2 + a_1b^1 + a_0 + a_{-1}b^{-1} + a_{-2}b^{-2} + ...$$  

----------------------------------------------------------------------------------------------------  
_In a positional numeral system there can be at most one radix point (the "decimal point" generalized). So if you see two dots/commas in a "base-60 number", almost always they're not radix points - they're separators between sexagesimal digits (because base-60 digits are usually written in groups 0-59)._  

_Separators split the number into base-60 "digits" (each 0-59)._  

_The radix point (if explicitly shown is the one place where powers switch from 60⁰ to 60⁻¹._  

_Common conventions:_  
* Colons (time-style): 2:30:15 = 2 · 60² + 30 · 60¹ + 15 · 60⁰  
It's exactly how hours:minutes:seconds works.  
* Commas or dots as digit separators: 2,30,15 or 2.30.15  
Same idea as colons, they're just grouping symbols: 2,30,15 = 2 · 60² + 30 · 60 + 15  
* Semicolon as the sexagesimal "point": 2;30,15  
A very common math/history convention is: ; → radix point and ,(or :) → digit separators   
Then:  2;30,15 = 2 + 30/60 + 16/60²   

----------------------------------------------------------------------------------------------------   

The simplest generalizations of the decimal number system are obtained when we take _b_ to be an integer greater than 1 and when we require the _a_'s to be integers in the range $0 \leqslat a_k < b.$ This gives us the standard binary (b=2), ternary (b=3), quanternary (b=4), quinary(b=5), ... number systems.  

In general, **we could take b to be any nonzero number, and we could choose the a's from any specified set of numbers.**   

The dot that appears between $a_0$ and $a_{-1}$ is called the _radix point_. When $b = 10$ , it is also called the decimal point, and when $b = 2$ , it is sometimes called the binary point, etc. Continental Europeans often use a comma instead of a dot to denote the radix point; the English formerly used a raised dot.   

The _a_'s  are called the _digits_ of the representation. A digit $a_k$ for large _k_ is often said to be "more significant" than the digits $a_k$ for small _k_; accordingly, the leftmost difit is referred to as the _most significant digit_ and the rightmost the _least significant digit_. In the standardbinary system the binary digits are often called _bits_.   

---------------------------------------------------------------------------------------------------   

A **shannon (Sh)** is a **unit of information / entropy**: it's what you get when you measure information with **log base 2**. In that unit, an event with probability $p$ has information content  
```math  
I = -log_2(p) shannons.  
```   
In particular, an event with $p = \frac{1}{2}$ has $I = 1$ shannon.  

A **bit** is often used in two different ways:  
1. a **binary digit / storage symbol** (0 or 1)  
2. a **unit of information** ("bits of information"), i.e. the same unit as above when using $log_2$.  

The whole point of the term **shannon** is to reduce this ambiguity: "n bits stored" vs "n shannons of information".   

**1 shannon = 1 bit (of information)**  

However, people rarely say "shannon" in practice; they usually just say "bits", even in information theory.   
---------------------------------------------------------------------------------------------------- 
