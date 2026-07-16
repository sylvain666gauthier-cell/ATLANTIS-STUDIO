# ATLANTIS STUDIO — Règles pour tous les agents

## Identité et autorité

Ce dépôt est le studio de production du **Livre-Portail**, saga en 13 tomes de Sylvain Gauthier.

**Sylvain Gauthier est l'autorité finale et unique du canon.** Aucun agent ne crée, modifie ou supprime un élément du canon de sa propre initiative. Aucun agent ne modifie une loi fondamentale sans validation explicite de l'auteur.

## Les trois états d'une idée

Toute idée porte obligatoirement un statut :

- **PROPOSITION** — idée en discussion, émise par l'auteur ou par un agent. N'engage rien.
- **VALIDÉE** — idée approuvée explicitement par l'auteur, en attente d'intégration.
- **CANONIQUE** — idée intégrée officiellement dans les fichiers de `canon/`.

Une suggestion d'agent est TOUJOURS une PROPOSITION. Elle ne devient jamais VALIDÉE ou CANONIQUE sans l'accord explicite de Sylvain.

## Procédure avant toute tâche créative

1. Lire les fichiers du canon concernés (`canon/`).
2. Lire les décisions récentes (`memory/decisions.md`) et le dernier compte rendu de session (`memory/sessions/`).
3. Vérifier `PROJECT_STATUS.md`.
4. Choisir le skill adapté (`skills/`).
5. Produire une proposition structurée et ATTENDRE la validation.

## Procédure après validation

1. Intégrer la modification.
2. Mettre à jour les fichiers du canon concernés.
3. Ajouter une entrée dans `memory/decisions.md` et `memory/changelog.md`.
4. Signaler les conséquences possibles sur les autres œuvres ou fichiers.

## Interdictions

- Ne jamais inscrire au canon une idée non validée.
- Ne jamais introduire de nouveau terme, concept ou personnage sans le signaler explicitement.
- Les artefacts ne réagissent JAMAIS d'eux-mêmes : toute révélation vient du travail, du doute, du conflit ou du coût. Cette règle narrative est inviolable.
- Prose : dense, directe, qui avance. Pas de dilution poétique, pas de rappels métafictionnels au lecteur. Le style est régi exclusivement par `canon/style.md`.
- Ne jamais employer le terme « Akasha » dans la prose des œuvres (voir vocabulaire, `canon/constitution.md`).

## Noms des agents — règle d'étanchéité

Les noms mythologiques des agents (Hermès Prime, Thot, etc.) sont des **identifiants**, pas des personnages. Aucun agent n'adopte le style, le ton ou la personnalité de la figure dont il porte le nom.

Les noms de l'**univers** (canon) et les noms de l'**outillage** (agents, studios, scripts) vivent dans deux espaces étanches. En cas de collision, le canon a priorité de nommage : c'est l'outil qui est renommé, jamais le canon.

## Changement d'outil (Claude Code ↔ Antigravity)

Toujours partir d'un état Git propre. Commiter avant de changer d'outil. Les mémoires internes des IDE ne comptent pas : seule la mémoire du dépôt (`memory/`) fait foi.

## Rituel de fin de session

Chaque session de travail significative se termine par un compte rendu déposé dans `memory/sessions/` (gabarit : `memory/sessions/template-session.md`), puis un commit Git.
