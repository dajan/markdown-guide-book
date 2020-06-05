# Pense bête {#cheat-sheet}

Cette fiche de référence donne un aperçu rapide de tous les éléments de la syntaxe de Markdown. Elle ne peut pas couvrir tous les cas de figure ! Si vous avez besoin de plus d'informations sur l'un de ces éléments, reportez-vous aux chapitres [Syntaxe de base](#basic-syntax) et [Syntaxe étendue](#extended-syntax).

## Syntaxe de base

La syntaxe de base concerne les éléments décrits dans le document de conception original de John Gruber. Toutes les applications Markdown prennent en charge ces éléments.

| Élément           | Symtaxe Markdown                                      |
|-------------------|------------------------------------------------------|
| [Titre](#headings)  | `# H1`                                           |
|                   | `## H2`                                              |
|                   | `### H3`                                             |
|-------------------|------------------------------------------------------|
| [Gras](#bold)     | `**texte en gras**`                                      |
|-------------------|------------------------------------------------------|
| [Italique](#italic) | `*texte en italique*`                                  |
|-------------------|------------------------------------------------------|
| [Citation](#blockquotes) |  `> citation`                             |
|-------------------|------------------------------------------------------|
| [Liste numérotée](#ordered-lists)   | `1. Premier élément`                       |
|                   | `2. Deuxième élément`                                     |
|                   | `3. Trosième élément`                                      |
|-------------------|------------------------------------------------------|
| [Liste à puces](#unordered-lists) | `- Premier élément`                      |
|                   | `- Deuxième élément`                                      |
|                   | `- Troisième élément`                                       |
|-------------------|------------------------------------------------------|
| [Code informatique](#code)     | `` `code` ``                                         |
|-------------------|------------------------------------------------------|
| [Ligne horizontale](#horizontal-rules)   |  `---`                          |
|-------------------|------------------------------------------------------|
| [Lien](#links)    |  `[titre du lien](https://www.exemple.ch)`                  |
|-------------------|------------------------------------------------------|
| [Image](#images)  |  `![texte de remplacement](image.jpg)`                            |


## Syntaxe étendue

Ces éléments prolongent la syntaxe de base en y ajoutant des caractéristiques supplémentaires. Toutes les applications Markdown ne prennent pas en charge ces éléments.

| Élément           | Syntaxe Markdown                                      |
|-------------------|------------------------------------------------------|
| [Table](#tables)  | `| Syntaxe | Description |`                           |
|                   | `| ------ | ----------- |`                           |
|                   | `| En-tête | Titre |`                                 |
|                   | `| Paragraphe | Texte |`                              |
|-------------------|------------------------------------------------------|
| [Bloc de code encadré](#fenced-code-blocks) | ```` ``` ````                 |
|                   | `{`                                                  |
|                   |   `"prenom": "Dominique-Alain",`                             |
|                   |   `"nom": "Jan",`                             |
|                   |   `"age": 54`                                        |
|                   | `}`                                                  |
|                   | ```` ``` ````                                        |
|-------------------|------------------------------------------------------|
| [Note de pas de page](#footnotes)  | `Une phrase avec un renvoi à une note de bas de page. [^1]`      |
|                   |                                                      |
|                   | `[^1]: Ceci est la note de bas de page.`                        |
|-------------------|------------------------------------------------------|
| [Titre ID](#heading-ids)  | `### Mon beau titre {#votre-id}`        |
|-------------------|------------------------------------------------------|
| [Liste de définitions](#definition-lists)  | `terme à définir`                           |
|                   | `: définition`                                       |
|-------------------|------------------------------------------------------|
| [Barré](#strikethrough)  | `~~Le monde est plat.~~`              |
|-------------------|------------------------------------------------------|
| [Liste de tâches](#task-lists)  | `- [x] Écrire la présentation du livre`              |
|                   | `- [ ] Mettre à jour le site web`                           |
|                   | `- [ ] Contacter les médias`                            |

