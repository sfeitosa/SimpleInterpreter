# SimpleInterpreter
Interpretador de Exemplo -- PLP2020

# Gerando o Parser

```
happy Parser.y
```

# Executando o Interpreter

```
runghc Interpreter.hs
2 + 4 <enter>
<CTRL + D>
``` 
 
Vai apresentar o resultado: 

```
Just (Num 6)
```

