# What is USBWebserver?

## USBWebserver is a combination of popular webserver software: Apache, MySQL, PHP and phpMyAdmin. With USBWebserver it is possible to develop and show your PHP websites everywhere and anytime. The main advantage of USBWebserver is that you can use it from USB or a regular CD.

## USBWebserver is perfect for:

* Demonstrating an offline version of your website
* Develop PHP websites anywhere and anytime
* No need for expensive hosting
* Working at multiple locations on the projects
* A good test before putting your website online
* And many more

## USBWebserver kan perfect dienen voor:

* U klanten offline een versie van hun website laten zien
* Overal makkelijk en snel verder het het ontwikkelen van u website
* PHP website's programmeren zonder dure hosting
* Het thuis en op school werken aan Php opdrachten
* Eerst lokaal U website grondig testen voordat u deze online zet
* En vele andere mogelijkheden

## Vaak gestelde vragen :

1. Waar moet ik mijn bestanden neerzetten?
Al u php bestanden moet u in de map root plaatsen.
U website is vervolgens te bereiken via http://localhost:8080/.

2. MySQL start niet op.
Dit probleem kan zich voordoen als u al eerder MySQL op uw computer heeft geinstalleerd. Er staat dan een configuratie bestand in uw windows of ssytem32 map die door usbwebserver gelezen word.
Door dit bestand genaamd my.ini te verwijderen of hernoemen moet usbwebserver werken.

3. Hoe kan ik bestanden chmodden?
Bij USBWebserver is het niet nodig om bestanden/mappen te chmodden als u bestanden wilt uploaden/bewerken met PHP.
Dit komt omdat USBWebserver op Windows draait.

4. Hoe pas ik de config bestanden van Apache/MySQL/PHP aan?
Al deze config bestanden staan in de map settings. Na het aanpassen van 1 van deze bestanden moet u USBWebserver herstarten voordat de wijzigingen zijn doorgevoerd.

5. Ik krijg error's die ik op mijn normale hosting niet heb.
USBWebserver is standaard ingesteld op het hoogste foutmelding niveau. U kunt deze instelling wijzigen in het bestand settings/php.ini op regel 345.
Om alleen de meest gangbare foutmeldingen weer te geven vervang deze regel door: error_reporting = E_ALL & ~E_NOTICE.

6. Hoe zet ik mijn website online?
U kunt al u bestanden uit de root map kopieren naar hosting door middel van een ftp programma.
Om de databases over te zetten moet u naar PhpMyAdmin gaan en hier klikken op Export.
Daar kunt u de betreffende database selecteren en deze exporteren.
Daarna moet u naar PhpMyAdmin van u hosting gaan en daar op SQL klikken.
Plak de export in dit vak en druk op uitvoeren.

7. Hoe kunnen andere mensen mijn website bekijken?
USBWebserver is een programma die het mogelijkmaakt lokaal op uw computer gebruik te maken van Apache/PHP.
Indien u wilt dat anderen uw website kunnen bekijken kunt u het beste een webhosting pakket aanschaffen.

8. Wat zijn de inlog codes van phpmyadmin?
Gebruikersnaam is 'root' en het wachtwoord 'usbw'.

9. Hoe kan ik mails versturen via USBWebserver.
Om mail te versturen is connectie met een smtp server nodig.
Een smtp server zit niet (meer) bij usbwebserver, omdat deze vaak als virussen worden gezien door virus scanners.
Wilt u toch mail versturen zult u een eigen smtp server moeten instellen voor php.
Open het bestand settings/php.ini op regel 752, daar staat het volgende:

```
    [mail function]
    ; For Win32 only.
    SMTP = localhost
    smtp_port = 25
```

Vervang localhost door u eigen smtp server.
