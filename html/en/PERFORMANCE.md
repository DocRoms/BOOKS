
# Un HTML performant.
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

Ces deux exemples présentent une page identique!

Vous pouvez remarquez que **l'exemple 2** comporte beaucoup plus de balise que **l'exemple 1**.

Il ne fait pas perdre de vue qu'une page doit comporter le moins de balises possible!
 
Plus vous avez de balises HTML, plus votre page sera lourde et lente à charger. 
N'ajoutez des balises, des attributs que si vous êtes sur de les utiliser!