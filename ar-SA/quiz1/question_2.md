
--- question ---

---
القائمة: السؤال 2 من 3
---

إليك المقطع البرمجي للغز العجلة اليدوية:

```blocks3
when flag clicked
set [turned v] to (0)
set [handwheel turned v] to (0)
repeat until <(handwheel turned) > (2)>
end
say [task complete] for (2) seconds
```

أي سطر من المقطع البرمجي ستضيفه إلى المقطع البرمجي لإخبار الشخصية بعدد المرات التي أدارت فيها العجلة ، باستخدام جملة كاملة؟

--- choices ---

- (x)

```blocks3
say (join [handwheel turned ] (join (handwheel turned) [ times])
```

  --- feedback ---

نعم ، إذا تم تدوير العجلة اليدوية 3 مرات ، فستظهر عدم دوران العجلة اليدوية</code>`: class = 'block3looks'}</p>

<p spaces-before="2">--- /feedback ---</p>

<ul>
<li>( )</li>
</ul>

<pre><code class="blocks3">say (join [handwheel turned ]  [ times])
`</pre>

  --- feedback ---

باستخدام هذا المقطع البرمجي ، إذا تم تدوير العجلة اليدوية 3 مرات ، فستقول إن `عجلة يدوية تحولت مرة`{: class = 'block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (join (handwheel turned)(join [handwheel turned ] [times])
```

  --- feedback ---

باستخدام هذا المقطع البرمجي ، إذا تم تدوير العجلة اليدوية 3 مرات ، فستقول `3 تحولت العجلة اليدوية مرة`{: class = 'block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (handwheel turned)
```
  --- feedback ---

باستخدام هذا المقطع البرمجي ، إذا تم تدوير العجلة اليدوية 3 مرات ، فستقول `3`{: class = 'block3looks'}

  --- /feedback ---

--- /choices ---

--- /question ---
