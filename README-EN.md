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


4.  Enter your Reseller ID and API Key (see below).

    ![img3.png](img3.png)

5.  Click **"Save"**.

## 🔑 API Credentials

Enter your **Reseller ID** into HostFact's "Username" field and your **API Key** into its "Password" field.

> 💡 Find your **Reseller ID** and **API Key** in your DomainNameAPI panel under **API Settings**.
> ⚠️ These are **API credentials** — your panel login details will **not** work here.

## Importing Domains

1.  After saving the registrar settings, you will be redirected to the domain import screen.
2.  Here you can select and import the desired domains.

    ![img4.png](img4.png)
    ![img5.png](img5.png)

## Usage

1.  After configuration and import, you can create products and register and manage domains through the DomainNameApi integration.

    ![img6.png](img6.png) 