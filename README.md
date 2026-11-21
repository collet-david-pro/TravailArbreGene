# TravailArbreGene

**Arbre généalogique et génogramme professionnels, 100 % hors ligne, dans un seul fichier HTML.**

Cet outil sert à représenter rapidement la situation familiale d'un élève ou d'un usager. Il a été conçu pour les professionnels du médico-social et de l'éducation : infirmières scolaires, assistantes sociales, éducateurs, psychologues.

> 🔒 **Aucune donnée ne quitte votre ordinateur.** Pas d'installation, pas de compte, pas de serveur, pas de connexion Internet.

> 🤖 Outil conçu avec l'aide de l'IA ([Claude](https://claude.com/claude-code), Anthropic). Voir [Conception](#conception).

---

## Sommaire

- [Fonctionnalités](#fonctionnalités)
- [Démarrage rapide](#démarrage-rapide)
- [Lire l'arbre : les symboles](#lire-larbre--les-symboles)
- [Liens de parenté disponibles](#liens-de-parenté-disponibles)
- [Export PDF](#export-pdf)
- [Sauvegarde et partage](#sauvegarde-et-partage)
- [Confidentialité et RGPD](#confidentialité-et-rgpd)
- [Compatibilité](#compatibilité)
- [Pour les développeurs](#pour-les-développeurs)

---

## Fonctionnalités

| | |
|---|---|
| 👤 **Fiches personnes** | Prénom, nom, nom de naissance, sexe, date de naissance (âge calculé) ou âge saisi, profession, décès, notes libres. |
| 🔗 **Liens de parenté guidés** | Il suffit d'écrire une phrase : « *Léa* est la *demi-sœur* de *Tom* ». L'outil traduit le lien, pose les questions utiles (« Qui est l'autre parent ? ») et crée les parents inconnus si besoin. Un parent inconnu peut ensuite être **remplacé** par une personne déjà saisie. |
| 🌳 **Arbre automatique** | Le dessin se construit et se met à jour seul, sans aucun placement manuel. Les familles recomposées sont gérées : unions multiples, demi-fratries, beaux-parents. |
| ⭐ **Personne concernée** | L'élève ou l'usager suivi est mis en évidence au centre de l'arbre. |
| 🏠 **Foyers** | Indiquent qui vit avec qui (domicile de la mère, famille d'accueil…), avec un contour ou une pastille de couleur. |
| 💬 **Relations émotionnelles** | Proche, fusionnelle, distante, conflit, rupture, violence, emprise. Un code couleur léger s'affiche à la demande, sans surcharger l'arbre. |
| 📄 **Export PDF** | A4 ou A3 paysage, avec légende automatique et logo de l'établissement. En option : tableau détaillé et version anonymisée. |
| 💾 **Un fichier par famille** | Chaque dossier est enregistré en `.json` sur votre poste, et se rouvre ou se partage facilement. |
| ❓ **Tutoriel intégré** | Une aide pas à pas est disponible dans l'application, avec un exemple fictif pour s'entraîner. |
| ✅ **Contrôles de cohérence** | Alertes en cas d'âges incohérents, de plus de deux parents biologiques ou de liens impossibles. |

---

## Démarrage rapide

1. **Téléchargez** le fichier [`arbre-genealogique.html`](arbre-genealogique.html) (bouton *Download raw file* sur GitHub).
2. **Ouvrez-le** par double-clic dans Firefox ou Chrome.
3. Cliquez sur **« Voir le tutoriel »**, ou sur **« Charger l'exemple »** pour découvrir l'outil avec une famille fictive.
4. **Ajoutez** une première personne, puis reliez les suivantes : « X est le/la … de Y ».
5. **Enregistrez** le dossier (fichier `.json`), puis exportez-le en **PDF**.

> ⚠️ **Il n'y a pas de sauvegarde automatique.** Un indicateur « non enregistré » s'affiche, et le navigateur vous prévient si vous fermez la page sans avoir enregistré.

---

## Lire l'arbre : les symboles

L'outil suit les conventions usuelles du **génogramme**.

| Symbole | Signification |
|---|---|
| ■ carré | Homme |
| ● cercle | Femme |
| ◆ losange | Sexe non précisé |
| ✕ croix dans le symbole | Personne décédée |
| double contour coloré | Personne concernée (élève / usager) |
| symbole grisé, pointillé | Personne inconnue (créée automatiquement) |
| ── trait plein | Mariage / PACS, filiation biologique |
| ╌╌ trait tireté | Concubinage, adoption |
| ┈┈ trait pointillé | Accueil / placement |
| ─/─ | Séparation |
| ─//─ | Divorce |

Les **relations émotionnelles** sont signalées par des pastilles de couleur. Un clic sur une personne affiche ses relations ; la **vue relations** les montre toutes.

---

## Liens de parenté disponibles

Père / mère · fils / fille · frère / sœur · demi-frère / demi-sœur · frère / sœur par alliance · conjoint(e) · ex-conjoint(e) · grand-parent · petit-enfant · oncle / tante · neveu / nièce · cousin(e) · beau-père / belle-mère · beau-frère / belle-sœur · gendre / belle-fille · enfant adopté / placé · **lien libre** (parrain, référent…).

Ces liens sont **calculés** à partir des filiations et des unions : la fiche de chaque personne affiche automatiquement le lien inverse. Exemple : « Léa est la sœur de Tom », donc « Tom est le frère de Léa ».

---

## Export PDF

Le bouton **PDF** ouvre une fenêtre d'options, puis la boîte d'impression du navigateur. Choisissez-y la destination **« Enregistrer au format PDF »**.

- Format **A4 ou A3**, paysage. L'outil suggère l'A3 pour les grandes familles.
- **En-tête** : logo de l'établissement, titre, date, auteur.
- **Légende** limitée aux symboles réellement utilisés.
- **Page 2** (option) : tableau des personnes, de leurs liens et de leurs notes.
- **Anonymisation** (option) : initiales seulement, notes et dates de naissance retirées.
- **Pied de page** : *Document confidentiel, données à caractère personnel*.

Le PDF est **vectoriel** : il reste net à toutes les tailles.

---

## Sauvegarde et partage

- **Enregistrer** télécharge un fichier `famille-NOM-AAAA-MM-JJ.json`. Rangez-le dans votre dossier professionnel.
- **Ouvrir** recharge un fichier enregistré.
- **Partager** un dossier avec un ou une collègue consiste simplement à lui transmettre le fichier `.json` par les canaux internes habituels.

Le format JSON est lisible et documenté. Vos données ne sont jamais enfermées dans l'outil.

---

## Confidentialité et RGPD

- **Fonctionnement 100 % local** : aucune requête réseau. Une politique de sécurité (*Content-Security-Policy*) intégrée au fichier **interdit au navigateur toute connexion sortante**, ce qui se vérifie facilement.
- **Aucun stockage caché** : ni cookie, ni `localStorage`, ni base de données du navigateur. Les données n'existent que dans la page ouverte et dans les fichiers que vous enregistrez vous-même.
- **Aucun traçage**, aucune statistique, aucune police ou bibliothèque téléchargée.
- **Option d'anonymisation** pour les documents transmis à des tiers.

> La responsabilité du stockage des fichiers `.json` et des PDF revient à l'utilisateur et à sa structure. Rangez-les dans un espace professionnel sécurisé.

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
- **Dessin** en SVG ; mise en page PDF via `@media print` et `@page`.
- **Logique pure** (modèle, moteur de parenté, disposition) isolée entre les commentaires `/* @core-start */` et `/* @core-end */`. Elle est exposée par un objet `Core` testable dans Node.
- **Modèle de données** : `personnes`, `unions`, `filiations`, `foyers`, `relations`, `liensLibres`. Les liens « métier » (frère, cousin…) ne sont jamais stockés : ils sont recalculés.

```
arbre-genealogique.html   application complète
exemple-famille.json      dossier fictif de démonstration
```

---

## Conception

Cet outil a été **conçu et développé avec l'aide de l'intelligence artificielle** : [Claude](https://claude.com/claude-code), l'assistant d'Anthropic, utilisé via Claude Code. Le projet est piloté par David Collet, qui a défini les besoins avec des professionnelles de terrain, puis testé et validé chaque fonctionnalité.

L'IA n'intervient qu'à la conception : **l'application elle-même n'utilise aucune IA** et ne se connecte à aucun service.
