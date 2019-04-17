# drupal8-travis-phpunit-behat
Drupal 8 with beta, travis and PHPunit tests for dev and production

### Note: The quickest way to import a production database locally with this setup is to do the following:

- Drop a .sql dump file into the project root (e.g. sql-dump.sql).
- Import the database: 

<code> docker exec ddkits_docker bash -c "mysql drupal < /var/www/drupalvm/drupal/sql-dump.sql" </code>

- Clear caches: 

<code> docker exec ddkits_docker bash -c "drush --root=/var/www/drupalvm/drupal/web cr </code>
