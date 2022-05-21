---
title: "Multifaktor Autentifikation"
author: "Sippo Rossi and Irfan Kanat"
date: "12/04/2021"
output: pdf_document
titlepage: true
titlepage-rule-color: "360049"
titlepage-background: "backgrounds/background2.pdf"
urlcolor: blue
---

Tidssvarende autentifikation anvender tre faktorer:

1- Noget du kender til, eksempelvis adgangskoder

2- Noget du er, eksempelvis fingeraftryk

3- Noget du har, eksempelvis nøgler

Multifaktor autentifikation har den konsekvens, at du ikke kun benytter en enkelt men flere forskellige faktorer samtidigt. Det er helt centralt for beskyttelse af konti der indeholder personfølsomme eller finansielle oplysninger. Som eksempelvis bank eller e-mail konti. Med multifaktor autentifikation er der, også selvom en hacker opnår adgang og kendskab til en beskyttelsesfaktor, ekstra sikkerhedstjek, der forhindre fuld adgang.

I Danmark har vi de nationale autentifikationssystemer NemID og MitID. Nøglekortet er noget du har og kan valideres af systemet. Uheldigvis er det resterende internet ikke omfattet af vores ellers fantastiske ID-systemer. Derfor er andre løsninger nødvendige.

Nogen af disse metoder kan umiddelbart virke en smule primitive, såsom engangskoder via SMS eller e-mail. Andre er mere sofistikerede, som eksempelvis benyttelse af en autentifikations applikation installeret på en mobiltelefon, eller en hardware nøgle som YubiKey.

Nu vil vi gennemgå brugen af Google Authenticator. Google Authenticator er en autentifikationsapplikation designet for at øge sikkerheden for dine personlige online-konti.

## Opsætning af Google Authenticator

Hent og installer Google Authenticator applikationen fra app store or play store.

[Play Store Link for Google Authenticator](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=en_US&gl=US)

[App Store Link for Google Authenticator](https://apps.apple.com/us/app/google-authenticator/id388497605)

## Opsætning af en Reddit konto for Google Authenticator

Du har brug for multifactor autentifikation for dine kritiske onlinekonti. Måske er Reddit ikke det bedste eksempel, men det illustrerer tydeligt fremgangsmetoden for opsætning af Authenticator.

Besøg Reddit websitet, klik ind på din konto og gå til settings. Vælg fanen ”Saftey & Privacy”. 

![Safety settings](figures/2FA0.png)

Scroll ned indtil du ser two-factor authentication.

![2 Factor Authentication](figures/2FA1.png)

Du bliver nu spurgt on din adgangskode, indtast og fortsæt. Du vil nu se en QR-kode på skærmen.

![The QR Code](figures/2FA3.png)

Skift nu til din Google Authenticator app på in mobiltelefon. Google Authenticator appen tillader ikke screenshots, derfor vil den resterende fremgangsmetode ikke være illustreret. Klik + ikonet i bunden af skærmbilledet og vælg skanning af QR-kode.

Skan QR-koden på skærmen, og der vil nu fremkomme en verifikationskode in din Authenticator app. Indtast koden i Reddit.

**Vigtigt**. Du kan miste adgang til din mobiltelefon eller din Authenticator app. For at genoprette din konto, kan Reddit generere flere engangskoder. Kopier disse koder og gem dem i din password manager. Hvis du mister adgangen til din Authenticator app, kan du nulstille din konto via en engangskode. **Du kan miste adgangen til disse konti, hvis du mister adgang till både appen og engangskoderne.** Derfor er det vigtigt, at de gemmes sikkert med din password manager.

Næste gang du logger ind med din adgangskode, vil Reddit spørge efter en kode. Åben din Authenticator app, og indtast det tilhørende sekscifrede tal.

![Codes reset frequently](figures/Authenticator2.jpeg)



\vfill
![CC4](CC4.png) This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).
