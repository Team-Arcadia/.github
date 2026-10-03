<div align="center">

<img src="https://www.arcadia-echoes-of-power.fr/storage/img/arcadialogotransparent2.webp" alt="Arcadia: Echoes Of Power" width="260"/>

# Team Arcadia

**Mods, forks, tools and community services behind *Arcadia: Echoes Of Power*.**

[![Organization](https://img.shields.io/badge/GitHub-Team--Arcadia-181717?style=flat-square&logo=github)](https://github.com/Team-Arcadia)
[![Discord](https://img.shields.io/badge/Discord-Join%20us-5865F2?style=flat-square&logo=discord&logoColor=white)](https://arcadia-echoes-of-power.fr/discord)
[![Website](https://img.shields.io/badge/Website-arcadia--echoes--of--power.fr-2E8B57?style=flat-square)](https://www.arcadia-echoes-of-power.fr)
[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.1-62B47A?style=flat-square)](#english)
[![NeoForge](https://img.shields.io/badge/NeoForge-21.1.x-D7742F?style=flat-square)](#english)

**[English](#english)** &nbsp;·&nbsp; **[Français](#francais)**

</div>

---

<a name="english"></a>

## English

Team Arcadia runs **Arcadia: Echoes Of Power**, a French modded Minecraft server (NeoForge 1.21.1) where Create
technology, magic and a player economy meet. The team does much more than a website: it writes its own mods, publishes
mods for the whole Minecraft community, and maintains fixed builds of the third-party mods the modpack relies on.

### What we make

| Family | Prefix | In short |
|---|---|---|
| [Arcadia mods](#arcadia-mods) | `arcadia-` | Mods written for our server and modpack: minigames, dungeons, protection, spawn, performance. |
| [Mods for everyone](#mods-for-everyone) | `mods-mc-` | Mods maintained by Team Arcadia but not tied to Arcadia. They work on any server or modpack. |
| [Forks we maintain](#forks-we-maintain) | `fork-mc-` | Third-party mods used in our modpack, patched by us to fix crashes and incompatibilities. |
| [Discord bot](#discord-bot) | `discord-bot-` | Arcadius, the bot of our Discord community. |
| [Website](#website) | `azuriom-` | Our Azuriom website, its theme and its plugins. |

The full guide (naming convention, how everything fits together, contributing) is on the
[organization page](https://github.com/Team-Arcadia).

### How we work: repository names

Every repository name starts with a **prefix that tells which family it belongs to**, followed by the name of the
project. You know what a repository is before opening it.

| Family | Repository name | Example | Rule |
|---|---|---|---|
| Arcadia mods | `arcadia-<mod-name>` | `arcadia-games`, `arcadia-guard` | A mod made for the Arcadia server or modpack. |
| Mods for everyone | `mods-mc-<mod-name>` | `mods-mc-rspolymorph` | A mod maintained by Team Arcadia that works without Arcadia. |
| Forks | `fork-mc-<original-mod-name>` | `fork-mc-ecologics` | Someone else's mod that we patch. The name is the original mod's name. |
| Website | `azuriom-<plugin-name>` | `azuriom-<plugin-id>` | A plugin of our Azuriom website. The theme is `azuriom-theme-<name>`. |
| Discord bots | `discord-bot-<bot-name>` | `discord-bot-arcadius` | A bot running on our Discord. |
| Organization | `.github` | `.github` | This repository: organization profile and default community files. |

**Rules for every repository**

1. **Lowercase only**, words separated by hyphens: `arcadia-spawndimension`, never `Arcadia_SpawnDimension`.
2. **The prefix is mandatory.** Pick it with one question: *is it our mod for Arcadia* (`arcadia-`), *our mod for
   everyone* (`mods-mc-`), or *someone else's mod we fix* (`fork-mc-`)?
3. **The name after the prefix says what the project is**: the mod's name for a mod, the original project name for a
   fork, the plugin's name for a website plugin.
4. **One-sentence description in English** and the topic `team-arcadia` on every repository.
5. **Forks keep the original license and credits.** Our patches go on a dedicated branch (`Arcadia-fix` when needed).

> A few older repositories predate this convention, for example `Arcadia-Dungeon`. They will be renamed over time;
> GitHub redirects old links automatically.

<a name="arcadia-mods"></a>

### Arcadia mods

Built *for* the Arcadia server and modpack. They run on NeoForge 1.21.1 and most of them are server-side only, so
players do not need to install anything extra.

| Mod | What it does |
|---|---|
| [arcadia-games](https://github.com/Team-Arcadia/arcadia-games) | 32 competitive minigames with scoring, leaderboards and configurable rewards. No client install. |
| [Arcadia-Dungeon](https://github.com/Team-Arcadia/Arcadia-Dungeon) | Configurable dungeons with adaptive bosses, wave phases, rewards and leaderboards. |
| [arcadia-lootbox](https://github.com/Team-Arcadia/arcadia-lootbox) | Data-driven loot boxes with keys, multi-draw and a hub interface. |
| [arcadia-guard](https://github.com/Team-Arcadia/arcadia-guard) | Zone protection with 86 flags, a full in-game interface, LuckPerms integration and 3D zone rendering. |
| [arcadia-spawndimension](https://github.com/Team-Arcadia/arcadia-spawndimension) | Spawn dimension and lobby, random teleport, themed tab list and cross-server tools. |
| [arcadia-patchcreate](https://github.com/Team-Arcadia/arcadia-patchcreate) | Performance and stability patches for Create, each one toggleable and checked against a bytecode fingerprint. |
| [arcadia-tweaks](https://github.com/Team-Arcadia/arcadia-tweaks) | Modular Mixin-based optimizations for the modpack (BotanyPots, Mekanism...), every patch behind its own toggle. |

<a name="mods-for-everyone"></a>

### Mods for everyone

Maintained by Team Arcadia, but **not made for Arcadia**: they have no dependency on our server and can be used in any
modpack or on any server.

| Mod | What it does | Side |
|---|---|---|
| [mods-mc-rspolymorph](https://github.com/Team-Arcadia/mods-mc-rspolymorph) | Recipe selection in the Refined Storage crafting and pattern grids, no Polymorph needed. NeoForge and Fabric. On [CurseForge](https://www.curseforge.com/minecraft/mc-mods/rs-polymorph). | Both |
| [mods-mc-creative-admin](https://github.com/Team-Arcadia/mods-mc-creative-admin) | Server-enforced creative mode restrictions: named profiles define what players may take. | Server |
| [mods-mc-customperm](https://github.com/Team-Arcadia/mods-mc-customperm) | Grant vanilla and modded commands to non-op players with fine-grained permissions. | Server |
| [mods-mc-better-creative](https://github.com/Team-Arcadia/mods-mc-better-creative) | Sort, pin and hide creative inventory tabs. Works on vanilla servers. | Client |

<a name="forks-we-maintain"></a>

### Forks we maintain

The Arcadia modpack runs more than 440 mods. When one of them crashes or conflicts with another, we fix it in a fork and
ship the fixed build in the pack. Each fork keeps the original license and credits; our changes live on a dedicated
branch (`Arcadia-fix` when the fork has several branches) and are described in its README.

| Fork | Original mod | What we fix |
|---|---|---|
| [fork-mc-createthefactorymustgrow](https://github.com/Team-Arcadia/fork-mc-createthefactorymustgrow) | Create: The Factory Must Grow | Machines surviving chunk reloads, client/server separation, multiplayer hardening, electrical network performance |
| [fork-mc-playersync](https://github.com/Team-Arcadia/fork-mc-playersync) | PlayerSync | Player data synchronization across our servers through MySQL |
| [fork-mc-deeperanddarker](https://github.com/Team-Arcadia/fork-mc-deeperanddarker) | Deeper and Darker | Deep Dark expansion, 1.21.1 maintenance |
| [fork-mc-ecologics](https://github.com/Team-Arcadia/fork-mc-ecologics) | Ecologics | Renderer registration race during parallel client setup |
| [fork-mc-immersivemelodies](https://github.com/Team-Arcadia/fork-mc-immersivemelodies) | Immersive Melodies | Launch crash on NeoForge 1.21.1 |
| [fork-mc-animalGardenowl](https://github.com/Team-Arcadia/fork-mc-animalGardenowl) | AnimalGarden Owl | Launch crash on NeoForge 1.21.1 |
| [fork-mc-createcentralkitchen](https://github.com/Team-Arcadia/fork-mc-createcentralkitchen) | Create: Central Kitchen | Compatibility with Farmer's Delight 1.3.1 |
| [fork-mc-endersdelight](https://github.com/Team-Arcadia/fork-mc-endersdelight) | Ender's Delight | Compatibility with Farmer's Delight 1.3.1 |
| [fork-mc-trailandtalesdelight](https://github.com/Team-Arcadia/fork-mc-trailandtalesdelight) | Trail and Tales Delight | Compatibility with Farmer's Delight 1.3.1 |

<a name="discord-bot"></a>

### Discord bot

| Repository | What it does |
|---|---|
| [discord-bot-arcadius](https://github.com/Team-Arcadia/discord-bot-arcadius) | Arcadius: AI-assisted conversations with memory, help detection and server information. Node.js and discord.js. |

<a name="website"></a>

### Website

[arcadia-echoes-of-power.fr](https://www.arcadia-echoes-of-power.fr) runs on [Azuriom](https://azuriom.com) with a custom
theme and in-house plugins: wiki, shop, votes, support, roadmap, creators space and staff tools. It talks to the game
servers through AzLink and to Discord through webhooks.

### About this repository

This is the special `.github` repository of the organization. `profile/README.md` is the page shown on the
[organization page](https://github.com/Team-Arcadia); community files placed here are used as defaults by every
repository that does not have its own. Only public repositories are listed on the profile.

### Contact

- Discord: [arcadia-echoes-of-power.fr/discord](https://arcadia-echoes-of-power.fr/discord)
- Email: [contact@arcadia-echoes-of-power.fr](mailto:contact@arcadia-echoes-of-power.fr)
- Website: [arcadia-echoes-of-power.fr](https://www.arcadia-echoes-of-power.fr)

<div align="right"><a href="#english">Back to top</a></div>

---

<a name="francais"></a>

## Français

La Team Arcadia fait tourner **Arcadia: Echoes Of Power**, un serveur Minecraft moddé français (NeoForge 1.21.1) où se
rencontrent la technologie Create, la magie et une économie joueur. L'équipe fait bien plus qu'un site web : elle écrit
ses propres mods, publie des mods pour toute la communauté Minecraft et maintient des versions corrigées des mods tiers
dont le modpack a besoin.

### Ce que nous faisons

| Famille | Préfixe | En bref |
|---|---|---|
| [Mods Arcadia](#mods-arcadia) | `arcadia-` | Mods écrits pour notre serveur et notre modpack : minijeux, donjons, protection, spawn, performances. |
| [Mods pour tous](#mods-pour-tous) | `mods-mc-` | Mods gérés par la Team Arcadia mais pas liés à Arcadia. Ils fonctionnent sur n'importe quel serveur ou modpack. |
| [Forks maintenus](#forks-maintenus) | `fork-mc-` | Mods tiers utilisés dans notre modpack, corrigés par nos soins pour régler crashs et incompatibilités. |
| [Bot Discord](#bot-discord) | `discord-bot-` | Arcadius, le bot de notre communauté Discord. |
| [Site web](#site-web) | `azuriom-` | Notre site Azuriom, son thème et ses plugins. |

Le guide complet (convention de nommage, fonctionnement d'ensemble, contribution) se trouve sur la
[page de l'organisation](https://github.com/Team-Arcadia).

### Comment on fonctionne : le nom des dépôts

Chaque nom de dépôt commence par un **préfixe qui indique sa famille**, suivi du nom du projet. On sait ce qu'est un
dépôt avant même de l'ouvrir.

| Famille | Nom du dépôt | Exemple | Règle |
|---|---|---|---|
| Mods Arcadia | `arcadia-<nom-du-mod>` | `arcadia-games`, `arcadia-guard` | Un mod fait pour le serveur ou le modpack Arcadia. |
| Mods pour tous | `mods-mc-<nom-du-mod>` | `mods-mc-rspolymorph` | Un mod géré par la Team Arcadia qui fonctionne sans Arcadia. |
| Forks | `fork-mc-<nom-du-mod-d-origine>` | `fork-mc-ecologics` | Le mod de quelqu'un d'autre que nous corrigeons. Le nom est celui du mod d'origine. |
| Site web | `azuriom-<nom-du-plugin>` | `azuriom-<plugin-id>` | Un plugin de notre site Azuriom. Le thème s'appelle `azuriom-theme-<nom>`. |
| Bots Discord | `discord-bot-<nom-du-bot>` | `discord-bot-arcadius` | Un bot qui tourne sur notre Discord. |
| Organisation | `.github` | `.github` | Ce dépôt : profil de l'organisation et fichiers communautaires par défaut. |

**Règles pour chaque dépôt**

1. **Minuscules uniquement**, mots séparés par des tirets : `arcadia-spawndimension`, jamais `Arcadia_SpawnDimension`.
2. **Le préfixe est obligatoire.** Il se choisit avec une seule question : *c'est notre mod pour Arcadia*
   (`arcadia-`), *notre mod pour tout le monde* (`mods-mc-`), ou *le mod de quelqu'un d'autre qu'on corrige*
   (`fork-mc-`) ?
3. **Le nom après le préfixe dit ce qu'est le projet** : le nom du mod pour un mod, le nom du projet d'origine pour un
   fork, le nom du plugin pour un plugin du site.
4. **Une description d'une phrase en anglais** et le topic `team-arcadia` sur chaque dépôt.
5. **Les forks gardent la licence et les crédits d'origine.** Nos correctifs vont sur une branche dédiée
   (`Arcadia-fix` si besoin).

> Quelques dépôts plus anciens sont antérieurs à cette convention, par exemple `Arcadia-Dungeon`. Ils seront renommés
> progressivement ; GitHub redirige automatiquement les anciens liens.

<a name="mods-arcadia"></a>

### Mods Arcadia

Faits *pour* le serveur et le modpack Arcadia. Ils tournent sur NeoForge 1.21.1 et la plupart sont uniquement côté
serveur : les joueurs n'ont rien de plus à installer.

| Mod | Ce qu'il fait |
|---|---|
| [arcadia-games](https://github.com/Team-Arcadia/arcadia-games) | 32 minijeux compétitifs avec scores, classements et récompenses configurables. Aucune installation côté client. |
| [Arcadia-Dungeon](https://github.com/Team-Arcadia/Arcadia-Dungeon) | Donjons configurables avec boss adaptatifs, phases de vagues, récompenses et classements. |
| [arcadia-lootbox](https://github.com/Team-Arcadia/arcadia-lootbox) | Coffres à butin pilotés par des données, avec clés, tirages multiples et interface hub. |
| [arcadia-guard](https://github.com/Team-Arcadia/arcadia-guard) | Protection de zones avec 86 flags, interface complète en jeu, intégration LuckPerms et rendu 3D des zones. |
| [arcadia-spawndimension](https://github.com/Team-Arcadia/arcadia-spawndimension) | Dimension de spawn et lobby, téléportation aléatoire, tablist thématique et outils inter-serveurs. |
| [arcadia-patchcreate](https://github.com/Team-Arcadia/arcadia-patchcreate) | Correctifs de performance et de stabilité pour Create, chacun activable et vérifié par empreinte de bytecode. |
| [arcadia-tweaks](https://github.com/Team-Arcadia/arcadia-tweaks) | Optimisations modulaires à base de Mixins pour le modpack (BotanyPots, Mekanism...), chaque correctif derrière son propre interrupteur. |

<a name="mods-pour-tous"></a>

### Mods pour tous

Gérés par la Team Arcadia, mais **pas faits pour Arcadia** : ils n'ont aucune dépendance à notre serveur et
s'utilisent dans n'importe quel modpack ou sur n'importe quel serveur.

| Mod | Ce qu'il fait | Côté |
|---|---|---|
| [mods-mc-rspolymorph](https://github.com/Team-Arcadia/mods-mc-rspolymorph) | Sélection de recette dans les grilles de craft et de patterns de Refined Storage, sans Polymorph. NeoForge et Fabric. Sur [CurseForge](https://www.curseforge.com/minecraft/mc-mods/rs-polymorph). | Les deux |
| [mods-mc-creative-admin](https://github.com/Team-Arcadia/mods-mc-creative-admin) | Restrictions du mode créatif imposées par le serveur : des profils nommés définissent ce que les joueurs peuvent prendre. | Serveur |
| [mods-mc-customperm](https://github.com/Team-Arcadia/mods-mc-customperm) | Accorder des commandes vanilla et moddées aux joueurs non-op avec des permissions fines. | Serveur |
| [mods-mc-better-creative](https://github.com/Team-Arcadia/mods-mc-better-creative) | Trier, épingler et masquer les onglets de l'inventaire créatif. Fonctionne sur les serveurs vanilla. | Client |

<a name="forks-maintenus"></a>

### Forks maintenus

Le modpack Arcadia compte plus de 440 mods. Quand l'un d'eux crashe ou entre en conflit avec un autre, nous le
corrigeons dans un fork et livrons la version corrigée dans le pack. Chaque fork conserve la licence et les crédits
d'origine ; nos modifications vivent sur une branche dédiée (`Arcadia-fix` quand le fork a plusieurs branches) et sont
décrites dans son README.

| Fork | Mod d'origine | Ce que nous corrigeons |
|---|---|---|
| [fork-mc-createthefactorymustgrow](https://github.com/Team-Arcadia/fork-mc-createthefactorymustgrow) | Create: The Factory Must Grow | Machines qui survivent au rechargement des chunks, séparation client/serveur, robustesse multijoueur, performances du réseau électrique |
| [fork-mc-playersync](https://github.com/Team-Arcadia/fork-mc-playersync) | PlayerSync | Synchronisation des données joueurs entre nos serveurs via MySQL |
| [fork-mc-deeperanddarker](https://github.com/Team-Arcadia/fork-mc-deeperanddarker) | Deeper and Darker | Extension du Deep Dark, maintenance 1.21.1 |
| [fork-mc-ecologics](https://github.com/Team-Arcadia/fork-mc-ecologics) | Ecologics | Concurrence à l'enregistrement des renderers pendant l'initialisation client parallèle |
| [fork-mc-immersivemelodies](https://github.com/Team-Arcadia/fork-mc-immersivemelodies) | Immersive Melodies | Crash au lancement sur NeoForge 1.21.1 |
| [fork-mc-animalGardenowl](https://github.com/Team-Arcadia/fork-mc-animalGardenowl) | AnimalGarden Owl | Crash au lancement sur NeoForge 1.21.1 |
| [fork-mc-createcentralkitchen](https://github.com/Team-Arcadia/fork-mc-createcentralkitchen) | Create: Central Kitchen | Compatibilité avec Farmer's Delight 1.3.1 |
| [fork-mc-endersdelight](https://github.com/Team-Arcadia/fork-mc-endersdelight) | Ender's Delight | Compatibilité avec Farmer's Delight 1.3.1 |
| [fork-mc-trailandtalesdelight](https://github.com/Team-Arcadia/fork-mc-trailandtalesdelight) | Trail and Tales Delight | Compatibilité avec Farmer's Delight 1.3.1 |

<a name="bot-discord"></a>

### Bot Discord

| Dépôt | Ce qu'il fait |
|---|---|
| [discord-bot-arcadius](https://github.com/Team-Arcadia/discord-bot-arcadius) | Arcadius : conversations assistées par IA avec mémoire, détection des demandes d'aide et informations serveur. Node.js et discord.js. |

<a name="site-web"></a>

### Site web

[arcadia-echoes-of-power.fr](https://www.arcadia-echoes-of-power.fr) tourne sur [Azuriom](https://azuriom.com) avec un
thème sur mesure et des plugins maison : wiki, boutique, votes, support, roadmap, espace créateurs et outils du staff.
Il communique avec les serveurs de jeu via AzLink et avec Discord via des webhooks.

### À propos de ce dépôt

C'est le dépôt spécial `.github` de l'organisation. `profile/README.md` est la page affichée sur la
[page de l'organisation](https://github.com/Team-Arcadia) ; les fichiers communautaires placés ici servent de fichiers
par défaut à tous les dépôts qui n'ont pas les leurs. Seuls les dépôts publics sont listés sur le profil.

### Contact

- Discord : [arcadia-echoes-of-power.fr/discord](https://arcadia-echoes-of-power.fr/discord)
- Email : [contact@arcadia-echoes-of-power.fr](mailto:contact@arcadia-echoes-of-power.fr)
- Site web : [arcadia-echoes-of-power.fr](https://www.arcadia-echoes-of-power.fr)

<div align="right"><a href="#francais">Retour en haut</a></div>

---

<div align="center">
<sub>© 2026 Arcadia: Echoes Of Power · Maintained by Team Arcadia · Lead development: vyrriox</sub><br/>
<sub>Not affiliated with Mojang Studios or Microsoft.</sub>
</div>
