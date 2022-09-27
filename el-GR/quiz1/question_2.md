
--- question ---

---
legend: Ερώτηση 2 από 3
---

Ακολουθεί ένα script για έναν γρίφο χειροτροχό:

```blocks3
when flag clicked
set [turned v] to (0)
set [handwheel turned v] to (0)
repeat until <(handwheel turned) > (2)>
end
say [task complete] for (2) seconds
```

Ποια γραμμή κώδικα θα πρόσθετες στο script για να πεις στον χαρακτήρα πόσες φορές έχει γυρίσει τον τροχό, χρησιμοποιώντας μια πλήρη πρόταση;

--- choices ---

- (x)

```blocks3
say (join [handwheel turned ] (join (handwheel turned) [ times])
```

  --- feedback ---

Ναι, αν ο χειροτροχός είχε περιστραφεί 3 φορές θα έλεγε `χειροτροχός γυρισμένος 3 φορές`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (join [handwheel turned ]  [ times])
```

  --- feedback ---

Με αυτό το script, αν ο χειροτροχός είχε περιστραφεί 3 φορές θα έλεγε `χειροτροχός γυρισμένος φορές`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (join (handwheel turned)(join [handwheel turned ] [times])
```

  --- feedback ---

Με αυτό το script, αν ο χειροτροχός είχε περιστραφεί 3 φορές θα έλεγε `3 χειροτροχός γυρισμένος φορές`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (handwheel turned)
```
  --- feedback ---

Με αυτό το script, αν ο χειροτροχός είχε περιστραφεί 3 φορές θα έλεγε `3`{:class='block3looks'}

  --- /feedback ---

--- /choices ---

--- /question ---
