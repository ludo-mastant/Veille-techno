# Veille Technologique - Problèmes avec les Extensions Microsoft C/C++ sur Cursor

## Contexte
Cursor est un éditeur de code basé sur le même fondement open source que Visual Studio Code (VS Code). Cependant, des problèmes ont émergé concernant l'utilisation des extensions populaires de Microsoft, notamment pour C et C++.

### Problème Signalé
Des utilisateurs ont signalé que l'extension **C/C++** de Microsoft ne fonctionnait plus comme prévu. Alors que la version 1.17.62 était opérationnelle, les versions ultérieures (1.18.21 et au-delà) rencontrent des dysfonctionnements. Par exemple, la fonctionnalité "Find all references" ne fonctionne pas après l'installation de ces versions récentes dans l'éditeur Cursor.

## Restrictions de l'Extension Marketplace de Microsoft
Microsoft impose des restrictions sur son **VS Code Extension Marketplace**, autorisant son utilisation uniquement avec certains produits et services, tels que Visual Studio, VS Code, GitHub Codespaces, Azure DevOps, et Azure DevOps Server. Cette restriction pousse les développeurs à privilégier les distributions officielles de Microsoft.

En réponse à cette politique, la fondation Eclipse a créé **Open VSX**, un marketplace alternatif pour les extensions open source, afin de permettre une plus grande liberté aux développeurs.

### Impact sur Cursor
Bien que Cursor offre la possibilité d'installer des extensions du **VS Code Marketplace**, y compris l'extension C/C++ de Microsoft, des restrictions sur certaines fonctionnalités apparaissent, comme la notification d'un message indiquant que l'extension ne peut être utilisée correctement. Les utilisateurs peuvent aussi installer l'extension à partir d'un fichier `.vsix`, mais cette méthode semble désormais compliquée, notamment en raison de la suppression des liens directs vers les fichiers d'extension.

## Solutions Alternatives
Les utilisateurs de Cursor peuvent envisager l'extension **clangd**, qui, bien qu'elle ait moins d'installations (1,7 millions contre 81 millions pour l'extension Microsoft), reste une alternative viable pour le développement en C/C++.

## Spéculations sur les Causes du Changement
Certains développeurs supposent que ces changements ont été motivés par l'arrivée d'une nouvelle fonctionnalité IA, **Agent Mode**, dans la version stable de VS Code, ce qui fait de Cursor un concurrent direct pour Microsoft.

## Conclusion
Bien que Cursor reste compatible avec certaines extensions de Microsoft, des problèmes de fonctionnement persistent, surtout avec les extensions liées aux langages C et C++. La politique plus stricte de Microsoft concernant l'utilisation de ses extensions dans des IDE tiers semble être une cause majeure de ces dysfonctionnements.
