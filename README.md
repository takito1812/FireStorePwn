<h1 align="center">
  <br>
  FireStorePwn (fsp)
</h1>

<h4 align="center">Firestore Database Vulnerability Scanner Using APKs</h4>

---

fsp scans an APK and checks if the Firestore database contains rules that are not safe, testing with and without authentication.

If there are problems with the security rules, attackers could steal, modify or delete data and raise the bill.

## How it works
<h3 align="center">
  <img src="https://i.imgur.com/IZTod0a.png" alt="fsp-flow" width="700px"></a>
</h3>

# Install fsp

```sh
sudo wget https://raw.githubusercontent.com/takito1812/FireStorePwn/main/fsp -O /bin/fsp
sudo chmod +x /bin/fsp
```

### Running fsp

#### Scanning an APK without authentication

```sh
fsp app.apk
```

#### Scanning an APK with authentication

With email and password.

```sh
fsp app.apk test@test.com:123456
```

With a token.

```sh
fsp app.apk eyJhbGciO...
```
