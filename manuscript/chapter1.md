# Pour commencer {#getting-started}

Markdown est un langage simple, formé de balises placées dans un texte. Les balises permettent d'ajouter des éléments de formatage à des documents de texte brut. Créé par John Gruber en 2004, Markdown est aujourd'hui l'un des langages de balises les plus populaires au monde.

L'utilisation de Markdown est différente de celle d'un éditeur [WYSIWYG][1]. Dans une application comme Microsoft Word, vous cliquez sur des boutons pour formater des mots et des phrases, et les changements sont visibles immédiatement. Le travail en Markdown est différent. Lorsque vous créez un fichier formaté par Markdown, vous ajoutez la syntaxe Markdown au texte pour indiquer quels mots et phrases doivent avoir un aspect différent.

Par exemple, pour indiquer un titre, vous ajoutez un dièse avant celui-ci (par exemple, `# Titre Un`). Ou pour mettre une phrase en gras, vous ajoutez deux astérisques avant et après celle-ci (par exemple, `**ce texte est en gras**`). Il vous faudra peut-être un certain temps pour vous habituer à voir la syntaxe de Markdown dans votre texte, surtout si vous êtes habitué aux applications WYSIWYG. La capture d'écran ci-dessous montre un fichier Markdown affiché dans [l’éditeur de textes Atom][2].

![Ficher Markdown dans l'éditeur de textes Atom][image-1]

Vous pouvez ajouter des éléments de formatage Markdown à un fichier de texte en clair à l'aide d'une application d'édition de texte. Ou vous pouvez utiliser l'une des nombreuses applications Markdown pour macOS, Windows, iOS, ou Androïd. Il existe également plusieurs applications web spécialement conçues pour écrire en Markdown.

Selon l'application que vous utilisez, il est possible que vous ne puissiez pas prévisualiser le document formaté en temps réel. Mais ce n'est pas grave. [Selon Gruber][3], la syntaxe de Markdown est conçue pour être lisible et discrète, de sorte que le texte des fichiers Markdown peut être lu par un être humain même s'il n'est pas rendu.

> L'objectif primordial de la syntaxe de formatage de Markdown est de la rendre aussi lisible que possible. L'idée est qu'un document formaté par Markdown doit pouvoir être publié tel quel, en texte brut, sans avoir l'air d'avoir été marqué avec des balises ou des instructions de formatage.

## Pourquoi utiliser Markdown?

Vous vous demandez certainement pourquoi des personnes utilisent Markdown plutôt que des traitements de textes WYSIWYG. Pourquoi écrire en Markdown lorsqu’on presser des boutons avec une souris pour mettre en forme sont texte ? En fait, il y a plusieurs raisons qui poussent des rédacteurs à utiliser Markdown à la place, ou en amont, d’un traitement de textes WYSIWYG.

- Markdown est universel. Des rédacteurs l’utilise pour créer des sites Web, des documents, des notes, des livres, des présentations, des courriels, ou des manuels techniques.

- Markdown est portable. Des fichiers textes formatés en Markdown peuvent être ouverts par n’importe quel application qui permet de lire du texte. Si vous décidez que vous n’aimez plus l’éditeur Markdown que vous utilisez jusqu’à présent, vous pouvez importer vos fichiers dans n’importe quel autre application Markdown. Ceci marque une profonde différence avec les traitement de textes habituels comme Microsoft Word qui enferment votre texte dans un format de fichier propriétaire.

- Markdown est indépendant de toute plateforme. Vous pouvez créer du texte en Markdown-formatted sur n’importe quelle machine avec n’importe quel système d’exploitation.

- Markdown est intemporel. Même si l’application que vous utilisez aujourd’hui pour créer vos textes en Markdown cesse d’exister, vous serez toujours à même de lire les fichiers en Markdown en utilisant n’importe quelle application de gestion de textes. Ce point est très important pour les rédacteurs de livres, de thèses universitaires, ou d’autres documents importants qui doivent être préservés et accessibles sur le long terme.

- Markdown omniprésent. Des sites Web comme Reddit ou GitHub supportent Markdown, ainsi qu’un grand nombre d’application de bureau ou basées sur des services en ligne.

## Bien démarrer avec Markdown

La meilleure façon de commencer avec Markdown est de l'utiliser. Ceci est plus facile que jamais grâce à une série d'outils gratuits.

Vous n'avez même pas besoin de télécharger quoi que ce soit. Il existe plusieurs éditeurs de Markdown en ligne que vous pouvez utiliser pour essayer d'écrire dans Markdown. [Dillinger]() est l'un des meilleurs éditeurs en ligne de Markdown. Il suffit d'ouvrir le site et de commencer à taper dans le panneau de gauche. Un aperçu du document mis en page apparaît dans le panneau de droite.

![L'éditeur Makdown en ligne Dillinger est gratuit et facile à utiliser pour bien débuter avec Markdown.][image-2]

Vous pouvez très bien garder le site Web de Dillinger ouvert pendant que vous lisez ce guide et vous pourrez ainsi essayer la syntaxe au fur et à mesure que vous vous familiariserez avec elle. Une fois que vous vous serez familiarisé avec le système Markdown, vous voudrez peut-être utiliser une application Markdown qui peut être installée sur votre ordinateur de bureau ou votre appareil mobile.

## Comment fonctionne Markdown {#how-markdown-works}

Dillinger rend l'écriture dans Markdown facile parce qu'il cache les choses qui se passent en coulisses, mais il vaut la peine d'explorer comment le processus fonctionne en général.

Lorsque vous écrivez dans Markdown, le texte est stocké dans un fichier en texte clair qui a une extension « `.md` » ou « `.markdown` ». Mais alors comment votre fichier au format Markdown est-il converti en HTML ou en un document prêt à être imprimé ?

La réponse courte est que vous avez besoin d'une application *Markdown* capable de traiter le fichier Markdown. Il existe de nombreuses applications disponibles, allant de simples scripts à des applications de bureau ressemblant à Microsoft Word. Malgré leurs différences visuelles, toutes ces applications font la même chose. Comme Dillinger, elles convertissent toutes le texte formaté en Markdown en HTML, pour qu'il puisse être affiché dans les navigateurs Web.

Les applications Markdown utilisent un *processeur Markdown* (également appelé « analyseur » ou parle aussi d’« implémentation ») pour lire le texte au format Markdown et le transformer en HTML. À ce stade, votre document peut être visualisé dans un navigateur Web ou combiné avec une feuille de style puis imprimé. Vous pouvez voir ci-dessous le schéma de ce processus.

I\> L'application Markdown et le processeur sont deux composants distincts. Toutefois, par souci de concision, je les ai combinés en un seul élément (« Markdown App ») dans la figure ci-dessous.

{width=70%}
![Schéma représentant le processus d'écriture en Markdown.][image-3]

Pour résumer, il s'agit d'un processus en quatre parties :

1. Créer un fichier Markdown à l'aide d'un éditeur de texte ou d'une application dédiée à Markdown. Le fichier doit avoir une extension « `.md` » «`.markdown` ».
2. Ouvrir le fichier Markdown dans une application Markdown.
3. Utiliser l'application Markdown pour convertir le fichier en Markdown en un document HTML.
4. Visualiser le fichier HTML dans un navigateur Web ou utiliser l'application Markdown pour le convertir dans un autre format de fichier; par exemple en PDF.

De votre côté, le processus variera peut-être quelque peu en fonction de l'application que vous utilisez. Par exemple, Dillinger combine essentiellement les étapes 1 à 3 dans une interface unique et transparente – tout ce que vous avez à faire est de taper dans le panneau gauche et le résultat final apparaît comme par magie dans le panneau droit. Mais si vous utilisez d'autres outils, comme un éditeur de texte avec un générateur de site Web statique, vous constaterez que le processus est beaucoup plus visible.

## Un Markdown, plusieurs saveurs

L'un des aspects les plus déroutants de l'utilisation de Markdown est que pratiquement chaque application Markdown met en œuvre une version légèrement différente de Markdown. Ces variantes du langage sont communément appelées *saveurs*. Il vous appartient de maîtriser la saveur de Markdown que votre application propose d’utiliser. 

Pour comprendre le concept des saveurs Markdown, il peut être utile de les considérer comme des dialectes. Les habitants de Ciudad Juárez parlent l'espagnol tout comme ceux de Barcelone, mais il existe des différences substantielles entre les dialectes utilisés dans les deux villes. Il en va de même pour les personnes utilisant différentes applications de la démarque. Utiliser [Dillinger][5] pour écrire avec Markdown est une expérience très différente de l'utilisation d'[Ulysse][6].

En pratique, cela signifie que vous ne savez jamais exactement ce qu'un logiciel veut dire lorsqu'elle dit qu'elle supporte le codage en Markdown. Parle-t-on seulement de la [syntaxe de base][7], ou de tous les éléments syntaxiques de base et [d’éléments syntaxiques étendus][8] combinés, ou d'une combinaison arbitraire d'éléments syntaxiques ? Vous ne le saurez pas tant que vous n'aurez pas lu la documentation ou commencé à utiliser l'application.

Si vous débutez, le meilleur conseil que je puisse vous donner est de choisir une application Markdown avec un bon support Markdown. Cela contribuera grandement à maintenir la portabilité de vos fichiers Markdown. Vous pourriez vouloir stocker et utiliser vos fichiers Markdown dans d'autres applications, et pour ce faire, vous devez commencer avec une application qui offre un bon support. Vous pouvez utiliser le [répertoire des outils][9] pour trouver une application qui vous convient.

## Ressources supplémentaires

Il existe de nombreuses autres ressources que vous pouvez utiliser pour apprendre le Markdown. Voici quelques-unes de mes favorites :

- [John Gruber’s Markdown documentation][10]. Le guide original écrit par le créateur de Markdown.
- [Markdown Tutorial][11]. Un site web *open source* qui vous permet de tester Markdown directement dans votre navigateur.
- [Awesome Markdown][12]. Un liste d’outils Markdown et d’autres ressources d’apprentissage du langage.
- [Typesetting Markdown][13]. Une série de plusieurs articles qui décrivent un écosystème pour éditer des documents en Markdown en utilisant [pandoc][14] et [ConTeXt][15].

[1]:	https://en.wikipedia.org/wiki/WYSIWYG
[2]:	https://atom.io
[3]:	http://daringfireball.net/projects/markdown/
[5]:	https://www.markdownguide.org/tools/dillinger/
[6]:	https://www.markdownguide.org/tools/ulysses/
[7]:	#basic-syntax
[8]:	#extended-syntax
[9]:	https://www.markdownguide.org/tools/
[10]:	https://daringfireball.net/projects/markdown/
[11]:	https://www.markdowntutorial.com/
[12]:	https://github.com/mundimark/awesome-markdown
[13]:	https://dave.autonoma.ca/blog/2019/05/22/typesetting-markdown-part-1
[14]:	https://pandoc.org/
[15]:	https://www.contextgarden.net/

[image-1]:	images/atom.png
[image-2]:	images/dillinger.png
[image-3]:	images/process.png