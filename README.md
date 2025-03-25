**1 Cloner le repository** :
```sh
git clone https://github.com/evaluationWeb/jefffapi.git
```

**2 Se déplacer dans le dossier** :
```sh
cd jefffapi
```

**3 configurer le fichier .env** :
```env
# ajouter la clé suivante
DATABASE_URL="mysql://root:@127.0.0.1:3306/jeffapi?serverVersion=10.4.32-MariaDB&charset=utf8mb4"
# si vous avez une base de données Mysql MariaDB à modifier en fonction de vos informations de connexion
```

**4 Installer les dépendances** :
```sh
composer install
```

**5 Créer la BDD** :
```sh
php bin/console d:d:c
```

**6 Migrer la stucture** :
```sh
php bin/console d:m:m
```

**7 Démarrer le serveur** :
```sh
symfony serve -d
```

**8 Ouvrir l'url swagger UI** :
http://127.0.0.1:8000/api 
ou https://localhost:8000/api



