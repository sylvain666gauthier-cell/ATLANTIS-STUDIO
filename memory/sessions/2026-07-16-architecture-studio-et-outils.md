# Compte rendu de session — 2026-07-16 — Architecture du studio, Maât, outils externes

> Emplacement : `memory/sessions/2026-07-16-architecture-studio-et-outils.md`

## Contexte

Analyse du document d'architecture « Atlantis Studio » (studio créatif unifié pour le Livre-Portail), discussion sur Obsidian comme mémoire, définition de la fonction cosmologique de Maât, évaluation de l'organigramme mythologique des agents, examen de trois projets GitHub (superpowers, hermes-agent, odysseus), et mise en place du protocole d'archivage des sessions.

## Décisions

| Statut | Décision | Fichiers concernés |
|---|---|---|
| VALIDÉE | Architecture générale du studio : séparation canon / mémoire, canon fragmenté en fichiers par concept, trois états des idées (PROPOSITION / VALIDÉE / CANONIQUE) | `canon/`, `memory/` |
| VALIDÉE | Démarrage en version minimale réduite : canon + mémoire + 3 skills (brainstorming, rédaction longue, vérification), un seul volume, Git dès le premier jour | racine du dépôt |
| VALIDÉE | Ne PAS créer les dossiers film-studio/, visual-studio/, audio-studio/, jeu, web avant qu'une œuvre approuvée existe (pas même en squelette) | — |
| VALIDÉE | Organigramme mythologique complet conservé comme vision cible dans `VISION.md` ; embauche des agents un par un quand une œuvre le réclame. Équipe fondatrice : Hermès Prime (orchestrateur), Thot (canon + mémoire), un écrivain (Volume I) | `VISION.md`, `HERMES.md` |
| VALIDÉE | Adoption de Superpowers (obra) comme méthodologie : plugin Claude Code + Antigravity ; son skill `writing-skills` servira de moule aux skills littéraires | `skills/` |
| VALIDÉE | Protocole d'archivage : compte rendu de session en fin de chaque conversation → `memory/sessions/` → commit Git ; une conversation = un sujet ; Projet Claude avec les fichiers pivots | `memory/sessions/` |
| PROPOSITION | Maât = mémoire cosmique de l'univers (fonction d'archive du circuit Terre–Lune–Maât–Soleil), en écho fractal à la mémoire organique. Grandes lignes discutées mais statut non tranché par l'auteur | `canon/01-cosmologie/maat.md`, `canon/02-vivant/memoire-organique.md`, `canon/03-lois/` |
| PROPOSITION | Le mot « Akasha » interdit dans la prose des œuvres (terme New Age daté) ; les traditions humaines (annales akashiques, Livre de Vie) traitées comme échos déformés de Maât | `canon/00-constitution/vocabulaire-interdit.md` |

## Propositions en suspens

- (IA) Trois pistes pour le coût d'accès à Maât — à trancher AVANT toute scène impliquant Maât :
  1. Accès partiel déformé par la structure du lecteur (chaque personnage = une clé différente → justifie la chorale des 13)
  2. La pesée comme filtre : Maât répond à la justesse, pas à la curiosité (l'antagoniste structurellement incapable d'y accéder par la force)
  3. Coût mémoriel : lire la mémoire cosmique s'échange contre de la mémoire personnelle
- (IA) hermes-agent (Nous Research) comme candidat pour incarner Hermès Prime en Phase 2 : orchestrateur permanent sur VPS, joignable par Telegram, cron en langage naturel. À réévaluer quand le besoin d'un opérateur permanent apparaît. Distinguer toujours *Hermès Prime* (le rôle) de *hermes-agent* (le logiciel).
- (IA) Obsidian comme fenêtre de navigation humaine sur le dépôt (pas comme fondation) : liens Markdown standards plutôt que wikilinks, `.obsidian/` dans le gitignore, ne pas dépendre des plugins.
- (IA) Automatiser la mise à jour de la mémoire (changelog généré depuis les diffs Git) plutôt que de la confier aux agents ; réduire les fichiers de mémoire au minimum.
- (IA) Vérification du canon partiellement scriptable : détection des termes du vocabulaire interdit et des noms absents de l'index, en complément du contrôle LLM.

## Questions ouvertes

- Collision de vocabulaire : « MAÂT LAB » (studio scientifique) vs Maât (entité cosmique canonique). Règle à formaliser : noms de l'univers et noms de l'outillage dans deux espaces étanches. Renommer le studio scientifique.
- Hermès apparaît deux fois dans l'organigramme (directeur général et rédacteur en chef) — à corriger.
- Articulation entre le nouveau cadrage « Atlantis Studio » (Li Wei, Aarav, Traité du Vivant) et le travail existant du Livre-Portail (Élias Marceau, chapitre 1 rédigé) : même univers ? Migration du matériel existant vers `canon/` = première tâche de la Phase 1.
- Statut définitif de Maât-mémoire-cosmique : à valider ou amender par l'auteur.

## Actions

- [ ] Créer le dépôt Git `ATLANTIS-STUDIO/` avec la structure minimale réduite
- [ ] Installer Superpowers dans Claude Code (`/plugin install superpowers@claude-plugins-official`) et Antigravity
- [ ] Créer `VISION.md` avec l'organigramme mythologique complet et les conditions d'embauche de chaque agent
- [ ] Migrer le matériel existant du Livre-Portail (chapitre 1, règles narratives, structure en 5 temps, antagoniste à 4 pouvoirs) vers `canon/`
- [ ] Créer le Projet Claude « Livre-Portail / Atlantis Studio » avec les fichiers pivots
- [ ] Trancher le coût d'accès à Maât avant d'écrire toute scène l'impliquant
- [ ] Renommer « MAÂT LAB » (éviter la collision avec le canon)
- [ ] Écarté : Odysseus (plateforme monolithique, ne sert pas le goulot d'étranglement)

## Vocabulaire / canon touché

- « Akasha » → candidat au vocabulaire interdit (prose)
- Règle proposée : espaces de nommage étanches entre univers (canon) et outillage (agents)
- Fichiers du canon à créer/toucher si Maât validée : `maat.md`, `circuit-continu.md`, `memoire-organique.md`, une loi éventuelle dans `03-lois/`

## Notes libres

Principe directeur de toute la session : le goulot d'étranglement du projet est **la prose approuvée**. Chaque outil, agent ou dossier se justifie par ce test : sert-il ce goulot aujourd'hui ? Le système garantit la cohérence, pas la qualité — `09-style/exemples-valides.md` doit être alimenté par des passages réellement écrits et approuvés, jamais par des règles aspirationnelles.
