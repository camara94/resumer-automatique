# Résumé Automatique
En général, les algorithmes de récapitulation sont soit extractifs, soit abstractifs en fonction du résumé généré. Les algorithmes d'extraction forment des résumés en identifiant et en collant ensemble les sections pertinentes du texte d'entrée. Ainsi, ils ne dépendent que de l'extraction des phrases du texte original. Pour une telle raison, les méthodes d'extraction produisent naturellement des résumés grammaticaux et nécessitent relativement peu d'analyse linguistique.

En revanche, les algorithmes abstractifs sont les plus humains et imitent le processus de paraphrase d'un texte, ce qui peut générer un nouveau texte qui n'est pas présent dans le document initial. Les textes résumés à l'aide de cette technique ressemblent davantage à des humains et produisent des résumés condensés. Cependant, les techniques abstractives sont beaucoup plus difficiles à mettre en œuvre que les techniques de synthèse extractive. Il convient de mentionner que les résumés abstractifs existants reposent souvent sur un composant de prétraitement extractif pour produire le résumé du texte.

## Projet
Dans cet article, nous allons partir sur le site de la radio **Mosaïque FM**. Lorsqu'un utilisateur saisi une URL on fait le résumé de l'article en question en utilisant l'approche extractive.
Nous allons decomposer le travail en deux partie:
* une première partie consistera à faire du web scraping avec les packages <code>**request**</code> et <code>**BeautifulSoup**</code>
* la partie II, nous allons utiliser le <code>**sklearn**</code>, le Framework <code>**spacy**</code> pour faire notre résumé automatique
  
## Partie I: Web Scraping en python
Avant de commencer, il faut installer **requests** et **bs4**:
* pip install requests --user
* pip install bs4 --user
