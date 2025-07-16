**L**oki, **A**lloy, and **G**rafana containers for ingesting and analyzing logs locally.

This project is intended for debugging and troubleshooting static logs.

Since those logs might be old, Alloy is configured to use the timestamp in the logs, as opposed to the default which is the ingest time/date.

Expected log format: `Jul 01 06:25:05 vaultdev02 vault[1337]: 2025-05-20T06:25:05.217-0700 [INFO]  expiration: revoked lease: lease_id=auth/kubernetes/login/h0392354158c45a0ec704c77176afb411b492affb852bede025ae86949ab17fb8`

 - Place your systemd formatted logs in the `logs/` folder.
 - Run `docker-compose up -d` to start the containers
 - Run `docker-compose down` to stop them.
