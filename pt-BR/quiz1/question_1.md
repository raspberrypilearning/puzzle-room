## Teste Rápido

Responda as três perguntas. Existem dicas para guiá-lo para a resposta correta.

Após responder cada pergunta, clique em **Verificar minha resposta**.

Divirta-se!

--- question ---

---
legend: Pergunta 1 de 3
---

Aqui está o personagem Monet próximo a um botão grande:

![personagem Monet ao lado de um grande botão vermelho](images/monet-by-button.png)

Quais blocos você usaria para que fosse exibido o número de vezes em que o botão foi pressionado, até que o botão fosse pressionado um total de 7 vezes?


--- choices ---

- ( )

```blocks3
when flag clicked
set [botão pressionado v] to (0)
repeat until <(botão pressionado) = (5)>
say (botão pressionado)
end
say [tarefa concluída] for (2) seconds
```

  --- feedback ---

Estes blocos exibem o número de vezes em que o botão foi pressionado, mas ele para após o botão ser pressionado 5 vezes.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
set [botão pressionado v] to (0)
if <(botão pressionado) > (6)> then
say (botão pressionado)
end
say [tarefa concluída] for (2) seconds
```

  --- feedback ---

Esses blocos só seriam executados uma vez no início do jogo, já que não há bloco "repita" sendo usado.

  --- /feedback ---

- (x)

```blocks3
when flag clicked
set [botão pressionado v] to (0)
repeat until <(botão pressionado) > (6)>
say (botão pressionado)
end
say [tarefa concluída] for (2) seconds
```

  --- feedback ---

Sim! Esses blocos mostram quantas vezes o botão foi pressionado e diz que a tarefa é concluída após 7 pressionamentos de botão.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
set [botão pressionado v] to (0)
repeat (7)
say (botão pressionado)
end
say [tarefa concluída)] for (2) seconds
```
  --- feedback ---

Esses blocos diriam o número `0` sete vezes muito rapidamente no início do jogo, pois não há bloco "se" para verificar o valor da variável.

  --- /feedback ---

--- /choices ---

--- /question ---
