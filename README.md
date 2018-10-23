# tde-wordpress
Holds the docker-compose file for TDE's wordpress container. This will bring up both the database and the wordpress container, and connect them together so they can talk.

## Usage 
From this directory:

```bash
docker-compose up -d
```

## Backup
The docker-compose file creates a data folder (`./data`) in the same directory, where the database will write its data contents to `./data/db` and wordpress will write its contents to `./data/tde-wp/wp-content`. The entire `./data` folder should be backed up.

## Restore 
If you have a backup of the `./data` folder, simply place it in the same folder as `docker-compose.yml` and then run bring up the containers with the docker-compose command above.
