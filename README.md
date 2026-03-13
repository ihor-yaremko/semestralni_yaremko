# semestralni_yaremko
## Movie Watch Tracker

Konzolová aplikace pro evidenci sledovaných filmů.

Uživatel může:
- přidávat filmy
- hodnotit filmy
- vyhledávat filmy
- třídit filmy podle různých parametrů
- ukládat data do souborů

---

# Zadání práce

Cílem práce je vytvořit konzolovou aplikaci v jazyce **Java**, která umožní evidenci sledovaných filmů.

Aplikace umožní:

- ukládání filmů
- přidávání hodnocení
- vyhledávání filmů
- třídění filmů
- práci se soubory

Program bude pracovat s **textovými i binárními soubory** a bude využívat principy **objektově orientovaného programování**.

---

# Motivace

Vybral jsem si toto téma, protože sledování filmů je populární aktivita a mnoho lidí sleduje velké množství filmů.

Často však nemají přehled o tom:

- jaké filmy již viděli
- jaké hodnocení jim dali
- kdy film sledovali
- jakého je film žánru

Tato aplikace umožní vytvořit jednoduchou evidenci sledovaných filmů.

---

# Popis problému

Uživatelé často sledují velké množství filmů, ale nemají jednoduchý nástroj, který by jim umožnil evidovat tyto informace.

Navrhovaná aplikace umožní:

- evidovat sledované filmy
- ukládat jejich hodnocení
- zobrazovat seznam filmů
- vyhledávat filmy
- třídit filmy podle různých parametrů
- ukládat data do souborů

Program bude ovládán pomocí konzolového menu.

---

# Řešení

Aplikace bude rozdělena do několika balíčků:

- **ui** – uživatelské rozhraní
- **app** – logika aplikace
- **utils** – pomocné třídy

Program bude využívat:

- Java Collections Framework
- Java Time API
- regulární výrazy
- vlastní výjimky
- enum typy

---

# Funkční specifikace

## 1. Správa filmů
1. Přidat film  
2. Zobrazit všechny filmy  
3. Smazat film  

## 2. Hodnocení filmů
1. Přidat hodnocení  
2. Zobrazit nejlépe hodnocené filmy  

## 3. Třídění filmů
1. Třídit podle názvu  
2. Třídit podle hodnocení  
3. Třídit podle data sledování  

## 4. Vyhledávání
1. Vyhledat film podle názvu  

## 5. Export dat
1. Uložit data do textového souboru  
2. Uložit data do binárního souboru  

## 0. Konec programu

Program obsahuje **víceúrovňové menu**, které umožňuje opakovaný výběr funkcí.

---

# Datový model

## Třída `Movie`

| Atribut | Datový typ | Popis |
|-------|-------|------|
| id | int | identifikátor filmu |
| title | String | název filmu |
| genre | Genre | žánr filmu |
| rating | int | hodnocení filmu (1–10) |
| watchDate | LocalDate | datum sledování |
