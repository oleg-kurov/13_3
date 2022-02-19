**front**
root@cp1:/home/rattle# kubectl port-forward pod/front-784597b7cd-gjwh2 8080:80
Forwarding from 127.0.0.1:8080 -> 80
Forwarding from [::1]:8080 -> 80
Handling connection for 8080


root@cp1:/home/rattle# curl 127.0.0.1:8080
<!DOCTYPE html>
<html lang="ru">
<head>
    <title>Список</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="/build/main.css" rel="stylesheet">
</head>
<body>
    <main class="b-page">
        <h1 class="b-page__title">Список</h1>
        <div class="b-page__content b-items js-list"></div>
    </main>
    <script src="/build/main.js"></script>
</body>


**for back**
root@cp1:/home/rattle# kubectl port-forward pod/back-cfbb5c4cf-pfpkb 9000:9000
Forwarding from 127.0.0.1:9000 -> 9000
Forwarding from [::1]:9000 -> 9000
Handling connection for 9000


root@cp1:/home/rattle# curl localhost:9000
{"detail":"Not Found"}

**for psql**
 kubectl port-forward pod/postgres-0 5432:5432
Forwarding from 127.0.0.1:5432 -> 5432
Forwarding from [::1]:5432 -> 5432
Handling connection for 5432


rattle@cp1:~$  psql --host localhost --port 5432 --dbname rattle --username rattle

Password for user rattle:
psql (12.3, server 11.5)
Type "help" for help.

rattle=>