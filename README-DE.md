<div align="center">  
  <a href="README-TR.md"   >   TR <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/TR.png" alt="TR" height="20" /></a>  
  <a href="README-EN.md"> | EN <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/US.png" alt="EN" height="20" /></a>  
  <a href="README-DE.md"> | DE <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/DE.png" alt="DE" height="20" /></a>  
  <a href="README.md"> | NL <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/NL.png" alt="NL" height="20" /></a>  
</div>

# DomainNameApi Integrationsdokumentation (DE)

## 📦 Download — verwenden Sie immer die Releases!

⬇️ **Die neueste getestete Version erhalten Sie hier: https://github.com/domainreseller/hostfact-dna/releases/latest**

> ⚠️ Verwenden Sie **nicht** den grünen Button **Code → Download ZIP** — damit laden Sie den unbearbeiteten Entwicklungsbranch herunter. Release-Pakete sind versioniert, getestet und produktionsreif.

## Installation

1.  Legen Sie den Ordner `domainnameapi` im Verzeichnis `Pro/3rdparty/domain/` ab oder laden Sie ihn per FTP hoch.

## Konfiguration im Control Panel

1.  Navigieren Sie zu `Control -> Services -> Registrare`.

    ![img1.png](img1.png)

2.  Klicken Sie auf die Schaltfläche **"Registrar hinzufügen"**.

    ![img2.png](img2.png)

3.  Wählen Sie **"DomainNameApi"** als API aus.


4.  Geben Sie Ihren Benutzernamen und Ihr Passwort ein.

    ![img3.png](img3.png)

5.  Klicken Sie auf **"Speichern"**.

## 🔑 API-Zugangsdaten — Benutzername/Passwort oder Reseller ID/API Key?

Beides wird unterstützt — tragen Sie die Daten in dieselben zwei Modulfelder ein; das Modul erkennt automatisch, welche API verwendet wird:

| Sie haben | Feld "Benutzername" | Feld "Passwort" | Verwendete API |
|---|---|---|---|
| **Neue Panel-Zugangsdaten** (empfohlen) | Reseller ID — UUID wie `xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` | API Key | REST |
| **Legacy-Zugangsdaten** | API-Benutzername | API-Passwort | SOAP |

> 💡 Ihre **Reseller ID** und Ihren **API Key** finden Sie in Ihrem DomainNameAPI-Panel unter **API Settings**.
> ⚠️ Dies sind **API-Zugangsdaten** — die E-Mail-Adresse und das Passwort Ihres Panel-Logins funktionieren hier **nicht**.

Es ist keine zusätzliche Konfiguration erforderlich — enthält das Benutzernamenfeld eine UUID, verwendet das Modul die moderne REST API, andernfalls das klassische SOAP.

## Domains importieren

1.  Nach dem Speichern der Registrar-Einstellungen werden Sie zum Bildschirm für den Domain-Import weitergeleitet.
2.  Hier können Sie die gewünschten Domains auswählen und importieren.

    ![img4.png](img4.png)
    ![img5.png](img5.png)

## Verwendung

1.  Nach der Konfiguration und dem Import können Sie Produkte erstellen sowie Domains über die DomainNameApi-Integration registrieren und verwalten.

    ![img6.png](img6.png) 