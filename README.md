# OME Stream pentru Samsung Tizen - descarcari

[Descarca instalatorul Windows si pachetul WGT](https://github.com/elisunou/ome-stream-tizen-downloads/releases)

Versiune de dezvoltare, separata de APK-ul Android. Nu include DataScene. Nu a fost inca validata pe un televizor fizic.

## Instalare

1. Descarca `OME-Stream-Tizen-Installer-Windows.zip` din Releases si dezarhiveaza-l.
2. Ruleaza `START-INSTALL.cmd` pe un PC Windows conectat la aceeasi retea cu televizorul.
3. Pe TV, deschide Apps, tasteaza `12345`, activeaza Developer Mode, introdu IP-ul calculatorului si reporneste TV-ul.
4. In instalator: introdu IP-ul televizorului, apasa **Conecteaza**, alege fisierul `.wgt` si apasa **INSTALEAZA PE TV**.

Necesita SDK-ul Samsung/Tizen instalat: SDB, Web CLI, TV Extension si Samsung Certificate Extension. Butonul **Instalare SDK** deschide pagina oficiala Samsung. SDK-ul nu este inclus in ZIP. Nu sunt necesare Node.js sau Git pentru folosirea instalatorului.

## Semnatura

**Fisierul `OME-Stream-Tizen-0.1.0-UNSIGNED.wgt` este NESEMNAT. Nu se instaleaza singur pe un televizor Samsung fizic.**

Instalatorul poate semna local o copie a acestuia folosind un profil Samsung existent care include DUID-ul televizorului. Butonul **Certificate Samsung** deschide managerul oficial pentru configurarea profilului si autentificare. Acesti pasi nu sunt automatizati. Daca ai deja un WGT semnat corect pentru televizorul tinta, il poti selecta si instala direct.

Detectarea fisierelor de semnatura nu reprezinta validare criptografica; televizorul verifica certificatul la instalare. Nu exista in aceasta pagina certificate, parole, chei Webtor sau DUID-uri personale. Nu deschide porturi in router pentru instalare.

## Dupa instalare

Configureaza in Setari conturile proprii FileList, SpeedApp, Seedpool, addonurile si serviciul TV live. Webtor REST API necesita o cheie personala si un plan platit. Compatibilitatea redarii si a trackerelor necesita testare cu propriile conturi.

Interfata, adaptoarele Webtor si instalatorul au trecut teste locale cu raspunsuri simulate. Nu este o declaratie ca toate functiile Android au fost portate sau ca instalarea pe TV a fost verificata. Sincronizarea Google Drive/Trakt, notificari de fundal, magazinul de skinuri Android, import ZIP, DLNA, trailere YouTube si Subs.ro nu sunt inca portate.

## Documentatie Samsung

- [Conectare TV / Developer Mode](https://developer.samsung.com/smarttv/develop/getting-started/using-sdk/tv-device.html)
- [SDK](https://developer.samsung.com/smarttv/develop/getting-started/setting-up-sdk/installing-tv-sdk.html)
- [Certificate](https://developer.samsung.com/smarttv/develop/tools/additional-tools/vscode/creating-certificates.html)
