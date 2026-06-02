---
title: \[Copy\]Funkční požadavky -- HerbDelivery
---

# Funkční požadavky - HerbDelivery

Tento dokument shrnuje funkční požadavky pro aplikaci HerbDelivery -
platformu propojující prodejce bylinek, klienty a poslíčky. Obsah je
rozdělen do kapitol a přehledných bodů.

## 1. Uživatelské účty

-   **Registrace a ověření uživatelů**

    -   Registrace klientů, prodejců a poslíčků

    -   Ověření e-mailu nebo telefonu

    -   Standardní onboarding podobný Wolt

-   **Správa profilu**

    -   Úprava kontaktních údajů

    -   Správa platebních metod

    -   Správa doručovacích adres

    -   Umožňuje rychlé opakované objednávky

## 2. Produkty a nabídka

-   **Přidání produktu**

    -   Název, cena, množství, fotka, popis, kategorie

    -   Podobné jako katalog u Wolt Market

-   **Úprava produktu**

    -   Změna ceny, popisu, fotky nebo množství

-   **Dostupnost produktu / vyprodáno**

    -   Pokud množství = 0 → produkt se označí jako vyprodáno

    -   Klient ho nemůže objednat

    -   Splňuje požadavek na blokaci objednávek při nulovém stavu

## 3. Prohlížení a filtrování

-   **Prohlížení nabídky**

    -   Klient vidí všechny dostupné produkty

-   **Filtrování**

    -   Podle ceny

    -   Podle typu bylinky

    -   Podle vzdálenosti

    -   Podle hodnocení

## 4. Objednávky

-   **Vytvoření objednávky**

    -   Výběr produktu a množství

    -   Zadání doručovací adresy

    -   Možnost přidat poznámku

-   **Platba a escrow**

    -   Platba kartou

    -   Peníze se drží v escrow do potvrzení doručení

## 5. Poslíčci

-   **Automatické přiřazení poslíčka**

    -   Algoritmus bere v úvahu vzdálenost, dostupnost a kapacitu

    -   Poslíček dostane notifikaci

-   **Přijetí nebo odmítnutí úkolu**

    -   Pokud odmítne, systém nabídne úkol dalšímu poslíčkovi

-   **Potvrzení vyzvednutí a doručení**

    -   Poslíček potvrdí vyzvednutí

    -   Klient potvrdí doručení

    -   Možnost foto nebo PIN jako důkaz

## 6. Sledování a notifikace

-   **Sledování objednávky v reálném čase**

    -   Live tracking poslíčka

    -   Odhad času doručení

-   **Notifikace**

    -   Klient: změna stavu objednávky

    -   Poslíček: nová objednávka

    -   Prodejce: poslíček přijel vyzvednout

## 7. Hodnocení a historie

-   **Hodnocení a recenze**

    -   Klient hodnotí prodejce i poslíčka

-   **Historie objednávek a transakcí**

    -   Vidí klient, prodejce, poslíček i administrátor

## 8. Administrace

-   **Řešení sporů a podpora**

    -   Administrátor řeší reklamace, refundy a chyby v doručení

-   **Provize a rozdělení plateb**

    -   Po doručení se peníze rozdělí mezi prodejce, poslíčka a
        platformu

-   **Bezpečnost a ochrana dat**

    -   GDPR

    -   Šifrování

    -   Bezpečné ukládání platebních údajů
