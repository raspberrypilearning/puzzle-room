
--- question ---

---
legend: Pergunta 3 de 3
---

Observe os blocos abaixo. Qual opção melhor descreve o comportamento do ator "Asteróides" quando a bandeira é clicada?


![ator "Asteróides"](images/rocks-sprite.png)
```blocks3
when flag clicked
go to (posição aleatória v)
repeat until <<touching (ator 1 v) ?> and <not<touching color (#000000) ?>>
go to (posição aleatória v)
```

--- choices ---

- ( )

O atro "Asteróides" se moverá para uma posição aleatória até tocar **ator 1** e tocar a cor preta.

  --- feedback ---

Esses blocos se encaixariam nessa descrição. <touching (ator 1 v) ?> e <touching color (#000000) ?>

  --- /feedback ---

- ( )

O ator "Asteróides" se moverá para uma posição aleatória até tocar **ator 1** ou não tocar na cor preta.

  --- feedback ---

<touching (ator 1 v) ?> ou <não<touching color (#FFFFFF) ?>

  --- /feedback ---

- (x)

O ator "Asteróides" se moverá para uma posição aleatória até tocar **ator 1** e tocar qualquer cor diferente de preto.

  --- feedback ---

Sim, está correto. O bloco `não`{:class='block3operators'} verifica se não está tocando o preto.

  --- /feedback ---

- ( )

O ator "Asteróides" se moverá para uma posição aleatória até que não toque no **ator 1** ou na cor preta.

  --- feedback ---

<not<touching (ator 1 v) ?>> or <touching color (#000000) ?>

  --- /feedback ---

--- /choices ---

--- /question ---
