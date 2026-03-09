# netdata
устранение ошибок
1. postgresql - добавить пользователя 
   1. docker exec -it prod-wine_host-1 psql -U wine -d postgres -c "CREATE USER netdata WITH PASSWORD 'postgres';"
   2. docker exec -it prod-wine_host-1 psql -U wine -d postgres -c "GRANT pg_monitor TO netdata;"