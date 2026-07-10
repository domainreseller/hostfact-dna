<div align="center">  
  <a href="README-TR.md"   >   TR <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/TR.png" alt="TR" height="20" /></a>  
  <a href="README-EN.md"> | EN <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/US.png" alt="EN" height="20" /></a>  
  <a href="README-DE.md"> | DE <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/DE.png" alt="DE" height="20" /></a>  
  <a href="README.md"> | NL <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/NL.png" alt="NL" height="20" /></a>  
</div>

# DomainNameApi Integration Documentation (EN)

## 📦 Download — always use Releases!

⬇️ **Get the latest tested version here: https://github.com/domainreseller/hostfact-dna/releases/latest**

> ⚠️ Do **not** use the green **Code → Download ZIP** button — that downloads the raw development branch. Release packages are versioned, tested and production-ready.

## Installation

1.  Place the `domainnameapi` folder into the `Pro/3rdparty/domain/` directory, or upload it via FTP.

## Configuration in the Control Panel

1.  Navigate to `Control -> Services -> Registrars`.

    ![img1.png](img1.png)

2.  Click the **"Add Registrar"** button.

    ![img2.png](img2.png)

3.  Select **"DomainNameApi"** as the API.


4.  Enter your username and password.

    ![img3.png](img3.png)

5.  Click **"Save"**.

## 🔑 API Credentials — Username/Password or Reseller ID/API Key?

Both are supported — enter them into the same two module fields; the module detects which API to use automatically:

| You have | "Username" field | "Password" field | API used |
|---|---|---|---|
| **New panel credentials** (recommended) | Reseller ID — UUID like `xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` | API Key | REST |
| **Legacy credentials** | API username | API password | SOAP |

> 💡 Find your **Reseller ID** and **API Key** in your DomainNameAPI panel under **API Settings**.
> ⚠️ These are **API credentials** — your panel login e-mail and password will **not** work here.

No extra configuration is needed — if the username field contains a UUID the module uses the modern REST API, otherwise classic SOAP.

## Importing Domains

1.  After saving the registrar settings, you will be redirected to the domain import screen.
2.  Here you can select and import the desired domains.

    ![img4.png](img4.png)
    ![img5.png](img5.png)

## Usage

1.  After configuration and import, you can create products and register and manage domains through the DomainNameApi integration.

    ![img6.png](img6.png) 