# Rapport d'Entraînement en Reconnaissance

Ce document présente les résultats d'un exercice de reconnaissance mené à des fins éducatives. Il est divisé en deux phases : la reconnaissance passive (OSINT) et la reconnaissance active (Nmap).

---

## Phase 1 : Reconnaissance Passive (OSINT)

### 🎯 Périmètre de l'exercice
-   **Nom de domaine cible :** mercedes-benz.fr

### 🛠️ Outils et Techniques
-   Commande `whois`
-   Opérateurs de recherche "Google Dorks"

### 📜 Résultats
-   **Analyse `whois` :** Le registraire identifié pour le nom de domaine est **KEY-SYSTEMS GmbH**.
-   **Résultats des Google Dorks :**
    -   **Dork utilisé :** `site:mercedes-benz.fr filetype:pdf`
    -   **Résultat :** A permis de trouver plusieurs documents PDF, principalement des brochures et des manuels d'utilisation.

---

## Phase 2 : Reconnaissance Active (Nmap)

### 🎯 Périmètre de l'exercice
-   **Cible autorisée :** `scanme.nmap.org`

### 🛠️ Outils et Techniques
-   Nmap (Network Mapper)

### 📜 Résultats
-   **Commande utilisée :** `nmap -sV scanme.nmap.org`
-   **Résumé des découvertes :** Le scan a révélé plusieurs ports ouverts. Les plus notables sont :
    -   **Port 22/tcp :** Ouvert, service **OpenSSH 6.6.1
    -   **Port 80/tcp :** Ouvert, service **Apache httpd 2.4.7

---

## 🧠 Compétences acquises
-   Collecte d'informations via `whois` et Google Dorks.
-   Scan de ports et de services avec Nmap.
-   Analyse et interprétation des résultats d'un scan Nmap.
-   Rédaction d'un rapport de reconnaissance structuré.
