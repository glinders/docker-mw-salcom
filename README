# Mediawiki as a Docker service

Mediawiki runs as a service, using a data container.

Data can be backed up and restored using the backup and restore containers

## usage

    make build; make run

## backup

All data resides in directory /varwww
Data is backed up to directory /backup (tar.gz file).
To back up, use command:

    docker start mw-salcom-app-backup

Use `docker cp mw-salcom-app:/backup <dest>` to get backups out of container.


## restore

Archive to restore must be one created above (format: 20180724.mw-salcom.tar.gz).
Use `docker cp <archive> mw-salcom-app:/restore` to get archive into container.
To restore, use command:

    docker start mw-salcom-app-restore
