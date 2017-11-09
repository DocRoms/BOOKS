# HTML Basics

## One Tag story
HTML is a est un language interpretté par un navigateur internet (Edge, Firefox, Opéra Chrome)
reçoivent des pages en HTML, et affichent la page designé à partir du code reçu.

Pour plus d'information, vous pouvez vous rendre sur le chapitre [Comprendre le fonctionnement d'un site Web]().

Le code HTML fonctionne sous forme de balises. Il en existe plusieurs types :
 
Une balise ouvrante et fermante : 
```html 
<html></html>
```

Une balise auto-fermante: 
```html
<br />
```

Ces différentes balises peuvent posséder un ou plusieurs attributs, ceux-ci peuvent être obligatoire ou facultatif, suivant la balise:

Une balise (img) avec ses attributs obligatoire (src et alt)  : 
```html
<img src="monLogo.jpg" alt="Mon Logo" />
```

Une balise (img) avec ses attributs obligatoire (src et alt), et un attribut facultatif (style):
```html
<img src="monLogo.jpg" alt="Mon logo" style="with:100%:height:auto" />
```

Voici un exemple complet de page HTML simplifiée: (en HTML5)
```html
<!DOCTYPE html>
<html lang="fr">
    <head>
        <title>Mon titre</title>
    </head>
    <body>
        <nav>Mon menu</nav>
        <section>
            <!-- Liste de mes articles -->
            <article>
                Mon premier article
            </article>
        </section>
    </body>
</html>
```

Dans cet exemple, deux lignes vous sont encore inconnues: 
```html
<!DOCTYPE html>
```
Il s'agit de la première information qui doit apparaitre sur votre page HTML, c'est cette balise spéciale (le doctype) qui présente au
navigateur internet, la version de HTML utilisée.

```html
<!-- Liste de mes articles -->
```
Cette ligne présente un commentaire, vous pouvez l'utilisez dans votre code sans aucunes incidence sur le design de votre page, 
Il suffit de laisser un commentaire entre les balises `<!--` et `-->`.



## Une histoire d'imbrication...
Les balises HTML s'imbriquent par niveau.
Une structure iddentique existe pour chaque page HTML, il faut obligatoirement le respecter :
```html
<html>
    <head></head>
    <body></body>
</html>
```
Cette structure est composée de trois balises dites 'structurelles', que sont `<html></html>`, `<head></head>` et `<body></body>` 

### La balise `<html>`
Cette balise ne doit contenir que les balises `<head>` et `<body>`.

### La balise `<head>`
Les balises contenues entre les balises `<head>` et `</head>` sont généralement des balises de présentation, et de description du corps du document.
Entre ces deux balises peuvent figurer: 

La balise `<title></title>` qui contient le titre du site internet : 
```html
<title>Mon site internet</title>
``` 

Les balises `<meta />` qui décrivent le site internet:
```html
<meta charset="UTF-8" />
<meta name="robots" content="index,follow,all" />
<meta name="identifier-URL" content="https://monSiteInternet.fr" />
<meta name="ContentOwner" content="Henry Goland" />
<meta name="Description" content="La description de mon site" />
<meta name="Keywords" content="Code, Lyon, Dev" />
<meta /> ...
```

Les balises `<link href="" rel="" type="" />` qui permettent de charger différentes ressources:
```html
<link rel="shortcut icon" type="image/x-icon"  href="monIcone.ico"/>
<link rel="stylesheet" type="text/css" href="monPremierFichier.css" />
<link rel="stylesheet" type="text/css" href="monsecondFichier.css" />
```

Les balises `<script></sript>` qui contiennent différents scripts (généralement du javascript): 
Ces balises peuvent être utilisées pour charger un fichier: 
```html
<script type="text/javascript" src="monScript.js" />
```
Ou contenir directement du code: 
```html
<script type="text/javascript">
    function logMyName(name){
        console.log(name);
    }
    
    logMyName('Heisenberg');
</script>
```

### La balise `<body>`
La balise `<body>` correspond au corps du site internet. Ici, mis à part les commentaires (ex : `<!-- Mon super commentaire-->`), tout 
ce que vous changerez aurra une incidence directe sur la page visible par vos utilisateurs.

Il existe des centaines de balises utilisables, que vous pouvez comprendre dans le chapitre []()

```html
<body>
    <header><!-- Entête --></header>
    <nav><!-- Navigation --></nav>        
    <aside><!-- Bloc secondaire à coté du contenu principam --></aside>
    <main><!-- Bloc principal-->
        <section><!-- Première section du site -->
            <h1><!-- Titre de la première section --></h1>
            <article><!-- Contenu de la première section --></article>
        </section>
        <section><!-- Seconde section du site -->
            <h1><!-- Titre de la seconde section --></h1>
            <article><!-- Contenu de la seconde section --></article>
        </section>
    </main>
    <article><!-- Contenu textuel de la page --></article>
    <footer><!-- Pied-de-page de la page -> site --></footer>
</body>
```