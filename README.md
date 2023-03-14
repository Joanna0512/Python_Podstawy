# Python_Podstawy
## Kurs SDA
<br>

<b>WYRAŻENIA LISTOWE \
</b>W wyrażeniu listowym nową listę tworzymy ze starej\
old_list = [1,2,3,4,5,6]\
new_list = [x**2 for x in old_list if not x%2]\
new_list = [4,16,36]\
x%2 = nieparzysta \

<b>STRINGI\
</b>SPLIT - przekształca string w listę, ale split na samej liście już nie da się użyć.\
fruit = "apple,banana,pear"\
fruit.split(',')\
['apple', 'banana', 'pear']\
<br>

fruit = ['apple', 'banana', 'pear']\
''.join(fruit)\
'applebananapear'\
', '.join(fruit)\
<br>

text.lower()  # tekst małymi literami\
text.upper()  # tekst wielkimi literami\
text.capitalize()  # pierwsza litera wielka\
text.title()  # pierwsza litera każdego słowa wielka\
text.swapcase()  # małe litery zamienia na wielkie, wielkie na małe\
text.index(“a”) #wyświetlanie indeksu wskazanego obiektu\
text.find(“a”) # to co indeks\
txt[::-1] - odwrócenie listy\
txt[-2:]+txt[:-2] = zmiana ostatnich pozycji na pierwsze\
txt.replace(“x”, “y”) - zmiana każdego x na y\
x = [*set(txt)] lub list(set(txt) - usuwanie duplikatu ze stringa\
<br>
## ZIP

<ul>

<li>przyjmuje dwie lub więcej listy </li>
<li>zwraca sekwencję krotek, gdzie każdy element krotki pochodzi z innej listy</li>
<li>jeśli funkcje mają różne długości przyjmuje najkrótszą</li>

