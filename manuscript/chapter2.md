# Réaliser des choses avec Markdown {#doing-things-with-markdown}

Maintenant que vous savez ce qu'est Markdown, vous vous demandez probablement ce que vous pouvez en faire. La réponse est : « à peu près tout ». Markdown est un moyen rapide et facile de prendre des notes, de créer du contenu pour un site web et de produire des documents prêts à imprimer.

Il ne faut pas longtemps pour apprendre la syntaxe de Markdown, et une fois que vous savez comment l'utiliser, vous pouvez écrire en utilisant Markdown à peu près partout. La plupart des gens utilisent Markdown pour créer du contenu pour le web, mais Markdown est bon pour formater n’importe quel texte : des messages électroniques aux listes d'épicerie.

Voici quelques exemples de ce que vous pouvez faire avec Markdown.

## Sites web

Markdown a été conçu pour le web, il n'est donc pas surprenant qu'il existe de nombreuses applications spécialement conçues pour la création de contenu de sites web.

Si vous recherchez la manière la plus simple possible de créer un site web avec des fichiers Markdown, consultez les sites [blot.im][1] et [smallvictori.es][2]. Une fois que vous vous êtes inscrit à l'un de ces services, un dossier est automatiquement créé dans votre Dropbox sur votre ordinateur. Il vous suffit de glisser et de déposer vos fichiers Markdown dans ce dossier et – pouf ! – ils se retrouvent transformé en site web. Rien de plus simple.

Si vous êtes familier avec le HTML, le CSS et le contrôle de version (Git ou CSV), consultez [Jekyll][3], un générateur de site statique, populaire, qui prend les fichiers Markdown et construit un site web HTML automatiquement. L'un des avantages de cette approche est que le service [GitHub Pages][4] fournit un hébergement gratuit pour les sites web générés par Jekyll. Si Jekyll n'est pas votre tasse de thé, choisissez simplement l'un des nombreux autres [générateurs de sites statiques][5] disponibles.

!\>J’ai utilisé Jekyll pour créer le site web [Markdown Guide][6]. Vous pouvez consulter le code source sur [GitHub][7].

Si vous souhaitez utiliser un système de gestion de contenu (CMS) pour alimenter votre site web, consultez [Ghost][8]. Il s'agit d'une plateforme de blogs libre et gratuite, avec un éditeur Markdown très agréable. Si vous êtes un utilisateur de WordPress, vous serez heureux d'apprendre qu'il existe un [support Markdown][9] pour les sites web hébergés sur WordPress.com. Les sites WordPress auto-hébergés peuvent utiliser le [plugin Jetpack][10].
Markdown was designed for the web, so it should come as no surprise that there are plenty of applications specifically designed for creating website content.

## Documents

Markdown n'a pas toutes les caractéristiques des traitements de texte comme Microsoft Word, mais il suffit pour créer des documents de base comme des devoirs et des lettres. Vous pouvez utiliser une application de création de documents Markdown pour créer et exporter des documents au format Markdown vers des fichiers PDF ou HTML. La format PDF est essentiel, car une fois que vous avez un document PDF, vous pouvez tout faire avec lui – l'imprimer, l'envoyer par e-mail ou le télécharger sur un site web.

Voici quelques applications de création de documents Markdown que nous recommandons :

- **Mac:** [MacDown][11], [iA Writer][12], ou [Marked][13]
- **iOS / Android:** [iA Writer][14]
- **Windows:** [ghostwriter][15] ou [Markdown Monster][16]
- **Linux:** [ReText][17] ou [ghostwriter][18]
- **Web:** [Dillinger][19] ou [StackEdit][20]

T\> [iA Writer][21] fournit des modèles pour prévisualiser, imprimer et exporter des documents au format Markdown. Par exemple, le modèle « Academic - MLA Style » qui met en retrait des paragraphes et ajoute un double espacement des phrases.

## Notes

À presque tous les égards, Markdown est la syntaxe idéale pour prendre des notes. Malheureusement, des outils comme [Evernote][22] ou [OneNote][23], deux des applications de prises de notes les plus populaires, ne supportent pas Markdown pour l’instant. La bonne nouvelle est que plusieurs autres applications de prise de notes *supportent* le langage Markdown :

- [Simplenote][24] est une application gratuite de prise de notes, disponible pour toutes les plateformes.
- [Notable][25] est une application de prise de notes qui fonctionne sur une variété de plateformes.
- [Bear][26] est une application proche de ce que propose Evernote. Elle est disponible pour les appareils Mac et iOS. Par défaut,  elle n'utilise pas la syntaxe Markdown standard, mais vous pouvez activer [le mode de compatibilité][27].
- [Boostnote][28] se présente comme une « application de prise de notes open source conçue pour les programmeurs ».

Si vous ne pouvez pas vous séparer d'Evernote, essayez [Marxico][29], un éditeur Markdown sur abonnement pour Evernote, ou utilisez le service [Markdown Here][30] avec le site web d'Evernote 

## Livres

Vous souhaitez publier un roman en auto-publication ? Essayez [Leanpub][31], un service qui prend vos fichiers au format Markdown et les transforme en livre électronique. Leanpub produit votre livre au format PDF, EPUB et MOBI. Si vous souhaitez créer des copies style livre de poche de votre livre, vous pouvez télécharger le fichier PDF vers un autre service tel que **[Kindle Direct Publishing][32]**. Pour en savoir plus sur l'écriture et l'auto-publication d'un livre à l'aide de Markdown, lisez [cet article de blog][33].

## Pràsentations

Croyez-le ou non, vous pouvez générer des présentations à partir de fichiers au format Markdown. Il faut un peu de temps pour s'habituer à créer des présentations dans Markdown, mais une fois que vous avez pris le coup de main, c'est beaucoup plus rapide et facile que d'utiliser une application comme PowerPoint ou Keynote. [Remarque][34] ([projet GitHub][35]) est un outil en ligne de diaporama Markdown très populaire, tout comme [Cleaver][36] ([projet GitHub][37]). Si vous utilisez un Mac et préférez utiliser une application, consultez [Deckset][38] ou [Marked][39].

## Email

Si vous envoyez beaucoup de courrier électronique et que vous êtes fatigué des contrôles de formatage disponibles sur les sites web de la plupart des fournisseurs de courrier électronique, vous serez heureux d'apprendre qu'il existe un moyen facile de rédiger des messages électroniques à l'aide de Markdown. [Markdown here][40] est une extension de navigateur web, gratuite et open-source, qui convertit le texte formaté par Markdown en HTML prêt à être envoyé.

## Documentation

Markdown est une solution naturelle pour la documentation technique. Les entreprises comme GitHub passent de plus en plus souvent à Markdown pour leur documentation – consultez leur [billet de blog][41] sur la façon dont GitHub a migré sa documentation au format Markdown avec [Jekyll][42]. Si vous rédigez de la documentation pour un produit ou un service, jetez un coup d'œil à ces outils pratiques :

- [Read the Docs][43] peut générer un site web de documentation à partir de vos fichiers Markdown open source. Il suffit de connecter votre dépôt GitHub à leur service et de pousser les fichiers (push) – Read the Docs fait le reste. Ils offrent également un [service pour les sociétés commerciales][44].
- [MkDocs][45] est un générateur de site statique simple et rapide qui est orienté vers la documentation technique. Les fichiers sources sont écrits en Markdown et organisés avec un seul fichier de configuration YAML. MkDocs possède plusieurs [thèmes de présentation][46], qui inclut celui du service [Read the Docs][47]. Un des derniers thèmes proposés est [MkDocs Material][48], qui reprend les éléments du service Material Design de Google.
- [Docusaurus][49] est un générateur de site statique conçu exclusivement pour la création de sites web de documentation. Il prend en charge les traductions, la recherche et le versionnage.
- [VuePress][50] est un générateur de site statique géré par [Vue][51] et optimisé pour la rédaction de documentations techniques.
- [Jekyll][52] a déjà été mentionné plus haut dans la section sur les sites web; mais c'est aussi une bonne option pour générer un site web de documentation à partir des fichiers Markdown. Si vous suivez cette voie, assurez-vous de consulter le page sur [le thème pour la documentation de Jekyll][53].

[1]:	https://blot.im
[2]:	https://smallvictori.es
[3]:	https://jekyllrb.com/
[4]:	https://pages.github.com/
[5]:	https://www.staticgen.com/
[6]:	https://www.markdownguide.org
[7]:	https://github.com/mattcone/markdown-guide
[8]:	https://ghost.org/
[9]:	https://en.support.wordpress.com/markdown/
[10]:	https://jetpack.com/support/markdown/
[11]:	https://macdown.uranusjr.com/
[12]:	https://ia.net/writer/
[13]:	https://marked2app.com/
[14]:	https://ia.net/writer/
[15]:	https://wereturtle.github.io/ghostwriter/
[16]:	https://markdownmonster.west-wind.com/
[17]:	https://github.com/retext-project/retext
[18]:	https://wereturtle.github.io/ghostwriter/
[19]:	https://dillinger.io
[20]:	https://stackedit.io/
[21]:	https://ia.net/writer/templates/
[22]:	https://evernote.com/
[23]:	https://www.onenote.com/
[24]:	https://simplenote.com/
[25]:	https://notable.md
[26]:	https://bear.app/
[27]:	https://bear.app/faq/Markup%20:%20Markdown/Markdown%20compatibility%20mode/
[28]:	https://boostnote.io/
[29]:	https://marxi.co/
[30]:	https://markdown-here.com/features.html#not-just-email
[31]:	https://leanpub.com/
[32]:	https://kdp.amazon.com/fr_FR/
[33]:	https://medium.com/techspiration-ideas-making-it-happen/how-i-wrote-and-published-my-novel-using-only-open-source-tools-5cdfbd7c00ca
[34]:	https://remarkjs.com
[35]:	https://github.com/gnab/remark
[36]:	https://jdan.github.io/cleaver/
[37]:	https://github.com/jdan/cleaver
[38]:	https://www.decksetapp.com/
[39]:	https://marked2app.com/
[40]:	https://markdown-here.com
[41]:	https://github.com/blog/1939-how-github-uses-github-to-document-github
[42]:	https://jekyllrb.com/
[43]:	https://readthedocs.org
[44]:	https://readthedocs.com/
[45]:	https://www.mkdocs.org/
[46]:	https://www.mkdocs.org/user-guide/styling-your-docs/
[47]:	https://readthedocs.org/
[48]:	https://squidfunk.github.io/mkdocs-material/
[49]:	https://docusaurus.io/
[50]:	https://vuepress.vuejs.org/
[51]:	https://vuejs.org/
[52]:	https://jekyllrb.com/
[53]:	https://idratherbewriting.com/documentation-theme-jekyll/