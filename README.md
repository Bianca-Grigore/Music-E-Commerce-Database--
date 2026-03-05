# 🎵 Bază de Date pentru un Magazin Online de Muzică 

## 📌 Descrierea Proiectului
Acest repository conține arhitectura, designul și implementarea practică a unei baze de date relaționale destinate administrării complexe a unui magazin e-commerce specializat în articole muzicale. Proiectul modelează fluxurile informaționale reale dintr-o astfel de afacere, asigurând integritatea datelor și optimizarea operațiunilor zilnice, de la stocuri până la interacțiunea cu utilizatorul final.

## ⚙️ Arhitectura și Modulele de Business
Schema bazei de date a fost proiectată modular, acoperind patru direcții principale de activitate:

### 1. 📦 Gestiunea Lanțului de Aprovizionare (Supply Chain)
Acest modul urmărește trasabilitatea produselor înainte ca acestea să ajungă la client. Baza de date înregistrează entitățile de tip **FURNIZOR** și gestionează locațiile fizice de stocare (**DEPOZIT**). Astfel, sistemul poate interoga în orice moment originea mărfii, rutele de aprovizionare și disponibilitatea produselor în anumite depozite specifice.

### 2. 🎸 Catalogul Comercial
Organizarea portofoliului de **PRODUSE** este flexibilă și detaliată. Produsele sunt structurate ierarhic pe **CATEGORII** (ex: instrumente, echipamente audio, viniluri) și, acolo unde este relevant, sunt direct asociate cu un **ARTIST** (pentru albume, merchandise, etc.). Această structură permite filtrări complexe și căutări rapide în platformă.

### 3. 👥 Interacțiunea cu Clienții și Vânzări (CRM)
Nucleul operațiunilor comerciale se bazează pe entitatea **CLIENȚI**. Baza de date păstrează un istoric complet și detaliat al **COMENZILOR** plasate de aceștia. Mai mult, a fost integrat un sistem de **RECENZII**, permițând stocarea feedback-ului oferit de cumpărători pentru fiecare produs în parte, esențial pentru evaluarea performanței comerciale.

### 4. 📈 Marketing și Promovare
Pentru a susține strategiile de vânzări, modelul relațional include o componentă dedicată pentru **CAMPANII PROMOȚIONALE**. Aceasta permite aplicarea unor strategii de marketing țintite și asocierea produselor cu diverse oferte pe perioade determinate de timp.

## 🛠️ Implementare Tehnică (Cerințe SGBD)
Scripturile `.sql` incluse în acest proiect acoperă întregul ciclu de dezvoltare a bazei de date:
* Modelarea conceptuală și logică (Diagrame ERD).
* Definirea structurii (creare tabele, chei primare, chei externe și constrângeri de integritate).
* Popularea bazei de date cu seturi de date de test (instrucțiuni INSERT).
* Interogări complexe (join-uri, subcereri, funcții grup).
* Implementarea logicii de business prin structuri PL/SQL (blocuri anonime, tipuri de date complexe, funcții, proceduri, pachete și triggere).
