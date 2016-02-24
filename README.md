# IFI_MvcBourse

Une application web sous MVC par VisualStudio.

## Installation de l'infrastructure

Installation de windows 8.1 SP1 puis visualstudio community 2015 et sqlserver 2016 express pour localDb.

Cependant sqlserver 2016 nécessite l'utilisation de .NET Framework 3.5 sp1, son installation revoit un code d'erreur 0x800F0906.
Une solution est proposée à ce lien :
[solution](http://stackoverflow.com/questions/25188234/windows-8-1-unable-to-install-net-framework-3-5-0800f0906)

Cette solution demande de taper une commande powershell sous le compte administrateur :
  Enable-WindowsOptionalFeature -Online -FeatureName 'NetFx3' -Source 'd:\sources\sxs'
pour activer le framework manquant.

## L'application d'inventaire

L'application utilise un CRUD avec une table pour inventorier des équipements réseau, pour simuler
un petit espace web pour une consultation sous condition d'être authentifié.
