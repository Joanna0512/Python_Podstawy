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
<br>
</ul>

a = [‘a’, ‘b’, ‘c’] \
b = [1,2,3] \
c = list(zip(a, b) = [(‘a’,1), (‘b’,2), (‘c’,3)]
<br>
## SET
<ul>
<li>w przeciwieństwie do list, kolejność elementów w zbiorze nie jest ustalona (ani istotna)</li>
<li>kolejną różnicą jest to, że elementy zbioru nigdy się nie powtarzają - wszystkie elementy są
  unikalne</li>
<li>zbiór tworzymy podając jego elementy rozdzielone przecinkami w nawiasach klamrowych</li>
<li>można też przekształcić listę w zbiór i ponownie zbiór na listę. Jest to najprostszy sposób na
  usunięcie duplikatów z listy</li>
</ul>
 <br>
  
<b> WYRAŻENIA SET \
</b>UWAGA! Zmiana nawiasu kwadratowego na klamrowy\
name_list = ['ala', 'kasia', 'zenek', 'norbet']\
name_lenght = {len(word) for word in name_list}\
name_lenght = {3, 5, 6}\
<br>
## SŁOWNIK DICT
słownik udostępnia trzy ważne metody:
- keys - zwraca zbiór wszystkich kluczy
- values - zwraca zbiór wszystkich wartości
- items - zwraca zbiór wszystkich par (klucz,
wartość)\
Należy pamiętać, że kiedy iterujemy po słowniku w pętli for to każdy kolejny element jest kluczem, a nie parą (klucz, wartość)\



