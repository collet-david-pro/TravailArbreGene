<p align="center">
  <img src="docs/banner.svg" alt="TravailArbreGene" width="820">
</p>

<p align="center">
  <b>Arbre généalogique et génogramme professionnels, 100 % hors ligne, dans un seul fichier HTML.</b><br>
  Pensé pour les infirmières scolaires, les assistantes sociales et tous les professionnels de l'accompagnement.
</p>

<p align="center">
  <a href="https://github.com/collet-david-pro/TravailArbreGene/releases/latest/download/arbre-genealogique.html"><img src="https://img.shields.io/badge/T%C3%A9l%C3%A9charger-arbre--genealogique.html-d9772b?style=for-the-badge" alt="Télécharger"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/hors%20ligne-100%25-34495e" alt="Hors ligne">
  <img src="https://img.shields.io/badge/RGPD-aucune%20donn%C3%A9e%20transmise-34495e" alt="RGPD">
  <img src="https://img.shields.io/badge/installation-aucune-34495e" alt="Sans installation">
  <img src="https://img.shields.io/badge/d%C3%A9pendances-0-34495e" alt="Zéro dépendance">
  <img src="https://img.shields.io/badge/navigateurs-Firefox%20%7C%20Chrome-34495e" alt="Navigateurs">
  <a href="LICENSE"><img src="https://img.shields.io/badge/licence-MIT-34495e" alt="Licence MIT"></a>
</p>

<p align="center">
  <img src="docs/captures/arbre.png" alt="Vue de l'arbre d'une famille recomposée (exemple fictif)" width="900">
</p>

> 🔒 **Aucune donnée ne quitte votre ordinateur.** Pas de compte, pas de serveur, pas de connexion Internet. Un double-clic sur le fichier, et c'est parti.
>
> 🤖 Outil conçu avec l'aide de l'IA ([Claude](https://claude.com/claude-code), Anthropic). Voir [Conception](#conception).

---

## Sommaire

- [Pourquoi cet outil ?](#pourquoi-cet-outil-)
- [Fonctionnalités](#fonctionnalités)
- [Captures d'écran](#captures-décran)
- [Démarrage rapide](#démarrage-rapide)
- [Lire l'arbre : symboles et icônes](#lire-larbre--symboles-et-icônes)
- [Liens de parenté](#liens-de-parenté)
- [Documents produits : PDF, image, synthèse](#documents-produits--pdf-image-synthèse)
- [Sauvegarde et partage](#sauvegarde-et-partage)
- [Confidentialité et RGPD](#confidentialité-et-rgpd)
- [Compatibilité](#compatibilité)
- [Pour les développeurs](#pour-les-développeurs)
- [Conception](#conception)
- [Licence](#licence)

---

## Pourquoi cet outil ?

Comprendre une situation familiale (divorces, familles recomposées, demi-frères et sœurs, placement…) prend du temps, et la dessiner à la main en prend encore plus. Les logiciels de généalogie existants sont pensés pour les loisirs, souvent en ligne, et peu compatibles avec des **données sensibles de mineurs**.

**TravailArbreGene** répond à trois besoins :

1. **Saisir vite**, avec de simples formulaires en français : « *Léa* est la *demi-sœur* de *Tom* ».
2. **Visualiser tout de suite** un génogramme propre, qui se met à jour seul.
3. **Produire un document** (PDF, image ou texte de synthèse) à joindre à un dossier, **sans jamais rien envoyer sur Internet**.

---

## Fonctionnalités

### Saisie

| | |
|---|---|
| 👤 **Fiches personnes** | Prénom, nom, nom de naissance, sexe, date de naissance (âge calculé automatiquement) ou âge, profession, décès, notes. |
| 🔗 **Liens guidés** | Une simple phrase : « X est le/la … de Y ». L'outil pose les bonnes questions (« Qui est l'autre parent ? », « Par quel parent ? ») et crée les parents inconnus si besoin. |
| ⚡ **Boutons rapides** | Depuis la fiche d'une personne : **+ Enfant**, **+ Parent**, **+ Frère/sœur**, **+ Conjoint**. |
| 🔄 **Parent inconnu remplaçable** | Le jour où vous savez qui c'est, remplacez le « Parent inconnu » par une personne déjà saisie : tous les liens sont reportés. |
| ↶ **Annuler / Rétablir** | Ctrl+Z / Ctrl+Y (Cmd+Z sur Mac), 50 niveaux. |
| ✅ **Contrôles de cohérence** | Alertes en cas d'âge incohérent, de plus de deux parents biologiques ou de boucle impossible dans l'arbre. |

### Contenu métier

| | |
|---|---|
| ⭐ **Personne concernée** | L'élève ou l'usager suivi est mis en évidence. |
| 📋 **Situation administrative** | Autorité parentale, résidence, mesure en cours (AED, AEMO, placement ASE ou judiciaire, tutelle), établissement et classe. |
| 📅 **Date de référence** | Tous les âges sont calculés « au JJ/MM/AAAA ». Un dossier rouvert un an plus tard reste cohérent. |
| 🏠 **Foyers** | Qui vit avec qui (domicile de la mère, famille d'accueil…), repéré par couleur. |
| 💬 **Relations** | Proche, fusionnelle, distante, conflit, rupture, violence, emprise. Chacune a son **icône** et s'affiche à la demande, sans surcharger l'arbre. |
| 👶 **Symboles complets** | Grossesse en cours, fausse couche, enfant mort-né, **jumeaux**. |

### Affichage

| | |
|---|---|
| 🌳 **Arbre automatique** | Disposition par générations. Les frères et sœurs sont classés par âge (aîné à gauche), chaque couple a sa propre ligne, et les familles recomposées sont lisibles. |
| 🗺️ **Légende intégrée** | Un cartouche sur l'arbre ne liste que les symboles réellement utilisés. |
| 🎯 **Vue centrée** | Pour les grandes familles : seules les personnes proches de l'élève restent affichées (profondeur 1 à 4). |
| 🔍 **Zoom et déplacement** | Molette ou boutons + / − / recentrer. |
| ❓ **Tutoriel intégré** | Une aide pas à pas et un **exemple fictif** pour s'entraîner. |

### Documents

| | |
|---|---|
| 📄 **PDF** | A4 ou A3, en-tête avec logo et nom de l'établissement, légende sur l'arbre et en fin de document. En option : tableau détaillé des personnes et version anonymisée. |
| 🖼️ **Image** | Export PNG ou SVG de l'arbre, pour l'insérer dans Word ou dans un rapport. |
| 📝 **Synthèse texte** | Un paragraphe rédigé qui décrit la composition familiale, prêt à copier-coller dans un écrit professionnel. Il peut être anonymisé. |

---

## Captures d'écran

*Toutes les données affichées sont fictives.*

<table>
  <tr>
    <td width="50%"><img src="docs/captures/relations.png" alt="Relations de la personne sélectionnée"><br><sub><b>Clic sur une personne</b> : ses relations apparaissent en arcs avec leur icône, et sa fiche s'affiche en bas.</sub></td>
    <td width="50%"><img src="docs/captures/synthese.png" alt="Synthèse texte"><br><sub><b>Synthèse</b> : un texte rédigé automatiquement, à copier dans un rapport.</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="docs/captures/fiche.png" alt="Fiche personne"><br><sub><b>Fiche personne</b> avec la situation administrative.</sub></td>
    <td width="50%"><img src="docs/captures/arbre.png" alt="Arbre complet"><br><sub><b>Arbre complet</b> : demi-fratries, jumelles, grossesse en cours, foyers et légende.</sub></td>
  </tr>
</table>

---

## Démarrage rapide

1. **Téléchargez** [`arbre-genealogique.html`](https://github.com/collet-david-pro/TravailArbreGene/releases/latest/download/arbre-genealogique.html), depuis la dernière version publiée.
2. **Ouvrez-le** par double-clic dans Firefox ou Chrome.
3. Cliquez sur **« Charger l'exemple »** pour découvrir l'outil, ou sur **« Voir le tutoriel »**.
4. Pour un vrai dossier : **Nouveau dossier**, puis renseignez **Dossier** (titre, établissement, logo, date de référence).
5. Ajoutez la personne concernée, puis sa famille avec les boutons **+ Parent**, **+ Frère/sœur**…
6. **Enregistrez** le fichier `.json`, puis exportez en **PDF**, en **Image** ou en **Synthèse**.

> ⚠️ **Il n'y a pas de sauvegarde automatique** : c'est voulu, pour ne rien laisser dans le navigateur. Un indicateur « non enregistré » s'affiche, et le navigateur vous prévient si vous fermez la page sans avoir enregistré.

---

## Lire l'arbre : symboles et icônes

L'outil suit les conventions du **génogramme**.

| Symbole | Signification | | Trait | Signification |
|---|---|---|---|---|
| ■ carré | Homme | | ── plein | Mariage / PACS, filiation biologique |
| ● cercle | Femme | | ╌╌ tireté | Concubinage, adoption |
| ◆ losange | Sexe non précisé | | ┈┈ pointillé | Accueil / placement |
| ☒ croix | Personne décédée | | ─/─ | Séparation |
| ▲ triangle | Grossesse en cours | | ─//─ | Divorce |
| • petit cercle plein | Fausse couche | | ⋀ traits joints | Jumeaux |
| contour orange | Personne concernée | | | |
| grisé pointillé | Personne inconnue | | | |

**Relations** : ♥ proche · ⚭ fusionnelle · ↔ distante · ⚡ conflit · ✂ rupture · ⚠ violence · 🔒 emprise.
Les icônes apparaissent à côté des personnes concernées. Un clic sur une personne affiche ses relations en arcs ; le bouton **Vue relations** les montre toutes.

---

## Liens de parenté

Père / mère · fils / fille · frère / sœur · demi-frère / demi-sœur · frère / sœur par alliance · conjoint(e) · ex-conjoint(e) · grand-parent · petit-enfant · oncle / tante · neveu / nièce · cousin(e) · beau-père / belle-mère · beau-frère / belle-sœur · gendre / belle-fille · enfant adopté / placé · **lien libre** (parrain, référent, meilleur ami…).

Les liens sont **calculés**, jamais saisis deux fois. Exemple : si « Léa est la sœur de Tom », la fiche de Tom indique automatiquement « Tom est le frère de Léa ». Deux enfants qui ont les mêmes parents sont « frère et sœur » ; un seul parent en commun, et l'outil indique « demi-frère / demi-sœur ».

---

## Documents produits : PDF, image, synthèse

**PDF** (bouton *Exporter en PDF*, puis « Enregistrer au format PDF » dans la fenêtre d'impression) :
- format A4 ou A3 paysage ; l'outil suggère l'A3 pour les grandes familles ;
- en-tête avec logo, nom de l'établissement, titre, date de référence et auteur ;
- légende dessinée sur l'arbre, plus une légende complète en fin de document ;
- en option : tableau des personnes (avec la situation administrative), tableau des relations, version anonymisée ;
- pied de page *Document confidentiel, données à caractère personnel* ;
- PDF vectoriel, net à toutes les tailles.

**Image** : PNG (haute définition) ou SVG, avec la légende, et anonymisation possible.

**Synthèse** : un texte rédigé, centré sur l'élève. Il donne sa scolarité, son foyer, ses parents et leur situation de couple, ses beaux-parents, sa fratrie (frères et sœurs, demi-frères et demi-sœurs), ses grands-parents, l'autorité parentale, sa résidence, la mesure en cours et ses relations significatives. Le texte reste modifiable avant d'être copié.

**Anonymisation** : les noms sont remplacés par des initiales. Les notes, le nom de l'établissement, le logo, le nom des foyers et les précisions libres sont retirés.

---

## Sauvegarde et partage

- **Enregistrer** télécharge un fichier `famille-NOM-AAAA-MM-JJ.json`. Rangez-le dans votre espace professionnel.
- **Ouvrir** recharge un fichier enregistré.
- **Partager** un dossier avec un ou une collègue revient à lui transmettre ce fichier par les canaux internes habituels.

Le format JSON est lisible et documenté : vos données ne sont jamais prisonnières de l'outil.

---

## Confidentialité et RGPD

- **100 % local** : une politique de sécurité (*Content-Security-Policy*) intégrée au fichier **interdit au navigateur toute connexion sortante**, ce qui se vérifie facilement.
- **Aucun stockage caché** : ni cookie, ni `localStorage`, ni base de données du navigateur. Les données n'existent que dans la page ouverte et dans les fichiers que vous enregistrez vous-même.
- **Aucun traçage**, aucune statistique, aucune police ou bibliothèque téléchargée.
- **Anonymisation** des documents transmis à des tiers.

> La responsabilité du stockage des fichiers `.json` et des documents produits revient à l'utilisateur et à sa structure.

---

## Compatibilité

| Navigateur | Statut |
|---|---|
| Firefox (récent) | ✅ |
| Chrome / Chromium (récent) | ✅ |
| Edge, Safari | non testés, probablement fonctionnels |

Le numéro de page du PDF n'apparaît que dans Chrome.

---

## Pour les développeurs

- **Un seul fichier** : HTML + CSS + JavaScript vanilla, sans framework, sans dépendance et sans étape de compilation.
- **Dessin** en SVG ; mise en page PDF via `@media print` et `@page` ; export PNG par canvas.
- **Logique pure** (modèle, moteur de parenté, disposition, synthèse) isolée entre `/* @core-start */` et `/* @core-end */`. Elle est exposée par l'objet `Core`, testable dans Node.
- **Modèle de données** : `dossier`, `personnes`, `unions`, `filiations`, `foyers`, `relations`, `liensLibres`. Les liens « métier » (frère, cousin…) ne sont jamais stockés : ils sont recalculés.

```
arbre-genealogique.html   application complète
exemple-famille.json      dossier fictif de démonstration
docs/                     logo, bannière et captures d'écran
```

---

## Conception

<img src="docs/logo.png" alt="Logo" width="64" align="right">

Cet outil a été **conçu et développé avec l'aide de l'intelligence artificielle** : [Claude](https://claude.com/claude-code), l'assistant d'Anthropic, utilisé via Claude Code. Le projet est piloté par David Collet, qui a défini les besoins avec des professionnelles de terrain, puis testé et validé chaque fonctionnalité.

L'IA n'intervient qu'à la conception : **l'application elle-même n'utilise aucune IA** et ne se connecte à aucun service.

---

## Licence

Ce projet est distribué sous **licence [MIT](LICENSE)**, libre et open source. Vous pouvez l'utiliser, le copier, le modifier, le partager et le redistribuer, y compris dans votre structure ou à des fins commerciales. La seule condition est de conserver la mention de copyright et le texte de la licence.

Le logiciel est fourni « tel quel », sans garantie.
