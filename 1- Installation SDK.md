# 1. Installer le SDK

Je vous propose d'installer le SDk a partir d'Intellij.

Pour ce faire :

1. Installer le plugin flutter. Redemarre IntelliJ
2. Demarrer un nouveau projet flutter. Intellij va alors installer le SDK flutter, et le SDK Android si besoin.

# 2. Connecter un telephone

Pour les telephones Android:

1. Activer les `developer options`
2. Activer `USB Debugging`

Le telephone devrait apparaitre en haut de Intellij, dans la liste des `device` possibles.

## Erreurs possibles

### Les licences du SDK android ne sont pas acceptees.
 
Pour les accepter, aller dans le repertoire tools/bin de votre installation du SDK Android. Lancer la commande `./sdkmanager --licenses` et repondez oui tout le temps.
 
### java.lang.NoClassDefFoundError: javax/xml/bind/annotation/XmlSchema

Le SDK Android a besoin de certaines classes anciennement packagee avec le SDK, mais qui ne le sont plus depuis le SDK 11 de java.
Utilisez une version 10 du SDK est la maniere la plus simple de resoudre le probleme.

Alternativement, vous pouvez essayer de rajouter cette variable d'environnement (ici pour windows): `set JAVA_OPTS=-XX:+IgnoreUnrecognizedVMOptions --add-modules java.se.ee`



