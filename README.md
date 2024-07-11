# gsp314-arcade-2024
tutorial to finish the gsp 314 challange lab

TASK 1 only

FIX BUG QUERY SQL :

open setup.txt dan change username/[MIGRATION ADMINE] as lab instruction.
open VM Instance > SSH
run the command :
- sudo apt install postgresql-13-pglogical
- sudo su - postgres -c "gsutil cp gs://cloud-training/gsp918/pg_hba_append.conf ."
sudo su - postgres -c "gsutil cp gs://cloud-training/gsp918/postgresql_append.conf ."
sudo su - postgres -c "cat pg_hba_append.conf >> /etc/postgresql/13/main/pg_hba.conf"
sudo su - postgres -c "cat postgresql_append.conf >> /etc/postgresql/13/main/postgresql.conf"
sudo systemctl restart postgresql@13-main
- sudo su - postgres
- nano setup.sql copy the file that already change the username
- Ctrl+X and save
- psql -f setup.sql

follow the lab instruction again for another task
