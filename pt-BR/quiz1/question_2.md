
--- question ---

---
legend: Pergunta 2 de 3
---

Aqui estão os blocos para o quebra-cabeça da roda-manual:

```blocks3
when flag clicked
set [girada v] to (0)
set [roda-manual girada v] to (0)
repeat until <(roda-manual girada) > (2)>
end
say [tarefa concluída] for (2) seconds
```

Qual bloco de código você adicionaria para dizer ao personagem quantas vezes ele girou a roda-manual, usando uma frase completa?

--- choices ---

- (x)

```blocks3
say (join [roda-manual girada ] (join (roda-manual girada) [ vezes])
```

  --- feedback ---

Sim, se a roda-manual tivesse sido girado 3 vezes, diria `roda-manual girada 3 vezes`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (join [roda-manual girada ]  [ vezes])
```

  --- feedback ---

Com este script, se a roda-manual tivesse sido girada 3 vezes, mostraria `roda-manual girada vezes`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (join (roda-manual girada)(join [roda-manual girada ] [vezes])
```

  --- feedback ---

Com este script, se o volante tivesse sido girado 3 vezes, mostraria `3 vezes a roda-manual girada`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (roda-manual girada)
```
  --- feedback ---

Com este script, se o volante tivesse sido girado 3 vezes, mostraria `3`{:class='block3looks'}

  --- /feedback ---

--- /choices ---

--- /question ---
