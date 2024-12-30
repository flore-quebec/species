
# Flore Québec

Ce dépôt contient les comptes-rendus pour toutes les espèces présentées sur le site de Flore Québec. Les comptes-rendus sont organisés par famille, puis par genre. Pour chaque espèce, l'information est contenue dans un seul fichier _markdown_ (`.md`) portant le nom de l'espèce (e.g. _Abies_balsamea.md_). Le format `markdown` facilite la mise en forme de texte en vue de l'intégration dans une page web.

## Structure du fichier `.md`

### Section photos

Les photos sont un élément très important des comptes-rendus. Si les photos sélectionnées sont bien choisies (et si de bonnes photos sont disponibles), il est souvent possible de se faire une idée de l'apparence et des éléments servant à identifier une espèce. Voici quelques critères à garder en tête lors de la sélection des photos:

- La première photo sert à représenter l'espèce sur le site. Cette photo doit être la plus représentative possible de ce qu'un observateur peut voir lorsqu'il rencontre l'espèce pour une première fois sur le terrain.
- Les photos suivantes devraient permettre de se faire une bonne idée de l'apparence d'une espèce à différents niveaux (aspect général, inflorescence, photos macros des fleurs, des fruits, photo de plus loin illustrant un parterre de l'espèce, bourgeon, écorce, etc.)
- Idéalement, les photos devraient illustrer les critères permettant l'identification

Toutes les photos proviennent de la plateforme iNaturalist et sont disponibles publiquement. Pour cette raison, il est impératif de sélectionner des photos ayant une licence permettant leur utilisation. **Les photos pouvant être utilisées ont obligatoirement une licence CC0, CC BY ou CC BY-NC**. Ces licences permettent une utilisation libre et non-commerciale dans la mesure où l'auteur de la photo est crédité. Les photos n'ayant pas une de ces licences seront rejetées.

Vous pouvez également utiliser l'explorateur de photos du site Flore Québec [https://florequebec.ca/photos](https://florequebec.ca/photos). Cet explorateur devrait grandement vous faciliter la tâche de recherche de photos.

#### Comment lister les photos?

La première partie du fichier `.md` contient les urls vers les photos qui sont présentées sur le site. Par exemple, le code suivant indique les photos à utiliser pour [_Cinna arundinacea_](https://github.com/frousseu/floreduquebecsp/blob/main/Esp%C3%A8ces/Poaceae/Cinna/Cinna_arundinacea.md). Plus spécifiquement, le code suivant indique que les photos 1, 3, 5 et 13 de l'observation iNaturalist [195220528](https://www.inaturalist.org/observations/195220528) doivent être utilisées, puis les photos 1 et 4 de l'observation [195220524](https://www.inaturalist.org/observations/195220524), la 5e photo de l'oservation [195226187](https://www.inaturalist.org/observations/195226187) et finalement la 4e photo de l'observation [195708914](https://www.inaturalist.org/observations/195708914). **Un nombre maximal de 8 photos seront utilisées et elles seront présentées dans l'ordre donné**. Il est primordial de respecter l'ordre voulu et la syntaxe présentée ici. À noter que si plusieurs photos proviennent d'une même observation, il faudra répéter les urls si les photos ne se suivent pas (_e.g._ 2 photos peuvent provenir d'une même observation avec la 1ère photo listée en premier et la 2e photo listée en 7e position) 

```
<!--

1-3-5-13-https://www.inaturalist.org/observations/195220528
1-4-https://www.inaturalist.org/observations/195220524
5-https://www.inaturalist.org/observations/195226187
4-https://www.inaturalist.org/observations/195708914

-->

```

À noter que cette section est circonscrite par les caractères `<!--` et `-->` pour éviter l'intégration des adresses dans le site. Ces caractères doivent être présents en tout temps dans le fichier `.md`.

### Section description

La seconde partie du fichier `.md` contient le compte-rendu de l'espèce qui apparaîtra sur le site internet. Les titres sont précédés par `##` pour la formatin du titre. Bien que les titres puissent être modifiés, il est impératif de conserver ces titres pour assurer l'uniformité du site. S'il n'y a aucune information pour une section, il est préférable de laisser un tiret `-` suite au titre. 

#### Traits distinctifs

Ici, on trouve une liste à points des traits distinctifs de l'espèce ou des éléments clés pour repérer et reconnaître l'espèce sur le terrain. En d'autres mots, que remarque-t-on de particulier chez cette espèce par rapport aux autres semblables? Pour cette partie, on sépare les éléments de la liste à points par des tirets `-`. Voir notamment en exemple le compte-rendu pour [_Cinna arundinacea_](https://github.com/frousseu/floreduquebecsp/blob/main/Esp%C3%A8ces/Poaceae/Cinna/Cinna_arundinacea.md?plain=1). 

#### Espèces semblables

Ici, on énumère les critères à regarder pour différencier cette espèce des autres espèces semblables. L'idéal est de cibler les espèces qui sont les plus semblables et de ne pas se perdre dans la description des autres espèces qui sont clairement différentes si on regarde attentivement les photos.

#### Habitat

Ici, on trouve une description sommaire de l'habitat et possiblement de la répartition de l'espèce. On peut se baser sur l'expérience personnelle.

#### Commentaires

Finalement, est-ce qu'il y a des remarques à faire pour l'espèce notamment en lien avec la distribution, la taxonomie, le statut ou en lien avec d'autres éléments intéressants concernant l'espèce? On peut aussi discuter des sous-espèces ou des variétés ou de certaines particularités de l'espèce.

## Formattage

Voici les principaux éléments de formattage `markdown` que vous pourriez vouloir utiliser lors de l'écriture des comptes-rendus. Les noms de taxon devraient être en italique.

| Code | Texte |
|----------|----------|
| `Ce texte est en _italique_` | Ce texte est en _italique_ |
| `Ce texte est en **gras**` | Ce texte est en **gras** |
| `L'adresse du site est [florequebec.ca](https://florequebec.ca)` | L'adresse du site est [florequebec.ca](https://florequebec.ca) |


## Comment contribuer ?

Pour contribuer, il faudra d'abord vous créer un compte [GitHub](https://github.com/). GitHub est une plateforme destinée à héberger du code et à la collaboration. Par l'utilisation de [Git](https://fr.wikipedia.org/wiki/Git), elle permet surtout d'assurer un suivi des modifications de fichiers et de quantifier les modifications sur ces fichiers. 

Votre première contribution aux comptes-rendus risque de vous paraître un peu difficile en raison de la complexité de cette plateforme. En effet, Git et GitHub sont des outils puissants, mais complexe et peuvent être difficile à apprivoiser au premier abord. Cependant, après une première exposition, le processus décrit plus bas devrait devenir un peu plus facile. Si vous voulez de l'aide lors de cette première contribution ou si vous avez des questions ou des difficultées, n'hésitez pas à contacter un membre de l'équipe de révision et il nous fera plaisir de vous assistez lors de la création de vos comptes-rendus.

À noter que l'intégration des modifications au site ne sont pas automatiques. Elles doivent d'abord être approuvées par un membre de l'équipe de révision. Pour l'intégration des photos sélectionnées, un script doit également être utilisé pour récupérer les photos et effectuer la mise à jour.

### 1. Création du compte GitHub

Lors de la création de votre compte, il est préférable d'utiliser votre nom complet (avec accents) afin de faciliter le lien avec votre bio comme contributeur (voir [ici](https://github.com/flore-quebec/species/tree/main/Contributeurs)). Votre nom d'utilisateur peut être celui que vous voulez, mais idéalement vous devriez spécifier votre nom complet comme identifiant. Par exemple, un nom d'utilisateur peut être _frousseu_, mais un nom complet serait _François Rousseu_. Il n'est pas nécessaire de créer le fichier .md contenant votre bio. Un membre de l'équipe de révision peut s'en charger.  

### 2. Trouvez le fichier de votre espèce

La façon la plus simple pour éditer le contenu pour une espèce est d'utiliser la plateforme en ligne. En premier, il faut naviguer vers le fichier .md de votre espèce. Les espèces sont classifiées dans des dossiers par famille et par genre. Lorsque vous êtes sur le fichier de l'espèce, vous pouvez utiliser le bouton en haut à droite *Edit this file* (le petit icône de crayon).

 <br><br>
![](https://cdn.hebergix.com/fr/floreqc/FQ_edit_file.png)
 <br><br>
 
### 3. Créez une image sur votre compte ( _fork_ )
 
La plateforme vous proposera de créer une _fork_ sur votre propre compte. Cette _fork_ est en quelque sort une image des différents dossiers et fichiers qu'il y a sur le site GitHub de Flore Québec. Cette image vous permettra de travailler les comptes-rendus directement sur votre compte sans que ces modifications affectent le site principal. Lors de la création de cette image (_fork_), conservez les sélections par défaut et choisissez s'il y a lieu l'option *Commit directly to the main branch*.

 <br><br>
![](https://cdn.hebergix.com/fr/floreqc/FQ_commit_changes.png)
 <br><br>

### 4. Éditez le fichier .md 

### 5. Enregistrez les changements (_Commit changes_)

Par la suite, il faudra cliquer sur le bouton vert *Commit changes* (en haut à droite) pour proposer les changements. Une branche (*fork*) sera alors créée sur votre compte GitHub à partir de laquelle vous pourrez éditer les comptes-rendus. Encore une fois, choisissez l'option *Commit to the main branch* s'il y a lieu.

<br><br>
![](https://cdn.hebergix.com/fr/floreqc/FQ_commit_main.png)
<br><br>

### 6. Soumettez vos modifications

Une fois que vous êtes satisfait de votre compte-rendu, vous pouvez soumettre votre compte-rendu à l'aide du bouton *Contribute*. Vous aurez accès à ce bouton en allant sur la page principale de votre _fork_.
 <br><br>
![](https://cdn.hebergix.com/fr/floreqc/FQ_contribute.png)
 <br><br>

### 7. Créez une demande de modifications

Ce bouton vous permettra de soumettre vos modifications par l'intermédiaire d'une _pull request_ (*Create pull request*) pour proposer d'intégrer les changements aux site. Ce processus peut paraître un peu complexe la première fois, mais après quelques fois, cela devrait vous paraître beaucoup plus facile. À noter que les changements que vous proposerez devront être approuvés par un membre de l'équipe de révision. Ceci permettra notamment de s'assurer de l'unformité du contenu et de repérer d'éventuelles erreurs de syntaxe *markdown* ou d'orthographe.

 <br><br>
![](https://cdn.hebergix.com/fr/floreqc/FQ_create_pull_request.png)
 <br><br>
 
### 8. Synchronisez votre _fork_

Lors de vos prochaines modifications ou écritures de comptes-rendus, il est préférable de synchronizer le contenu de votre _fork_ avec celui du site principal. Pour ce faire, vous devez utiliser le bouton *Sync fork* sur la page principale de votre _fork_. Ceci vous permettra d'intégrer les modifications récentes sur votre _fork_. Cette étape n'est pas essentielle, mais elle peut-être très utile si par exemple une autre personne aurait déjà écrit le compte-rendu pour l'espèce que vous souhaitez modifier.

<br><br>
![](https://cdn.hebergix.com/fr/floreqc/FQ_sync_fork.png)
 <br><br>

Pour vos comptes-rendus suivants, vous pouvez directement écrire les comptes-rendus sur votre _fork_. L'idéal est de les soumettre au site principal au fur et à mesure pour faciliter la révision par l'équipe.

Si vous êtes un contributeur régulier, vous pourriez également obtenir les droits pour proposer ou intégrer directement vos modifications sur le site sans passer par le processus de *fork* (création d'une branche sur votre compte) ou de *pull request*. Pour toutes questions, n'hésitez pas à contacter un membre de l'équipe de révision et notamment François Rousseu.  


 





