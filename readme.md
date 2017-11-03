# Présentation du systeme de template

## Le fichier template.xml
créer le fichier template.xml dans le repertoir __assets/xml__. 
ce fichier contient une section de balise pour chaque theme de votre application, ainsi que les posssitions ou serons chargées les vues de ce theme 

## La librairie Template.php
créer le fichier Template.php dans le repertoir libraries de votre application
cette librairie contient des méthodes pour : 
1. changer de theme de votre application
2. charger les vues d'un theme donné
3. charger le titre, les fichiers CSS, les fichiers JS d'un theme, etc

## Le theme  par defaut default.php
creer le repertoir themes dans le dossier appliction de votre application et y mettre votre fichier default.php 

## Le fichier de configuration folder_path.php 
Ce fichier contient les chemens d'acces aux nouveaux elements ajoutés dans notre application.
Ajouter le fichier folder_path dans le fichier de configuration _autoload.php_
$autoload['config'] = array('folder_path') ;

# Comment utiliser le système
Mettez votre nouveau theme dans le dossier __application/themes/nouveautheme.php__
Dans le fichier __nouveautheme.php__ definissez les positions des différentes vues qui serons charger dans le nouveau thème
Definissez les mêmes positions dans votre fichier __assets/xm/template.xml__ 
	<theme name="admin">
			<description>
				<![CDATA[
					This is the default template for our template system
				]]>
			</description>
			<position>output</position>
			<position>post_6</position>
		</theme>	

