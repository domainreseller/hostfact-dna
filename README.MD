<div align="center">  
  <a href="README-TR.md"   >   TR <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/TR.png" alt="TR" height="20" /></a>  
  <a href="README-EN.md"> | EN <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/US.png" alt="EN" height="20" /></a>  
  <a href="README-DE.md"> | DE <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/DE.png" alt="DE" height="20" /></a>  
  <a href="README.md"> | NL <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/NL.png" alt="NL" height="20" /></a>  
</div>

# DomainNameApi Integratie Documentatie (NL)

## 📦 Download — gebruik altijd de Releases!

⬇️ **Download hier de nieuwste geteste versie: https://github.com/domainreseller/hostfact-dna/releases/latest**

> ⚠️ Gebruik **niet** de groene knop **Code → Download ZIP** — daarmee downloadt u de ruwe ontwikkelbranch. Release-pakketten zijn geversioneerd, getest en klaar voor productie.

## Installatie

1.  Plaats de map `domainnameapi` in de map `Pro/3rdparty/domain/`, of upload deze via FTP.

## Configuratie in het Control Panel

1.  Navigeer naar `Control -> Services -> Registrars`.

   ![img1.png](img1.png)

2.  Klik op de knop **"Registrar Toevoegen"**.

    ![img2.png](img2.png)

3.  Selecteer **"DomainNameApi"** als de API.


4.  Voer uw gebruikersnaam en wachtwoord in.

    ![img3.png](img3.png)

5.  Klik op **"Opslaan"**.

## 🔑 API-inloggegevens — Gebruikersnaam/Wachtwoord of Reseller ID/API Key?

Beide worden ondersteund — vul ze in dezelfde twee modulevelden in; de module detecteert automatisch welke API gebruikt moet worden:

| U heeft | Veld "Gebruikersnaam" | Veld "Wachtwoord" | Gebruikte API |
|---|---|---|---|
| **Nieuwe panelgegevens** (aanbevolen) | Reseller ID — UUID zoals `xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` | API Key | REST |
| **Legacy-gegevens** | API-gebruikersnaam | API-wachtwoord | SOAP |

> 💡 U vindt uw **Reseller ID** en **API Key** in uw DomainNameAPI-panel onder **API Settings**.
> ⚠️ Dit zijn **API-inloggegevens** — het e-mailadres en wachtwoord waarmee u in het panel inlogt, werken hier **niet**.

Er is geen extra configuratie nodig — als het gebruikersnaamveld een UUID bevat, gebruikt de module de moderne REST API, anders de klassieke SOAP API.

## Domeinen Importeren

1.  Na het opslaan van de registrar-instellingen, wordt u doorverwezen naar het scherm voor het importeren van domeinen.
2.  Hier kunt u de gewenste domeinen selecteren en importeren.

    ![img4.png](img4.png)
    ![img5.png](img5.png)

## Gebruik

1.  Na de configuratie en import kunt u producten aanmaken en domeinen registreren en beheren via de DomainNameApi integratie.

    ![img6.png](img6.png)
