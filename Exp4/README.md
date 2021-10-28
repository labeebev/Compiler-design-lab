# Experiment 4

Write program to find First and Follow of any given grammar.

Eg.

Grammar
E → E + T | T
T → T * F | F
F → (E) | id




# Input format

Enter the productions: 6

E=E+T
E=T
T=T*F
T=F
F=(E)
F=i


# Output format


First(E) = { (, i, }

 First(T) = { (, i, }

 First(F) = { (, i, }

-----------------------------------------------

 Follow(E) = { $, +, ),  }

 Follow(T) = { $, +, ), *,  }

 Follow(F) = { $, +, ), *,  }
 
