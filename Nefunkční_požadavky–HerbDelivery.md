---
title: Nefunkční požadavky -- HerbDelivery
---

# Nefunkční požadavky - HerbDelivery

Tento dokument shrnuje nefunkční požadavky systému HerbDelivery. Obsah
je rozdělen do kapitol a přehledných bodů.

## 1. Výkon a dostupnost

-   **Dostupnost systému**

    -   Systém musí být dostupný 24/7

    -   Cílová dostupnost: 99.9 % měsíčně

-   **Výkon a odezva**

    -   API odezva do 300 ms

    -   Načtení stránky do 1 sekundy

-   **Propustnost**

    -   Zpracování minimálně 500 objednávek za minutu

-   **Škálovatelnost**

    -   Systém musí zvládnout 10× nárůst uživatelů a objednávek

## 2. Bezpečnost

-   **Autentizace a ochrana účtů**

    -   Podpora dvoufaktorového ověřování

    -   Bezpečné ukládání hesel (bcrypt/argon2)

-   **Ochrana dat**

    -   Šifrování dat při přenosu (TLS 1.2+)

    -   Šifrování dat v úložišti (AES-256)

-   **Platební bezpečnost**

    -   Splnění standardu PCI DSS

-   **Ochrana soukromí**

    -   Dodržování GDPR

    -   Definovaná doba uchování osobních údajů

## 3. Spolehlivost a obnova

-   **Spolehlivost transakcí**

    -   Escrow a rozdělení plateb musí být atomické

    -   Použití ACID transakcí nebo kompenzační logiky

-   **Obnova po havárii**

    -   RTO: maximálně 1 hodina

    -   RPO: maximálně 15 minut

-   **Monitorování a alerting**

    -   24/7 monitoring

    -   Definované SLO metriky

-   **Auditovatelnost**

    -   Uchovávání logů minimálně 1 rok

    -   Neměnitelné auditní záznamy

## 4. Použitelnost a UX

-   **Uživatelská přívětivost**

    -   Intuitivní rozhraní pro všechny role

    -   Cílové skóre SUS: 75+

-   **Mobilní dostupnost**

    -   Podpora iOS a Android

    -   Podpora posledních dvou verzí OS

-   **Offline režim pro poslíčky**

    -   Lokální cache

    -   Fronta požadavků při ztrátě připojení

-   **Přístupnost**

    -   Splnění standardu WCAG 2.1 úroveň AA

## 5. Lokalizace a rozšiřitelnost

-   **Mezinárodní lokalizace**

    -   Podpora více jazyků

    -   Snadné přidání nového jazyka

-   **Údržba a rozšiřitelnost**

    -   Modulární architektura

    -   Minimálně 80 % pokrytí testy

-   **Testovatelnost**

    -   Automatizované testy: unit, integration, E2E

    -   CI pipeline

## 6. Náklady a právní požadavky

-   **Sledování nákladů**

    -   Monitoring cloudových nákladů

    -   Měsíční rozpočet a alerty

-   **Právní shoda**

    -   Dodržování zákonů pro prodej bylin a potravin

    -   Certifikace dle místní legislativy

## 7. Logika vyprodáno

-   **Blokace objednávek**

    -   Pokud je produkt vyprodán, systém okamžitě zabrání jeho
        objednání

    -   Kontrola probíhá transakčně při checkoutu
