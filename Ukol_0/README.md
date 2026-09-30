# Úkol 0: Hello World (Ukázkový úkol)

Vítejte u nultého, ukázkového úkolu! 

Cílem tohoto úkolu není řešení složitého algoritmického problému, ale **seznámení se s celým procesem vypracování, lokálního testování a odevzdávání úkolů** přes GitHub formou Pull Requestu.

---

## Zadání

Vaším úkolem je upravit funkci `hello_world()` v souboru `hello_world.py` tak, aby vracela přesný řetězec:
```text
Hello world!
```

### Soubor k úpravě:
* `Ukol_0/hello_world.py`

Funkce `hello_world()` aktuálně vrací prázdný řetězec `""`. Upravte její návratovou hodnotu.

---

## Jak fungují testy?

V souboru `test.py` je připraven automatický test pomocí standardní knihovny `unittest`:

```python
import unittest
from hello_world import hello_world

class TestFunkci(unittest.TestCase):
    def test_hello_world(self):
        self.assertEqual(hello_world(), "Hello world!")
```

Tento test zavolá vaši funkci `hello_world()` a porovná její výsledek s očekávaným řetězcem `"Hello world!"`. **Soubor `test.py` nijak neupravujte.**

---

## Lokální testování

Před odevzdáním si vždy lokálně ověřte funkčnost svého řešení. V terminálu přejděte do složky `Ukol_0` a spusťte test:

```shell
cd Ukol_0
python -m unittest test.py
```
*(Na Linuxu/macOS případně použijte `python3 -m unittest test.py`)*

Pokud test projde, uvidíte výstup podobný tomuto:
```text
.
----------------------------------------------------------------------
Ran 1 test in 0.001s

OK
```

---

## Odevzdání úkolu

Jakmile testy lokálně projdou:
1. Vytvořte commit se svým řešením:
   ```shell
   git add hello_world.py
   git commit -m "Reseni Ukol 0"
   ```
2. Nahrajte změny do svého forknutého repozitáře:
   ```shell
   git push origin master
   ```
3. Otevřete **Pull Request** v původním repozitáři podle podrobného návodu v hlavním [README.md](../README.md).
