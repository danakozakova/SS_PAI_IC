# Ako si doma rozbehať Python a Jupyter vo VS Code

Tento návod je pre tých, ktorí si chcú prostredie zo školy nainštalovať aj doma. Nie je povinný.

## Čo potrebuješ

1. **Python** — stiahni z [python.org](https://www.python.org/downloads/). Pri inštalácii zaškrtni **Add python.exe to PATH**.
2. **Visual Studio Code** — stiahni z [code.visualstudio.com](https://code.visualstudio.com/).

## Postup

**1. Vytvor priečinok a otvor ho vo VS Code**

Vytvor si priečinok (napr. `IC`). Vo VS Code zvoľ *File → Open Folder* a vyber ho. Vždy pracuj v tomto otvorenom priečinku.

**2. Rozšírenia**

Stlač `Ctrl+Shift+X`, vyhľadaj a nainštaluj **Python** a **Jupyter** (obe od Microsoftu).

**3. Vytvor prostredie (`.venv`)**

Otvor terminál (*Terminal → New Terminal*) a napíš:

```
py -m venv .venv
```

Na macOS/Linuxe: `python3 -m venv .venv`

**4. Nainštaluj `ipykernel`**

```
.venv\Scripts\python -m pip install ipykernel
```

Na macOS/Linuxe: `.venv/bin/python -m pip install ipykernel`

(Ak chceš do prostredia dať aj Kivy, urob to rovnako: `.venv\Scripts\python -m pip install kivy`.)

**5. Vyskúšaj notebook**

1. Vytvor nový súbor `skuska.ipynb` (*File → New File*).
2. Vpravo hore klikni na **Select Kernel → Python Environments** a vyber `.venv`.
3. Do bunky napíš `print("Ahoj")` a stlač `Shift+Enter`.

Ak sa pod bunkou zobrazí `Ahoj`, všetko funguje.

## Keď to nejde

- Nemáš otvorený **priečinok** (pozri krok 1) → `.venv` sa nenájde.
- Nemáš vybraný **kernel** (vpravo hore).
- V `.venv` nie je `ipykernel` (zopakuj krok 4). VS Code ti niekedy sám ponúkne jeho inštaláciu, vtedy súhlas.

## Príkazy na jednom mieste

**Rozšírenia vo VS Code** (to isté ako krok 2, len z terminálu):

```
code --install-extension ms-python.python
code --install-extension ms-toolsai.jupyter
```

**`ipykernel` v prostredí `.venv`:**

```
.venv\Scripts\python -m pip install ipykernel
```

Na macOS/Linuxe: `.venv/bin/python -m pip install ipykernel`

Ak máš prostredie aktivované (v termináli vidíš `(.venv)`), stačí:

```
python -m pip install ipykernel
```
