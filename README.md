## Why Julia?
[Julia is fast!](https://julialang.org/benchmarks/)  
[Julia solves two-language problem](https://www.nature.com/articles/d41586-019-02310-3)
(you don't have to make prototype in Matlab/Python/... and then re-code in C/C++)  
[Julia metaprogramming](https://docs.julialang.org/en/v1/manual/metaprogramming/) is cool. For example, the following Julia codes (natural and concise) solve first-order differential equation:
```julia
  using Modia
  @model FirstOrder begin
     x = Variable(start=1)   # start means x(0)
     T = Parameter(0.5)      # Time constant
     u = 2.0                 # Same as Parameter(2.0)
  @equations begin
     T*der(x) + x = u        # der() means time derivative
     end
  end
```

## Julia in Tennessee
### Memphis
[TODO]

## General julia
[Resources on learning Julia](https://julialang.org/learning/)  
[Julia main website](https://julialang.org/)  
[Julia forum](https://discourse.julialang.org/)  
