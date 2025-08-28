# calculate_shelves
**This is a small C++ program with a linear function I came up with myself.**<br>
I wanted it to be simple for the beginning...<br>
and hopefully improve it sometime...

**The Exercise I came up with, for myself:**<br>
How much shelves do I need, at least, for my Bookshelf with the amount of my current books.

At first, to keep it really simple so I make as less as possible wrong,<br>
I came up with 1 book pro shelve.

After that I came up with the variable names. Where I struggled the most at :(

Variable's:
1) Bookshelf row's --> **r**
2) number of vertical shelf levels --> **s**
3) missing books --> **m**

with those I came up with this function: **[ rs - m ]**

so that if r = 3, s = 2 and m = 0.<br>
you have an result of 6, what would mean with 1 book pro shelve my bookshelf would be completly full.<br>
And if r = 3, s = 2 and m = 1.<br>
that would mean 1 book missing results in 1 shelve missing. So **m** can't be right and needs to be updated or removed.<br>
I decide to keep it simple and removed it, so I can decide later how to proberly remove missing books.<br>
--> **[ rs ]**

Then I changed **r**, cause<br>
--> **[ r = max. numbers of book width in cm  / max. bookshelf width in cm ]**<br>
--------> max. numbers of book width = w(lower B) = wB<br>
--------> max. bookshelf width = w(lower Bs) = wBs<br>
--> **[ r = wB / wBs ]**<br>
So in this case involving the amount of books, I have more than 1 possible book pro shelve.<br>
So I changed <r = Bookshelf row's> from above, cause it doesn't make sense anymore, to <a = amount of shelf's needed>.<br>
--> **[ a = wB / wBs ]**

Final result: **[ a = wB / wBs ]**

Note: a = ( wie viele "kästchen" in abhängigkeit zur breite des regals nötig sind bei n anzahl von Büchern )
