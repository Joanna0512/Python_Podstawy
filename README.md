# Python_Podstawy
## Kurs SDA
<br>

<b>WYRAŻENIA LISTOWE \
</b>W wyrażeniu listowym nową listę tworzymy ze starej\
old_list = [1,2,3,4,5,6]\
new_list = [x**2 for x in old_list if not x%2]\
new_list = [4,16,36]\
x%2 = nieparzysta \
<br>
## OPERACJE NA LISTACH
![image](https://user-images.githubusercontent.com/110059749/225616322-d70ffdeb-135f-4d6f-a320-78ea510a2dc4.png)

<b>list.pop([i])\
</b>Remove the item at the given position in the list, and return it. If no index is specified, a.pop() removes and returns the last item in the list. 
<br>

<b> FUNKCJA ENUMERATE\
</b> umożliwia iteracje po obiektach, przy jednoczesnej informacji którą iterację wykonujemy \
<br>
for imie in enumerate(imiona):\
    print(imie)\
(0, 'a')\
(1, 'b')\
jeśli dodam dodatkowy parament np. count wyprinuje się następujacy wynik:\
<br>
for count, imie in enumerate(imiona):\
    print(count, imie)\
0, a\
1, b
## STRINGI
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

## TOUPLE
<br>
Krotka (ang. tuple) jest niezmienną listą. Zawartość krotki określamy tylko podczas jej tworzenia. Potem nie możemy już jej zmienić.\

![image](https://user-images.githubusercontent.com/110059749/225631428-943d317a-6658-4746-a2dc-3e8deed4708a.png)


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
<li>tworzenie pustego setu: set()</li>
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

![image](https://user-images.githubusercontent.com/110059749/225618721-8d788534-9199-4326-973f-3f4075c76f2b.png)

## OPERACJE NA PILKACH\  
f = open('file.txt', mode='w')\
f.write ('ala ma psa')\
f.close()

<b>Tryby otwarcia pliku\
</b>○ Funkcja open posiada następujące tryby:\
○ r - tylko do odczytu (domyślny)\
○ w - do zapisu, jeśli plik nie istnieje to zostanie utworzony, jeśli istnieje jego stara zawartość zostanie\
usunięta. UWAGA! jeśli, chcę żeby to co wpisałam się zapisało, muszę zrobić f.close()\
○ x - do tworzenia, operacja nie powiedzie się, jeśli plik już istnieje\
○ a - dopisywanie, jeśli plik nie istnieje to zostanie utworzony, jeśli istnieje to nowa treść zostanie
dopisana\
○ t - tryb tekstowy (domyślny)\
○ b - tryb binarny\
○ + - oznacza, że po otwarciu kursor ustawi się na końcu pliku. Domyślnie ustawia się na początku.\
<br>
x= "hello Joann"\
f.write(x lub "przykładowy tekst")\
f.writelines(jak wyżej)\
<br>
Jeśli nie chcę za każdym razem używać f.close() używamy funkcji “with open”
przykład:\
<br>
with open('file.txt', mode='w') as file_txt:\
  for t in range(100):\
    file_txt.write(f'{t} C\n')\
czyli wydrukuj t(liczby od 0 do 100 i C, \n = nowa linijka\

Drukowanie zawartości pliku:\
file_2 = open('file2.txt', mode='r')\
tekst_z_pliku = file_2.read()\
tekst_z_pliku.split('\n') - każda wartość od nowej linijki\
<br>
p = open('100_pan_tadeusz.txt',mode='r')\
<br>
while(True):\
  line =p.readline()\
  if not line:\
    break\
  print(line)


    
