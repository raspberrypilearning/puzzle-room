
--- question ---

---
legend: Ερώτηση 3 από 3
---

Κοίταξε τα μπλοκ παρακάτω. Ποια περιγραφή περιγράφει καλύτερα τη συμπεριφορά του αντικειμένου βράχου, όταν πατηθεί η σημαία;


![αντικείμενο βράχου](images/rocks-sprite.png)
```blocks3
when flag clicked
go to (random position v)
repeat until <<touching (sprite 1 v) ?> and <not<touching color (#000000) ?>>
go to (random position v)
```

--- choices ---

- ( )

Το αντικείμενο rocks θα μετακινηθεί σε μια τυχαία θέση μέχρι να αγγίξει το **αντικείμενο 1** και να αγγίξει το μαύρο χρώμα.

  --- feedback ---

Αυτά τα μπλοκ θα ταίριαζαν σε αυτήν την περιγραφή. <touching (sprite 1 v) ?> και <touching color (#000000) ?>

  --- /feedback ---

- ( )

Το αντικείμενο rocks θα μετακινηθεί σε μια τυχαία θέση μέχρι να αγγίξει το **αντικείμενο 1** ή να μην αγγίξει το μαύρο χρώμα.

  --- feedback ---

<touching (sprite 1 v) ?> ή <όχι<touching color (#FFFFFF) ?>

  --- /feedback ---

- (x)

Το αντικείμενο rocks θα μετακινηθεί σε μια τυχαία θέση μέχρι να αγγίξει το **αντικείμενο 1** και να αγγίξει οποιοδήποτε χρώμα εκτός από το μαύρο.

  --- feedback ---

Ναι, αυτό είναι σωστό. Το μπλοκ `όχι`{:class='block3operators'} ελέγχει ότι δεν αγγίζει μαύρο.

  --- /feedback ---

- ( )

Το αντικείμενο rocks θα μετακινηθεί σε μια τυχαία θέση μέχρι να μην αγγίζει το **αντικείμενο 1** και ή το μαύρο χρώμα.

  --- feedback ---

<not<touching (sprite 1 v) ?>> or <touching color (#000000) ?>

  --- /feedback ---

--- /choices ---

--- /question ---