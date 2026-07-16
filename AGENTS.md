# ATLANTIS STUDIO — Règles pour tous les agents

## Identité et autorité

Ce dépôt est le studio de production du **Corpus Atlante** de Sylvain Gauthier.

Œuvre en production : **Le Traité du Vivant** — manuscrit fondateur qui englobe l'univers atlante, structuré par les treize constellations originelles. Les tomes narratifs (Livre-Portail) viendront ensuite.

**Sylvain Gauthier est l'autorité finale et unique du canon** (voir `canon/00-constitution.md`, qui prime sur le présent fichier pour tout ce qui concerne le canon).

## Statuts des idées

Les statuts et leurs qualificatifs sont définis par la Constitution (sections 4 et 4 bis) :
`[PROPOSITION]`, `[VALIDÉ]`, `[CANONIQUE]`, `[INTERPRÉTATION]`, `[À RÉSOUDRE]`, `[ABROGÉ]`,
avec les qualificatifs `[PROPOSITION FORTE]`, `[CANONIQUE DANS SES GRANDES LIGNES]`, `[À DÉTAILLER]`.

Règle absolue : toute suggestion d'agent est une `[PROPOSITION]`. Elle ne monte en statut que par décision explicite de Sylvain.

## Ordre de lecture du canon

```text
00-constitution.md → 01-lois.md → 02-cosmologie.md → 03-vivant.md → 04-constellations.md → 05-style.md
```

Les fichiers spécialisés citent les Lois Fondatrices ; ils ne les reformulent jamais.

## Procédure avant toute tâche créative

1. Lire les fichiers du canon concernés, dans l'ordre ci-dessus.
2. Lire `memory/decisions.md` et le dernier compte rendu de `memory/sessions/`.
3. Vérifier `PROJECT_STATUS.md`.
4. Choisir le skill adapté (`skills/`).
5. Produire une proposition structurée et ATTENDRE la validation.

## Procédure après validation

Suivre le workflow de modification de la Constitution (section 11) : modification atomique, mise à jour du journal (`memory/changelog.md`, format YAML de la Constitution section 12), signalement des conséquences.

## Interdictions

- Ne jamais inscrire au canon une idée non validée. Le silence du canon demeure un silence (Constitution, 9).
- Ne jamais introduire de nouveau terme, concept ou personnage sans signalement explicite.
- Respecter intégralement les interdictions fondamentales de la Constitution (section 7) et le vocabulaire contrôlé (section 8).
- Style : appliquer `canon/05-style.md` — pour le Traité, la Partie I (voix du manuscrit) uniquement.

## Noms des agents — règle d'étanchéité

Les noms mythologiques des agents sont des identifiants, pas des personnages. Aucun agent n'adopte le style, le ton ou la personnalité de la figure dont il porte le nom.

Les noms de l'univers (canon) et de l'outillage vivent dans deux espaces étanches (Constitution, 2 bis). En cas de collision, le canon a priorité : c'est l'outil qui est renommé.

## Changement d'outil (Claude Code ↔ Antigravity)

Toujours partir d'un état Git propre. Commiter avant de changer d'outil. Seule la mémoire du dépôt (`memory/`) fait foi.

## Rituel de fin de session

Chaque session significative se termine par un compte rendu dans `memory/sessions/` (gabarit : `template-session.md`), puis un commit Git.
