# docker-networking
docker networking like dns , multiple images etc


1. Run postgress docker compose , so db is up and running :
`docker-compose -f postgress.yaml up`

2. Run migration docker compose ,so db migration and kick in (also pass this so that it holds on for any inspection):
`docker-compose -f migration.yaml run  --entrypoint="tail -f /dev/null" db_migrate`
   
