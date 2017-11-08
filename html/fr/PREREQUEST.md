#Les bases du HTML

##Une histoire de balise
Le HTML est un language interpretté par un navigateur internet (Edge, Firefox, Opéra Chrome)
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

## Une histoire d'imbrication...



## Un HTML performant.
Voici deux codes HTML qui ont exacyement le même rendu: 

Exemple 1: 
```html
<!DOCTYPE html>
<html lang="fr">
    <head>
        <title>Mon titre</title>
    </head>
    <body>
        <nav>Mon menu</nav>
        <section>
            <article>
                Mon premier article
            </article>
        </section>
    </body>
</html>
```

Exemple 2: 
```html
<!DOCTYPE html>
<html lang="fr">
    <head>
        <title>Mon titre</title>
        <style></style>
    </head>
    <body>
        <div id="content">
            <nav>
                <span>Mon menu</span>
            </nav>
            <section>
                <div id="articles">
                <article>
                    <p>
                    Mon premier article
                    </p>
                </article>
                <article>
                    
                </article>
                </div>
            </section>
        </div>
    </body>
</html>
```