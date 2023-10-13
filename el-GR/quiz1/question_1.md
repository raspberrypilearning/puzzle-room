## Γρήγορο κουίζ

Απάντησε στις τρεις ερωτήσεις. Υπάρχουν συμβουλές που θα σε καθοδηγήσουν στη σωστή απάντηση.

Όταν έχεις απαντήσει σε κάθε ερώτηση, κάνε κλικ στο **Έλεγξε την απάντησή μου**.

Διασκέδασέ το!

--- question ---

---
legend: Ερώτηση 1 από 3
---

Εδώ είναι ο χαρακτήρας Monet δίπλα σε ένα μεγάλο κουμπί:

![ο χαρακτήρας Monet που στέκεται δίπλα σε ένα μεγάλο κόκκινο κουμπί](images/monet-by-button.png)

Ποια μπλοκ θα χρησιμοποιούσες, ώστε ο αριθμός των πατημάτων των κουμπιών να εμφανίζεται συνεχώς, μέχρι να πατηθεί το κουμπί συνολικά 7 φορές;


--- choices ---

- ( )

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat until <(button pressed) = (5)>
say (button pressed)
end
say [task complete] for (2) seconds
```

  --- feedback ---

Το script σου λέει τον αριθμό των πατημάτων κουμπιών, ωστόσο σταματά μετά από μόνο 5 πατήματα κουμπιών.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
set [button pressed v] to (0)
if <(button pressed) > (6)> then
say (button pressed)
end
say [task complete] for (2) seconds
```

  --- feedback ---

Αυτά τα μπλοκ θα τρέξουν μόνο μία φορά στην αρχή του παιχνιδιού, καθώς δεν χρησιμοποιείται βρόχος.

  --- /feedback ---

- (x)

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat until <(button pressed) > (6)>
say (button pressed)
end
say [task complete] for (2) seconds
```

  --- feedback ---

Ναι! Αυτό το script λέει πόσες φορές έχει πατηθεί το κουμπί κάθε φορά και λέει ότι η εργασία ολοκληρώθηκε μετά από 7 πατήματα κουμπιών.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat (7)
say (button pressed)
end
say [task complete)] for (2) seconds
```
  --- feedback ---

Αυτά τα μπλοκ θα έλεγαν τον αριθμό `0` επτά φορές πολύ γρήγορα στην αρχή του παιχνιδιού, καθώς δεν υπάρχει συνθήκη που να ελέγχει την τιμή της μεταβλητής.

  --- /feedback ---

--- /choices ---

--- /question ---
