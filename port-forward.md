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
root@cp1:/home/rattle# kubectl port-forward pod/back-cfbb5c4cf-pfpkb 8000:80
Forwarding from 127.0.0.1:8000 -> 80
Forwarding from [::1]:8000 -> 80
Handling connection for 8000
E0218 10:50:52.664267  274047 portforward.go:406] an error occurred forwarding 8000 -> 80: error forwarding port 80 to pod 3c2d5838a2cb331a3ae4c1b340a9327b969df01f55f20580c266ca572444b609, uid : failed to execute portforward in network namespace "/var/run/netns/cni-eae423b1-8cc2-b801-6c53-dd4813c431a7": failed to connect to localhost:80 inside namespace "3c2d5838a2cb331a3ae4c1b340a9327b969df01f55f20580c266ca572444b609", IPv4: dial tcp4 127.0.0.1:80: connect: connection refused IPv6 dial tcp6: address localhost: no suitable address found
E0218 10:50:52.664629  274047 portforward.go:234] lost connection to pod


root@cp1:/home/rattle# curl 127.0.0.1:8000
curl: (52) Empty reply from server


