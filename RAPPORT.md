## 1. Statistiques descriptives

### Interprétation

**CPU** : l'utilisation moyenne (41,4 %) est légèrement supérieure à la médiane (39,2 %). L'asymétrie positive (0,58), la plus forte des quatre métriques, indique une traîne vers les valeurs élevées : quelques périodes de forte charge tirent la moyenne vers le haut. Le maximum de 100 % montre que le processeur atteint ponctuellement la saturation. Avec un CV de 50 %, c'est la métrique la plus irrégulière.

**Mémoire** : moyenne (7,20 Go) et médiane (7,14 Go) sont très proches, mais l'asymétrie reste positive (0,41) et la dispersion forte (CV de 45 %). La moitié centrale des mesures se situe entre 4,8 et 9,0 Go. Le maximum de 16 Go est une valeur ronde, qui correspond aux plateaux visibles sur les courbes : il suggère que la mémoire atteint sa capacité maximale lors des pics d'activité.

**Réseau** : la distribution est quasi symétrique (asymétrie de 0,08), mais très étalée (CV de 47 %, IQR de 85 Mbps). Le trafic varie fortement entre 25 et 200 Mbps. Comme pour la mémoire, le maximum rond de 200 Mbps et les plateaux observés suggèrent un plafond, probablement la limite de bande passante du lien.

**Température** : c'est la métrique la plus stable (CV de 16 %), avec une distribution symétrique (asymétrie de 0,07) et une moyenne proche de la médiane (41,4 °C contre 40,8 °C). Elle varie entre 27,8 et 57,9 °C. Cette stabilité s'explique par l'inertie thermique : un composant met du temps à chauffer et à refroidir, ce qui lisse les variations brutales de charge.

### Synthèse

Le CPU, la mémoire et le réseau sont des métriques très irrégulières, qui atteignent ponctuellement leur plafond (100 %, 16 Go, 200 Mbps) : le serveur connaît des épisodes de saturation. La température, plus stable, reste dans une plage raisonnable. Les distributions étant asymétriques pour le CPU et la mémoire, la **médiane** est un indicateur plus représentatif que la moyenne pour décrire leur niveau habituel.