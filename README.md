# migrate_csv_d8_custom
CSV to Drupal 8 Migration with Entity Reference!

### Site building:-

1) Create a new Content Type called Actors (machine name - actors). You can keep the fields/settings to default. We don't need to add additional fields for this sample migration.
2) Create a new Content Type called Movies (machine name - movies). Add a new field Actors (field_actors) which  would be Entity Reference to Actors Content Type.
3) Place the actors.csv and movies.csv files to root of your local Drupal 8 site.
4) Enable the module "migrate_csv_d8_custom".

### Migration:-

```sh
drush ms
drush mi actors
drush mi movies
```
