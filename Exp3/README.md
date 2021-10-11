# Experiment 4

Construct a recursive descent parser for an expression according to the grammar below.
E → TE’
E’ → +TE’/- TE’/ε
T → FT’
T’ → *FT’/ /FT’/ ε
F → (E) / id




# Input format

Enter the productions: 10

E=TR        //E' is represented using R
R=+TR
R=-TR
R=#
T=FY        //T' is represented using Y
Y=*FY
Y=/FY
Y=#
F=(E)
F=i         //id is represented using i




# Output format


First(E) = { (, i, }

 First(R) = { +, -, #, }

 First(T) = { (, i, }

 First(Y) = { *, /, #, }

 First(F) = { (, i, }

-----------------------------------------------

 Follow(E) = { $, ),  }

 Follow(R) = { $, ),  }

 Follow(T) = { +, -, $, ),  }

 Follow(Y) = { +, -, $, ),  }

 Follow(F) = { *, /, +, -, $, ),  }
