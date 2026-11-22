# finanalytics-powerbi

Dashboard Power BI de **Finance Analytics** pour un contexte industriel  : rentabilité, écarts budget/réel, bilan et ratios.

Toutes les données sont **illustratives** et ne proviennent d'aucune entreprise réelle.

## Contenu du dashboard (3 pages)

| Page | Question | Visuels principaux |
|---|---|---|
| **Synthèse** | Où en est-on vs budget ? | KPI (CA, EBITDA, marge, résultat net), courbe Réel vs Budget, écart EBITDA par ligne produit |
| **Écarts et causes** | Pourquoi l'écart ? | Pont EBITDA Budget → Réel, matrice P&L, effet prix par ligne |
| **Bilan et cash** | Sommes-nous solides ? | Current ratio, gearing, ROE, DSO / DIO / DPO, CCC, structure de l'actif |

Filtres communs : année, site, ligne produit.

## Modèle de données

Schéma en étoile : 5 dimensions (date, site, ligne produit, comptes P&L et bilan), 4 tables de faits (P&L, volumes/prix, bilan, ratios trimestriels de contrôle) et une table de mesures DAX.

## Mesures DAX clés

- **P&L** Réel et Budget : CA, marge sur coûts variables, EBITDA, EBIT, résultat net
- **Écarts** Réel vs Budget, avec statuts d'alerte
- **Décomposition Prix / Volume / Mix** et pont EBITDA
- **Bilan et ratios** : current ratio, gearing, ROE, DSO, DIO, DPO, CCC
- **Contrôles intégrés** : réconciliation avec la table de ratios, équilibre du bilan





