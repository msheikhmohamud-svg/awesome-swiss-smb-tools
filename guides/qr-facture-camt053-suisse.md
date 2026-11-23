# QR-facture suisse et relevés bancaires ISO 20022 (`camt.053` / `camt.054`) : checklist technique

Depuis le remplacement complet des bulletins de versement rouges et orange (BVR/BV) par la **QR-facture suisse**, toute facturation et tout rapprochement bancaire professionnel en Suisse reposent sur les **Swiss Payment Standards** publiés par **SIX**. Un outil de gestion pour indépendants ou PME doit être testé sur ces flux précis avant utilisation en production.

---

## 1. QR-facture suisse : points de contrôle essentiels

- **Adresses structurées :** Les spécifications suisses encadrent strictement le format des adresses (rue, numéro, code postal, localité, pays) plutôt que les anciennes adresses non structurées.
- **Types de références :**
  - **Référence QR (QRR)** avec IBAN-QR (27 caractères numériques, idéale pour la réconciliation automatisée des paiements entrants).
  - **Creditor Reference (SCOR / ISO 11649)** avec IBAN standard.
  - **Sans référence** (cas simples ou dons).
- **Lisibilité & contrôle :** Vérifier que le Swiss QR Code généré respecte les dimensions officielles, la croix suisse centrée et la section paiement détachable (ou format numérique conforme).

---

## 2. Relevés bancaires ISO 20022 : `camt.053` vs `camt.054` vs `pain.001`

| Message XML ISO 20022 | Rôle dans la comptabilité PME |
|---|---|
| **`camt.053`** *(Bank-to-Customer Statement)* | Extrait de compte complet de fin de journée/mois contenant toutes les écritures comptabilisées (soldes d'ouverture/clôture et mouvements). |
| **`camt.054`** *(Debit/Credit Notification)* | Avis détaillé des encaissements (notamment les paiements QR regroupés), utile pour rapprocher chaque facture client sans attendre le relevé mensuel. |
| **`pain.001`** *(Customer Credit Transfer)* | Fichier d'ordres de paiement émis par le logiciel vers l'e-banking pour régler les factures fournisseurs. |

### Bonnes pratiques lors du test d'un logiciel
1. Importer un vrai fichier `camt.053` anonymisé contenant plusieurs types de mouvements (paiement partiel, frais bancaires, remboursement, encaissement groupé).
2. Réimporter le même fichier une deuxième fois pour vérifier que **la détection des doublons** bloque toute double comptabilisation.
3. Vérifier qu'une opération rapprochée par erreur peut être annulée ou corrigée tout en conservant une piste d'audit claire.

---

## 3. Sources officielles & liens

- **SIX — Spécifications QR-facture :** [six-group.com — QR-bill](https://www.six-group.com/fr/products-services/banking-services/payment-standardization/standards/qr-bill.html)
- **SIX — Standards ISO 20022 (camt / pain) :** [six-group.com — Standards](https://www.six-group.com/fr/products-services/banking-services/payment-standardization/standards.html)
- **Découvrir l'approche Sismondi :** [Sismondi Pro](https://sismondi.app/pro) · [Guide comptabilité suisse](https://sismondi.app/guide-comptabilite-suisse)
