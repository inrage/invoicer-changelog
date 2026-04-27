# Changelog Invoicer

Toutes les nouveautés livrées en production sur [Invoicer](https://invoicer.fr).

Format basé sur [Keep a Changelog](https://keepachangelog.com/fr/1.1.0/).

---

## 2026-04-21 — Paiement par carte bancaire

Vos clients règlent vos factures en un clic depuis un lien envoyé par email, SMS ou WhatsApp.

- Lien de paiement par facture, partageable sur n'importe quel canal
- Page de paiement simple aux couleurs du commerçant
- Encaissement géré par Stripe (vous gardez votre compte bancaire, l'argent y arrive sous 2 jours)
- Bascule automatique de la facture en "payée" dès le règlement
- Reçu envoyé au client à vos couleurs (pas celles de Stripe)
- Activation en 5 minutes via Stripe (souvent validation immédiate pour AE)
- Disponible sur les plans Pro (15 €) et Business (39 €). Commission Stripe ~1,5 % + 0,25 € par carte française.

→ [En savoir plus](https://invoicer.fr/features/paiement-en-ligne)

## 2026-04-17 — Déclaration URSSAF automatique

La compta mensuelle ou trimestrielle d'un auto-entrepreneur en 5 minutes, zéro charge mentale.

- CA encaissé calculé automatiquement (factures payées sur la période)
- Cotisations estimées avec les taux 2026 (BIC vente 12,3 %, BIC service 21,2 %, BNC général 25,6 %, BNC CIPAV 23,2 %)
- ACRE auto-appliqué selon date de fin
- Alertes franchise TVA (37 500 € services, 85 000 € vente) et plafond micro (77 700 € / 188 700 €)
- Projection annuelle pour anticiper un dépassement
- Rappel email automatique avec récap + lien direct vers le portail URSSAF
- Export CSV prêt à coller dans le portail URSSAF
- Activité mixte vente/service supportée (override par ligne)

→ [En savoir plus](https://invoicer.fr/features/declaration-urssaf)

## 2026-04-17 — Devis révisables avec lien public

Modifiez un devis envoyé sans annuler, partagez un lien sécurisé à votre client ou apporteur d'affaires.

- Bouton "Créer une révision" qui repasse le document en brouillon éditable
- Numéro du devis préservé (le client ne voit pas de référence changeante)
- Historique complet des versions avec auteur, date, raison
- Lien public signé de 90 jours, sans compte requis pour le consulter
- Le lien affiche toujours la dernière version validée (pas les brouillons en cours)

→ [En savoir plus](https://invoicer.fr/features/devis-revisables)

## 2026-04-13 — Synchronisation bancaire enrichie

Le rapprochement bancaire passe au niveau supérieur grâce à Bridge API.

- Suggestions intelligentes de rapprochement (référence dans le libellé, montant exact, nom du client)
- Mode rattrapage pour reconstituer l'historique des paiements bancaires passés
- Détection multi-factures (un virement → plusieurs factures d'un même client)
- Alertes d'expiration DSP2 (renouvellement en un clic à 180 jours)
- Recherche et filtrage avancés des transactions

→ [En savoir plus](https://invoicer.fr/features/synchronisation-bancaire)

## 2026-03-29 — Relances automatiques d'impayés

Vos factures impayées se relancent toutes seules, à votre rythme et sur votre ton.

- 3 niveaux d'escalade : rappel amical → relance → mise en demeure
- Délais entre niveaux configurables
- Templates personnalisables avec variables `[REFERENCE]`, `[TOTAL_TTC]`, `[DUE_DATE]`, `[CONTACT_FULLNAME]`
- PDF de la facture joint automatiquement
- Timeline complète des relances envoyées sur la fiche facture
- Une seule relance par jour et par facture (escalade progressive)

→ [En savoir plus](https://invoicer.fr/features/relances-automatiques)

## 2026-02-25 — Facturation électronique 2026

Préparez-vous à la réforme obligatoire dès septembre 2026 directement depuis Invoicer.

- Tableau de bord e-invoicing dédié
- Assistant pas-à-pas pour connecter votre compte à Pennylane (PDP agréée)
- Connexion OAuth sécurisée
- Émission de factures au format électronique conforme depuis vos documents existants

→ [En savoir plus](https://invoicer.fr/facturation-electronique)

## 2026-02-24 — Factur-X et TVA internationale

Vos factures embarquent automatiquement le format Factur-X et la TVA s'adapte au pays du client.

- XML Factur-X (profil Basic) embarqué dans chaque PDF
- TVA automatique : 0 % avec mention art. 262 ter I (intra-UE B2B), 0 % avec mention art. 262-I (hors UE)
- Nouveaux taux 2,1 % et 10 % disponibles
- Champ pays sur la fiche société

## 2026-02-23 — Lignes de texte libre dans les documents

Insérez du texte informatif en markdown entre vos lignes de prix.

- Lignes sans quantité, prix ou TVA
- N'impactent pas les totaux
- Utiles pour précisions techniques, conditions particulières, sections

## 2026-02-23 — Notifications "Quoi de neuf"

Restez informé des dernières nouveautés sans quitter l'application.

- Icône dédiée dans la barre de navigation
- Point bleu pour les nouveautés non lues
- Résumé court + description détaillée par entrée

## 2026-02-22 — Note markdown sur les documents

Champ note avec mise en forme markdown sur factures, devis et avoirs.

- Markdown supporté
- Apparaît sur le PDF généré dans tous les templates
- Pour conditions particulières, infos complémentaires, détails de livraison

## 2026-02-20 — Destinataires email intelligents

Les destinataires sont automatiquement résolus selon les catégories et tags des contacts.

- Configuration par contact : "tous les emails" ou ciblage par catégories/tags
- Suggestions automatiques à l'envoi
- Regroupement par source dans le sélecteur

## 2026-02-18 — TVA par ligne de document

Définissez un taux de TVA différent pour chaque ligne d'un document.

- Multiples taux sur un même document (20 %, 10 %, 5,5 %, 2,1 %)
- Récap TVA avec ventilation par taux
- Taux par défaut configurable sur chaque service

## 2026-02-18 — Checklist d'onboarding

Guide de démarrage interactif sur le dashboard.

- Étapes essentielles : profil entreprise, premier service, premier client, première facture
- Disparaît automatiquement une fois complétée

## 2026-02-17 — Visite guidée

Tours interactifs page par page pour découvrir l'interface.

- Surbrillance des éléments importants
- Explications contextuelles
- Progression sauvegardée

## 2026-02-16 — Gestion des membres

Gérez les membres de votre groupe directement depuis l'application.

- Suppression de membres
- Création de nouveau groupe depuis un compte existant

## 2026-02-05 — Sélection de documents en masse

Sélectionnez plusieurs documents pour voir les totaux et exécuter des actions groupées.

- Cases à cocher dans la liste
- Total HT et TTC affichés sur la sélection
- Actions groupées (export Pennylane…)
- Sélection conservée entre les pages

---

📝 La liste complète des nouveautés est aussi disponible directement dans l'application sous l'icône **"Quoi de neuf"**.
