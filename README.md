This is a calculator created while learning how to make a custom programming language

All numbers and operators are represented as uppercase strings

       2  -> TWO
  
      '+' -> ADD

==NUMBERS==

The language only acknowledges strings representing single-digit integers. Numbers larger

than nine, negatives, and floats need multiple single-digit numbers placed next to each other

      10   -> ONE ZERO
      
      1.0  -> ONE DOT ZERO
      
      -1   -> NEG ONE

==OPERATORS==

The following list shows the recognized operators (as used in Python) and symbols in the language
      '+'   ->  ADD
  
      '-'   ->  SUB
  
      '*'   ->  MUL
  
      '/'   ->  DIV
  
      '//'  ->  FLR
  
      '%'   ->  MOD
  
      '**'  ->  POW
  
      '('   ->  L
  
      ')'   ->  R

==MONOS==
They are probably most similar to statements. Monos will affect the rest of the line, but themselves

don't have a default value.

The first three are placed before what they affect.
  
      RND   -> round              RND TWO FIVE DOT FIVE -> 26
  
      CLG   -> ceiling rounding   CLG TWO FIVE DOT ONE  -> 26
  
      FLR   -> floor rounding     FLR TWO FIVE DOT NINE -> 25

      These can be placed anywhere in the input as long as it precedes a number
  
      ONE ADD CLG TWO DOT ONE -> 1 + ceiling(2.1) -> 4

      SHEQ should be placed at the end of the input
  
      SHEQ  -> SHow EQuation      TWO FIVE DIV SIX SHEQ -> 25/6

==VARIABLES==

Variables can only be represented by lowercase letters and underscores
  
      ONE -> 1
  
      one -> variable name

To assign variables, start the input with the variable name plus the mono 'IS' plus

the value, which can also be an equation
  
      var_one IS ONE                    -> var_one = 1
  
      var_two IS ONE ADD TWO            -> var_two = 3
  
      var_three IS var_one ADD var_two  ->  var_three = 4
