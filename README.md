\# Receipt Camera Uploader



Simple Termux script til at tage billeder af kvitteringer og uploade dem automatisk til Google Drive.



\## Formål

Dette script er grundstenen til et budget tracking system der giver detaljeret indsigt i indkøbsmønster på vare-niveau.



\## Features

\- Tag billede med Termux kamera

\- Auto-upload til Google Drive

\- Organiserer i mapper efter måned/år

\- Opretter automatisk nye mapper hvis nødvendig

\- Termux Widget support - 1-tap funktionalitet



\## Prerequisites



\### På Android:

\- \[Termux](https://f-droid.org/packages/com.termux/) (installer fra F-Droid, IKKE Google Play)

\- \[Termux:API](https://f-droid.org/packages/com.termux.api/)

\- \[Termux:Widget](https://f-droid.org/packages/com.termux.widget/) (valgfri, men anbefalet)



\### Google Cloud Setup:

\- Google Cloud projekt med Drive API aktiveret

\- OAuth2 credentials (se `setup/google\_api\_setup.md`)



\## Installation



\### 1. Termux Setup

```bash

\# Opdater Termux

pkg update \&\& pkg upgrade



\# Installer nødvendige pakker

pkg install python git termux-api



\# Giv Termux adgang til storage

termux-setup-storage



\# Clone repository

git clone https://github.com/SolidAlphaVFX/receipt-camera-uploader.git

cd receipt-camera-uploader



\# Installer Python dependencies

pip install -r requirements.txt

