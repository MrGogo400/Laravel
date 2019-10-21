# Tome 1 : Comment je me suis suicider 

---

- [First Section](#section-1)

<a name="section-1"></a>
# # **Installation de l'environnement de développement et création du premier projet.**

### Le jour où j'ai installé Composer

Windows (ta essayer de changer d'OS ?) : 

https://getcomposer.org/Composer-Setup.exe


Linux / OSX : 

```bash
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === 'a5c698ffe4b8e849a443b120cd5ba38043260d5c4023dbf93e1558871f1f07f58274fc6f4c93bcfd858c6bd0775cd8d1') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');" 
```


### Le jour où j'ai installé Laravel

Dans un terminal : 

```php
composer global require laravel/installer
```

Puis : 

```php
laravel new blog
```

### Le jour où j'ai run laravel

Toujours dans un terminal :

```php
php artisan serve
```

### Le jour où j'ai connecter la base données (CF : Moodle)

Dans le .env : 

```php
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=mabasedonnées
DB_USERNAME=monusernamedemabasedonnées
DB_PASSWORD=monmdpdemabasedonnées
```

### Le jour où j'ai eu un premier rendu visuel

Sur la page d'accueil : 

----

![Tavuçaclaque?](https://i.imgur.com/dWXnMmm.png)

###### ta vue ça claque ?

### Le jour où j'ai créer les premières pages

Donc la dans ton web.php tu mets ça : 

```php
    Route::get('/test', ['middleware' => 'role:test', function () {
        return view('test');
```
###### Enfin un truc qui y ressemble car honnêtement j'ai fait ça ya longtemps donc j'ai oublié

----

Et après tu es censée avoir autre chose que ça mais vue que j'ai trop avancée dans le tuto pro gamers j'ai autre chose tmtc :

----

![çaclaqueencoreplus](https://i.imgur.com/7OFvcST.png)


### Après y'a des baux avec des "constrollers" mais j'ai oublié donc on passe aux "views"

---

La tu a une "view" qui a spawn normallement a par si il faut faire un truc dans les "controllers" mais bon comme on dit YOLO #BringBackYolo

---

Donc dans ta "view" tu mettre t'on code HTML

```php
<html>
    <body>
        <h1>Hello, name</h1>
    </body>
</html>
```

---

###### Donc là c'est tellement bien codé que quand tu mets une variable en balise code sur larecipe, ça la prend en compte comme du vrai code donc je peux pas la mettre, mais c'est censé ressembler à ça :

---

![laravelsansfaille](https://i.imgur.com/IDFoSDx.png)

### 