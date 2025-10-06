# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Projet Overview

Neth CRM est un CRM personnalisé construit avec n8n et PostgreSQL. Le projet est en phase initiale de configuration.

## Stack Technique

- **Automation Platform**: n8n (hébergé sur VPS Infomaniak)
- **Base de données**: PostgreSQL (sur le même VPS)
- **Langages**: JavaScript/TypeScript pour les scripts n8n

## Structure du Projet

- `workflows/`: Workflows n8n exportés au format JSON
- `scripts/`: Scripts JavaScript/TypeScript réutilisables pour les nœuds Code de n8n
- `database/`: Schémas SQL et documentation de la base de données PostgreSQL
- `docs/`: Documentation du projet

## Contexte Important

1. **L'utilisateur préfère travailler en français** et souhaite comprendre chaque étape
2. **Approche progressive**: L'utilisateur demande explicitement le "go" avant de passer à l'étape suivante
3. **Pas de custom nodes n8n pour l'instant**: Le projet utilise des workflows n8n standards avec des nœuds Code JavaScript/TypeScript
4. **Base de données existante**: Les tables PostgreSQL existent déjà sur le VPS

## Workflow de Développement

1. Les workflows n8n sont développés sur le VPS Infomaniak
2. Les workflows sont exportés au format JSON et versionnés dans `workflows/`
3. Les scripts réutilisables sont stockés dans `scripts/` pour être utilisés dans les nœuds Code
4. La documentation de la base de données doit être maintenue dans `database/`

## Git Workflow

- Branche principale: `main`
- Remote: https://github.com/Nethelvetic/neth_crm.git
