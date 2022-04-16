# gallery-photo
Installer les dépendances du compositeur

composer install
Générer une clé locale pour laravel (stockée dans .env)

php artisan key:generate
lier le dossier de stockage

php artisan storage:link
Migrer la base de données (à partir de zéro) vers la dernière version

php artisan migrate
Amorcer la base de données avec les données essentielles (comme les autorisations et les rôles de base)

php artisan db:seed
Pour voir la liste des commandes artisanales disponibles

php artisan list
Comme vous utiliserez beaucoup artisan (et nous en tant que programmeurs sommes paresseux), créez un alias dans votre .bash_profile

alias art='php artisan'
Nous devons également installer npm avec ses paquets

npm install
Et exécutez npm pour le laisser générer un site Web agréable et propre pour vous

npm run dev
Exécution des tests
Exécuter tous les tests

composer test
L’exemple ci-dessus exécute phpunit, phpcs, phpmd et larastan. Infos trouvées dans le reste de ce paragraphe.

phpunit - tous les tests définis
Cette commande exécutera tous les tests unitaires php trouvés dans le dossier de test. cela inclut les tests d’unité ainsi que les tests de fonctionnalité.

./vendor/bin/phpunit
Analyseurs de code statique et tests de style de codage
Pour exécuter tous les analyseurs à la fois :

composer lint
