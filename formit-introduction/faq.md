# Forum Aux Questions

## A propos de FormIt

**Qu’est-ce que FormIt et FormIt Pro ?**

FormIt est un environnement de modélisation, de visualisation, d’analyse et de calcul 3D pour la conception architecturale.

Fonctionnalités de FormIt :

* Moteur de modélisation de solides robuste, avec des outils et des workflows puissants optimisés pour la conception de bâtiments
* Visualisation améliorée de l’environnement pour illustrer les options de conception, y compris les états de modèle enregistrés à l’aide de scènes
* Emplacement, images satellite et terrain 3D à l’aide de Bing Maps
* Matériaux de la bibliothèque de matériaux d’Autodesk
* Outils d’organisation et de visibilité du modèle tels que des groupes, des calques et des scènes
* Outils d’analyse, notamment :
   * Validation de l’étanchéité et des faces arrière pour le diagnostic et la réparation des modèles solides
   * Soleil et Ombres
   * Analyse d’ensoleillement
   * Analyse d’énergie
* Intégrations de produits Autodesk :
   * BIM 360 Docs
   * Insight \(analyse d’énergie\)
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* Formats de fichier pris en charge :
   * Ouverture/Importation
      * AXM, DWG, FBX, SAT, STL, OBJ, WSM, SketchUp, Image
   * Exportation
      * AXM, FBX, OBJ, STL, SAT, DAE, DXF

FormIt est disponible gratuitement sur [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) et [dans votre navigateur](https://app.formit.autodesk.com/). Un abonnement à **FormIt Pro** est requis pour utiliser [FormIt pour Windows](https://formit.autodesk.com/page/download), la version la plus puissante et riche en fonctionnalités de FormIt. L’abonnement à **FormIt Pro** permet également d’accéder à des fonctionnalités supplémentaires sur iOS et le Web, telles que l’analyse d’énergie et d’ensoleillement. **FormIt Pro** est inclus dans [Autodesk AEC Collection](https://www.autodesk.fr/collections/architecture-engineering-construction/overview).

**Qu’est devenu FormIt pour Android ?**

Dans un souci constant de rationaliser l’offre de produits FormIt, nous avons dû prendre la décision difficile de mettre fin à l’application Android. Si vous l’avez installée, elle va continuer à s’exécuter, mais elle n’est plus disponible dans le Play Store.

**Comment obtenir Formit ?**

Pour exécuter la version Windows, vous devez avoir accès à **FormIt Pro**, qui fait partie de notre abonnement à [AEC Industry Collection](https://www.autodesk.fr/collections/architecture-engineering-construction/overview). Si votre bureau dispose de Revit, il y a de fortes chances que vous ayez déjà accès à FormIt. Vous pouvez [télécharger FormIt pour Windows directement à partir de notre site Web ](https://formit.autodesk.com/page/download) ou de l’application de bureau Autodesk.

En outre, la version Web peut être exécutée directement et gratuitement à partir de notre site Web : [http://formit.autodesk.com](http://formit.autodesk.com).

Vous pouvez télécharger gratuitement la version iOS à partir de l’App Store d’Apple \(iPad uniquement\).

**Si je suis étudiant ou enseignant, puis-je accéder à FormIt Pro gratuitement ?**

Oui. Vous pouvez accéder à l’abonnement FormIt Pro via le portail [Autodesk Education Portal](https://www.autodesk.fr/education/edu-software/overview?sorting=featured&page=1).

**Comment apprendre à utiliser FormIt ?**

Le meilleur endroit pour commencer est le [didacticiel FormIt Primer](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html).

Il existe plusieurs sections du guide, allant du niveau débutant \(création d’une maison moderne complète\) à un niveau plus avancé \(utilisation de Revit et de Dynamo de manière plus avancée\).

Notre série de webinaires FormIt Friday contient également plus de 20 vidéos. Ces webinaires sont disponibles sur notre [chaîne YouTube](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH).

## Utilisation de Revit

**Comment FormIt fonctionne-t-il avec Revit ?**

FormIt est une application de conception et d’esquisse 3D distincte, mais celle-ci crée des données qui peuvent être facilement converties au format Revit [à l’aide du complément FormIt pour Revit](https://formit.autodesk.com/page/formit-revit).

**Que se passe-t-il lorsque vous importez des données dans Revit ?**

À partir de la version 2016, Revit est fourni avec un complément permettant d’utiliser les données FormIt. Lorsque vous importez un fichier FormIt AXM dans Revit, ce complément examine chaque objet du fichier et le recrée dans Revit à l’aide de l’API. Par défaut, tous les éléments de FormIt sont classés dans la catégorie Volume.

Le convertisseur FormIt prend chaque objet de volume et crée une famille de volumes dans Revit à l’aide de l’[API Direct Shape](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/FRA/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html).

Direct Shape est un objet non modifiable utilisé dans les workflows IFC. Bien qu’il ne soit pas modifiable, il présente l’avantage de transférer des textures de matériaux complètes entre FormIt et Revit. [Voici un didacticiel ](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html) qui explique le workflow FormIt vers Revit plus en détail.

**FormIt permet-il de créer des murs, des sols et d’autres familles système Revit ?**

Pas directement. Comme indiqué ci-dessus, chaque objet est défini par défaut sur la catégorie Volume. Pour créer des murs, des sols, etc., vous devez importer le modèle dans Revit à l’aide du complément de conversion et utiliser les outils Revit natifs afin de créer des familles système à partir du modèle de volume sous-jacent.

**Revit peut-il renvoyer des données vers FormIt ?**

Oui. Pour réimporter des données dans FormIt, exportez tout ou, de préférence, une _partie_ de votre fichier Revit au format SAT. Il n’est généralement pas nécessaire d’envoyer TOUTES vos données Revit vers FormIt. Au lieu de cela, créez une vue filtrée dans Revit qui inclut uniquement les données minimales \(par exemple, les sols et les murs\) avant l’enregistrement au format SAT.

## Utilisation d’autres applications

**Pourquoi le format de fichier par défaut « .AXM » est-il utilisé ?**

Avant que FormIt ne soit officiellement nommé, le nom de code interne était XModeler. Par conséquent, le format de fichier que nous avons créé était Autodesk X Modeler, ou AXM.

**Quels types de formats 3D FormIt peut-il importer ?**

* Windows : AXM, DWG, FBX, OBJ, SAT, SKP, STL
* Web : OBJ, STL
* iOS : OBJ, STL, SAT

**Quels types de formats FormIt peut-il exporter ?**

* Windows : FBX, OBJ, SAT, STL, DAE, DXF
* Web : OBJ, SAT, STL
* iOS : OBJ

**Comment FormIt fonctionne-t-il avec Dynamo ?**

[Découvrez comment FormIt et Dynamo fonctionnent ensemble](https://formit.autodesk.com/page/formit-dynamo) pour créer des workflows de conception informatique.

**Quelle est la différence entre FormIt et SketchUp ?**

* Interopérabilité [**améliorée avec Revit**](../tool-library/revit.md) ****
* [**Intégration de Dynamo**](../tool-library/dynamo.md) pour la conception informatique
* Outils natifs d’[**analyse d’ensoleillement**](../tool-library/solar-analysis.md) et d’[**analyse d’énergie**](../tool-library/energy-analysis.md) optimisés par Autodesk Insight
* Noyau de modélisation de solides plus robuste qui permet des opérations de modélisation avancées
* Outils de modélisation avancés natifs tels que [**Balayage, Couverture, Lisser**](../tool-library/cover-sweep-loft.md), Décaler le solide/Solide de coque, et Congé/Raccordement 3D et [**Aplanir les faces**](../tool-library/flatten-face.md)
* Plusieurs [**plans de coupe** ](../tool-library/section-planes.md)visibles
* Outils de diagnostic comme [**Afficher les problèmes d’étanchéité et Afficher les faces arrière**](../tool-library/visual-styles.md)
* [**Exportation de parties du modèle**](../tool-library/export-data.md) en fonction des éléments sélectionnés et/ou visibles
* Exportation native des fichiers OBJ, SAT et STL

**Puis-je utiliser mes raccourcis clavier SketchUp ?**

Oui. FormIt pour Windows dispose d’un modèle de clavier entièrement modifiable. De nombreux raccourcis SketchUp courants sont déjà disponibles par défaut, mais vous pouvez les modifier dans le menu Modifier > Préférences.

**Est-il possible d’utiliser mes fichiers DWG ?**

Oui. FormIt permet d’importer des fichiers DWG 2D et3D.

## Questions d’assistance courantes

**Comment bénéficier d’une assistance ?**

Vous pouvez contacter votre revendeur Autodesk ou consulter le [forum FormIt](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=fr). De préférence, commencez par rechercher votre question. Si vous n’obtenez pas de réponse, publiez un nouveau sujet et l’équipe FormIt y répondra.

**Que faire si je ne peux pas me connecter ?**

* Cette [publication sur le forum](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=fr) traite des problèmes de connexion courants.
* Si vous disposez d’un PC équipé d’un processeur graphique commutable \(GPU\), il est important de s’assurer que FormIt utilise toujours le processeur graphique plus performant. Voici les instructions pour [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) et [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1).

**Que faire en cas d’échec de l’analyse d’énergie Insight ?**

Si l’analyse d’énergie Insight signale une erreur ou ne renvoie aucun résultat, [consultez la page Analyse d’énergie Insight](https://formit.autodesk.com/page/formit-insight) pour obtenir des conseils de dépannage courants.

