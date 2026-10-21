# 🐍 Python Cheatsheet: Základy pro začátečníky

---

## 1. Proměnné a základní datové typy

```python
# Datové typy
cislo = 10                  # int (celé číslo)
desetinne = 3.14            # float (desetinné číslo)
text = "Ahoj světe!"        # str (řetězec)
pravda = True               # bool (Pravda / Nepravda: True, False)

# Výpis do konzole
print(text)
print(f"Číslo je: {cislo}")  # f-string (pohodlné formátování)
```

---

## 2. Podmínky (`if`, `elif`, `else`)

```python
vek = 18

if vek >= 18:
    print("Jsi dospělý.")
elif vek >= 15:
    print("Máš občanku.")
else:
    print("Jsi ještě dítě.")

# Ternární operátor (jednorádkový if)
status = "Plnoletý" if vek >= 18 else "Mladistvý"
```

### Logické operátory
- `and` – platí obě podmínky zároveň (`x > 0 and x < 10`)
- `or` – platí alespoň jedna podmínka (`x == 1 or x == 2`)
- `not` – negace podmínky (`not True` je `False`)

---

## 3. Cykly

### Cyklus `for` (všechny hlavní formy zápisu)

```python
# 1. Procházení rozsahu čísel: range(stop) -> 0 až 4
for i in range(5):
    print(i)

# 2. Rozsah s počátkem a koncem: range(start, stop) -> 1 až 5
for i in range(1, 6):
    print(i)

# 3. Rozsah s krokem: range(start, stop, step) -> 0, 2, 4, 6, 8
for i in range(0, 10, 2):
    print(i)

# 4. Záporný krok (zpětné odpočítávání) -> 5, 4, 3, 2, 1
for i in range(5, 0, -1):
    print(i)

# 5. Procházení prvků seznamu (listu)
ovorce = ["jablko", "banán", "pomeranč"]
for ovoce in ovorce:
    print(ovoce)

# 6. Procházení prvků i s indexem (enumerate)
for index, ovoce in enumerate(ovorce):
    print(f"{index}: {ovoce}")

# 7. Jednorádkový for cyklus (List Comprehension)
ctverce = [x**2 for x in range(5)]  # [0, 1, 4, 9, 16]
```

### Cyklus `while`

```python
pocitadlo = 0

# Běží, dokud platí podmínka
while pocitadlo < 3:
    print(pocitadlo)
    pocitadlo += 1  # Stejné jako: pocitadlo = pocitadlo + 1

# Řízení cyklů
while True:
    # break – okamžitě ukončí cyklus
    break

for i in range(10):
    if i % 2 == 0:
        continue  # přeskočí zbytek těla cyklu a jde na další krok
    print(i)
```

---

## 4. Seznamy (Listy)

```python
# Vytvoření listu
prvky = [10, 20, 30, 40, 50]

# Přístup k prvkům (indexuje se od 0)
print(prvky[0])    # 10 (první prvek)
print(prvky[-1])   # 50 (poslední prvek)

# Slicing (výřezy): [start:stop:krok]
print(prvky[1:4])  # [20, 30, 40]
print(prvky[:2])   # [10, 20]
print(prvky[:: -1])# Obrané pořadí: [50, 40, 30, 20, 10]

# Úprava a přidávání
prvky.append(60)       # Přidá prvek na konec
prvky.insert(0, 5)     # Vloží prvek na index 0
prvky.remove(30)       # Odstraní první výskyt hodnoty 30
vymazany = prvky.pop() # Odstraní a vrátí poslední prvek

# Užitečné funkce
dlouzka = len(prvky)   # Počet prvků
prvky.sort()           # Seřadí vzestupně
```

---

## 5. Funkce

```python
# 1. Základní funkce bez parametrů
def pozdrav():
    print("Ahoj!")

pozdrav()

# 2. Funkce s parametry a návratovou hodnotou (return)
def secti(a, b):
    return a + b

vysledek = secti(5, 3)  # 8

# 3. Funkce s výchozím parametrem (default argument)
def privitej(jmeno="hoste"):
    print(f"Vítej, {jmeno}!")

privitej()          # Vítej, hoste!
privitej("Petře")   # Vítej, Petře!

# 4. Lambda (anonymní jednorádková funkce)
dvojnasobek = lambda x: x * 2
print(dvojnasobek(4))  # 8
```

---

## 6. Další užitečné datové struktury

```python
# Slovník (Dictionary) - dvojice klíč: hodnota
osoba = {"jmeno": "Jan", "vek": 25}
print(osoba["jmeno"])

# Množina (Set) - pouze unikátní hodnoty
unikatni = {1, 2, 2, 3}  # Uloží se jako {1, 2, 3}
```