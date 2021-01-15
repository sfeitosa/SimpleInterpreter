# PLP2020 - Interpretador de Exemplo

**Gerando o Parser**

O código-fonte *Parser.y* contém as definições aceitas pelo *Happy* para a geração do analisador léxico e sintático. 

Para fazer a geração, basta executar o seguinte comando:

```
happy Parser.y
```

Sempre que adicionar/alterar alguma informações no arquivo *Parser.y*, é preciso executar novamente o comando acima.

Caso o sistema apresente mensagem de erro, informando que o comando *Happy* não existe, é preciso instalá-lo no seu sistema. Para isto, basta executar o comando:

```
stack install happy
```

**Executando o Interpreter**

Para rodar/testar o interpretador desenvolvido, vamos usar o programa ```runghc```, conforme pode ser visto abaixo.

```
stack runghc Interpreter.hs
```

Ao executar este comando, o programa fica aguardando a entrada do usuário, que pode digitar a expressão para ser interpretada. Como exemplo, vamos digitar a expressão ```2 + 4``` e teclar *ENTER*. Para que o resultado seja apresentado, precisamos ainda utilizar as combinações de teclas *CTRL + Z* (*CTRL + D* no Linux). Estes comandos na sequência são apresentados abaixo.

```
2 + 4 <enter>
<CTRL + Z> <enter>
``` 

Realizado este procedimento, o resultado do processamento do interpretador será apresentado na tela.

```
Just (Num 6)
```

Mais detalhes sobre as funções e ajustes necessários para o trabalho final podem ser encontrados em comentários nos arquivos *Parser.y* e *Interpreter.hs*.
