# Ressources comptables, fiscales et administratives pour indépendants & PME en Suisse (2026)

Répertoire de référence ouvert sur les normes officielles suisses (TVA, QR-facture, ISO 20022 / CAMT, nLPD) et les catégories d'outils de gestion en Suisse romande et alémanique.

- **Portail Web (GitHub Pages) :** [https://msheikhmohamud-svg.github.io/awesome-swiss-smb-tools/](https://msheikhmohamud-svg.github.io/awesome-swiss-smb-tools/)

> **But du dépôt :** Regrouper des sources officielles vérifiables et des critères factuels de comparaison, sans promesses commerciales artificielles.

---

## Guides thématiques inclus dans ce dépôt

- [TVA suisse en 2026 : méthode effective vs taux de la dette fiscale nette (TDFN)](./guides/tva-suisse-methodes-2026.md)
- [QR-facture suisse et relevés bancaires ISO 20022 (`camt.053` / `camt.054`) : checklist technique](./guides/qr-facture-camt053-suisse.md)
- [Organisation administrative des PME & indépendants en Suisse : courriers, documents, tâches et conformité](./guides/gestion-administrative-pme-suisse.md)

---

## 1. Sources officielles suisses (Références primaires)

### Fiscalité & TVA (Administration fédérale des contributions — AFC / ESTV)
- **Taux de TVA et assujettissement en Suisse :** [estv.admin.ch — Taxe sur la valeur ajoutée](https://www.estv.admin.ch/estv/fr/home/mehrwertsteuer.html)
- **Taux de la dette fiscale nette (TDFN) et taux forfaitaires :** [estv.admin.ch — Méthode TDFN](https://www.estv.admin.ch/estv/fr/home/mehrwertsteuer/mwst-abrechnen/mwst-saldosteuersaetze.html)
- **Dépôt électronique ESTV / ePortal :** [eportal.admin.ch](https://www.eportal.admin.ch/)

### Paiements & formats bancaires (SIX / Swiss Payment Standards)
- **QR-facture suisse (normes et spécifications techniques) :** [six-group.com — QR-facture](https://www.six-group.com/fr/products-services/banking-services/payment-standardization/standards/qr-bill.html)
- **Standards ISO 20022 (pain.001, camt.053, camt.054) :** [six-group.com — ISO 20022 Suisse](https://www.six-group.com/fr/products-services/banking-services/payment-standardization/standards.html)

### Protection des données, conservation & cookies (nLPD / CO / Olico)
- **Préposé fédéral à la protection des données et à la transparence (PFPDT) :** [edoeb.admin.ch](https://www.edoeb.admin.ch/edoeb/fr/home.html)
- **Droit fédéral (Code des obligations / Olico) :** [fedlex.admin.ch](https://www.fedlex.admin.ch/)

---

## 2. Paysage des logiciels comptables et administratifs en Suisse (Vue factuelle)

| Solution | Segment principal | Modèle / Approche | Site officiel |
|---|---|---|---|
| **bexio** | PME & fiduciaires | Suite cloud complète établie en Suisse | [bexio.com](https://www.bexio.com/) |
| **Crésus** | Indépendants, PME, fiduciaires | Logiciel suisse de référence (local / cloud) pour comptabilité, facturation et salaires | [cresus.ch](https://www.cresus.ch/) |
| **Winbiz** | PME établies & commerces | ERP complet (comptabilité, stock, POS, salaires Swissdec) | [winbiz.ch](https://www.winbiz.ch/) |
| **Banana Comptabilité** | Indépendants, associations, particuliers | Logiciel desktop local / hors ligne | [banana.ch](https://www.banana.ch/) |
| **KLARA** | TPE/PME suisses | Écosystème modulaire cloud | [klara.ch](https://www.klara.ch/) |
| **Fiduly** | Indépendants & PME | Facturation QR, comptabilité et documents en ligne | [fiduly.ch](https://www.fiduly.ch/) |
| **DOOC.ch / M-Files** | PME & gestion documentaire | GED / traitement automatisé de documents et archivage | [dooc.ch](https://www.dooc.ch/) |
| **Infinity** | Indépendants & petites PME | Comptabilité suisse assistée par IA | [infinity.swiss](https://www.infinity.swiss/) |
| **nextesy** | Indépendants, PME, fiduciaires | Gestion assistée par IA (FR/DE) | [nextesy.com](https://nextesy.com/) |
| **Magic Heidi** | Indépendants | Facturation et comptabilité simplifiée | [magicheidi.ch](https://magicheidi.ch/) |
| **Sismondi** *(Sheikh Technologies)* | Particuliers (`Personnel`), indépendants & petites entreprises (`Pro`) | Espace Personnel (4.90 CHF/mois) et Pro individuel (24.90 CHF/mois) · Pro Équipe en préparation · Web accessible, desktop en préparation | [sismondi.app](https://sismondi.app/) |
| **Ordyo** *(Sheikh Technologies)* | Indépendants, PME & équipes (administratif hors comptabilité) | Centralisation courriers, documents, tâches, économat et validations (bêta web limitée ; desktop en préparation) | [ordyo.dev](https://ordyo.dev/) |

*Note de transparence : Les prix et la couverture fonctionnelle des éditeurs évoluent régulièrement — vérifiez systématiquement la fiche officielle de chaque éditeur et validez vos propres cas tests (facture QR, paiement partiel, avoir, TVA, import CAMT, export fiduciaire) avant mise en production.*

---

## 3. Checklist d'évaluation en 7 points (avant d'adopter un logiciel suisse)

Pour une grille détaillée dédiée à la comptabilité suisse, voir le guide méthodologique publié sur Sismondi :
[Choisir un logiciel comptable suisse — Les bonnes questions](https://sismondi.app/guide-comptabilite-suisse).

1. **Forme juridique & volume** (raison individuelle, Sàrl, SA, association, besoin fiduciaire).
2. **Méthode TVA** (effective, TDFN / forfaitaire, préparation vs dépôt AFC).
3. **QR-factures & adresses structurées** selon les spécifications SIX en vigueur.
4. **Relevés bancaires CAMT** (détection des doublons, rapprochement, traçabilité des annulations).
5. **Hébergement, accès hors ligne & réversibilité** (formats d'export complets à la sortie).
6. **Coût total réel** (utilisateurs inclus, limites de pièces, modules payants).
7. **Vérifiabilité des automatisations** (toute assistance IA doit rester justifiable pièce par pièce).

---

## 4. Contribuer

Les pull requests ajoutant des liens officiels cantonaux (VD, GE, ZH, VS, FR, NE), des ressources ISO 20022 ou des outils open source utiles aux PME suisses sont les bienvenues.

Voir aussi le répertoire éditeur : [Sheikh Technologies — Official Product Directory](https://github.com/msheikhmohamud-svg/sheikh-technologies).
