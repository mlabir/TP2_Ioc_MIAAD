# TP2_Ioc_MIAAD
Mise en œuvre de l'injection des dépendances Partie2 #Sprin #Mavn

 l'injection des dépendances utilisant Spring framework. 
  puis on a commencer par la version XML et on a créé le fichier de configuration(applicationContex.XML).
  
  version capteur(XML):
  
  ![version capt version xml](https://user-images.githubusercontent.com/102171913/162547536-3d4166e4-bb5c-4276-9e43-6ed6c5af0435.PNG)

  on remplace la classe "dao.DaoImpl" par  "ext.DaoImpl" dans le fichier de configuration donne:
  
  ![version base meaven](https://user-images.githubusercontent.com/102171913/162547671-31f3bb20-8eea-4ba7-8877-541feb5055eb.PNG)

Passant à la version Annotation où on a utilisé la notion @Qualifier qui permet d'injecter les instances .

L'injection d'instance dao:

![version annotation](https://user-images.githubusercontent.com/102171913/162547950-7ee66b63-8ba2-455f-9052-cbb481cbe29e.PNG)

pour compiler l'application via le cmd on utilise la commande :--> mvn compiler:

![image](https://user-images.githubusercontent.com/102171913/162548363-8f1955e6-d8d6-476d-aeae-903bc1969fa5.png)

pour executer le test on utilise la commande :--> mvn  test

![image](https://user-images.githubusercontent.com/102171913/162548494-434e5549-98ab-4007-bbea-03c91b27e4a7.png)

pour  generer les packages : --> mvn package

et pour simplifier les chose et faire la compilation, le teste, et la generation les packages et l'envoyer vers  repository maven utilisant tout simplement la commande ---> mvn install

et on peut eviter l'utilisation de ces commandes dans le terminale car ils existent dejà dans l'IDE

![image](https://user-images.githubusercontent.com/102171913/162548752-f3ecd99f-ace0-4dc4-9f2d-a67908028997.png)
