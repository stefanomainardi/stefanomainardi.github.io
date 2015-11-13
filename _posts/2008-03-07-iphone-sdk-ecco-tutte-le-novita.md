---
title: iPhone SDK ecco tutte le novità
author: Stefano Mainardi
layout: post
permalink: /2008/03/07/iphone-sdk-ecco-tutte-le-novita/
podPressPostSpecific:
  - 's:245:"a:6:{s:15:"itunes:subtitle";s:15:"##PostExcerpt##";s:14:"itunes:summary";s:15:"##PostExcerpt##";s:15:"itunes:keywords";s:17:"##WordPressCats##";s:13:"itunes:author";s:10:"##Global##";s:15:"itunes:explicit";s:2:"No";s:12:"itunes:block";s:2:"No";}";'
btc_comment_counts:
  - 'a:0:{}'
btc_comment_summary:
  - 'a:0:{}'
dsq_thread_id:
  - 2303403473
categories:
  - Tech
tags:
  - apple
  - iphone
  - itouch
  - sdk
  - sviluppo
---
Dopo mesi di attesa Apple ha **finalmente rilasciato** l&#8217;SDK formalmente il *Software Developer Kit*, per tutti gli sviluppatori o Software House che vogliano cimentarsi nello sviluppo di applicazioni per iPhone o iPod Touch con **strumenti ufficiali** messi a disposizione da Apple. Anche se nel corso dei mesi sono nate **moltissime applicazioni di qualità** totalmente amatoriali.

<p style="text-align: center">
  <img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/iphone_sdk.gif" height="159" width="476" />
</p>

La novità più importante di questo rilascio è sicuramente il kit **iPhone Enterprise**, facendo entrare questo dispositivo nell&#8217;olimpo del **mercato business** aggiungendo funzionalità richieste dal mercato come ad esempio **la sincronizzazione con Microsoft Exchange attraverso ActiveSync**, funzioni **Push per email e contatti**, l&#8217;aggiunta di **protocolli di sicurezza** come il **WPA2/802.1x** e supporto a** Cisco IPsec VPN**. Tutto questo sarà disponibile nel prossimo aggiornamento software per iPhone, ed integrato all&#8217;interno del nuovo firmware.

<!--more-->

### SDK &#8211; Tutto (o quasi) quello che c&#8217;è da sapere

All&#8217;inizio dell&#8217;evento si è parlato delle applicazioni web, si parla di **oltre mille** applicazioni e del grande successo ed interesse che hanno riscosso, con il rilascio di questo tool tutti potranno utilizzare gli stessi strumenti utilizzati da Apple per creare **applicazioni stand-alone**, e quindi più funzionali.

E&#8217; stata illustrata nel dettaglio la piattaforma che come si era detto è **basata su OSX **di cui ne condivide gran parte delle tecnologie ad esempio **CoreAudio** e **CoreAnimation**, **OpenGL** tranne Cocoa che è stato sviluppato per funzionare con interfaccia classiche, *tastiera e mouse*, ed è stata quindi sviluppata una versione ad-hoc per interazione con il device *Multitouch* denominato, appunto, **Cocoa Touch**, il tutto accessibile ed integrato ovviamente nell&#8217;IDE di sviluppo Xcode.

<p style="text-align: center">
  <img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/apple-sdk-01.jpg" />
</p>

<small> </small>

<p align="center">
  <small>(Foto di <a href="http://www.engadget.com/2008/03/06/live-from-apples-iphone-press-conference/" target="_blank">Engadget</a>)</small>
</p>

Tanti gli strumenti integrati ed interessanti, come l&#8217;emulatore interno **Iphone Simulator**

<p style="text-align: center">
  <img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/apple-sdk-02.jpg" />
</p>

<small> </small>

<p align="center">
  <small>(Foto di <a href="http://www.engadget.com/2008/03/06/live-from-apples-iphone-press-conference/" target="_blank">Engadget</a>)</small>
</p>

Strumento in grado di **riprodurre fedelmente** il funzionamento del dispositivo, inclusi i classici &#8220;movimenti&#8221; che possiamo fare sul display multi-touch (swipe, pinch ecc..), **ottimo strumento** per fare test e debug senza avere un dispositivo fisico.

Interessante anche lo strumento di **debugging grafico**, che mostra in realtime ed in situazioni di stress **il *comportamento* dell&#8217;applicazione**, ottimo strumento e più veloce di un debugger classico per capire visivamente **come e dove ottimizzare** la nostra applicazione.

Durante la presentazione sono state presentate **nuove applicazioni dimostrative**, nello specifico alcuni videogiochi che facevano **uso di OpenGL** ed il risultato è davvero spettacolare (**ma la batteria?**), ed applicazioni create, a detta loro, in **meno di due settimane** come ad esempio un *distorsore* di foto che fa uso del multitouch. Ed ovviamente il classico Hello World! creato al volo per far vedere la semplicità dei nuovi strumenti.

<p style="text-align: center">
  <img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/apple-sdk-03.jpg" />
</p>

<p align="center">
  <small>(Foto di <a href="http://www.engadget.com/2008/03/06/live-from-apples-iphone-press-conference/" target="_blank">Engadget</a>)</small>
</p>

Sono state mostrate anche nuove applicazioni, **il messenger AIM di AOL**, e qualche demo di **Sega ed Electronics Arts**, i quali si sono **dichiarati entusiasti** delle potenzialità offerte dall&#8217;iPhone, pare che ne vedremo delle belle anche in questo campo. Nel <a href="http://www.apple.com/quicktime/qtv/keynote/" target="_blank">video della presentazione</a> pubblicato da poco potete vedere la dimostrazione delle nuove applicazioni.

Sono **tante le feature**s ed è stata allestita una pagina apposita con tutti i <a href="http://developer.apple.com/iphone/program/details.html" target="_blank">dettagli</a> , ed è anche possibile **scaricare questo ormai famoso SDK** da <a href="http://developer.apple.com/iphone/sdk1/" target="_blank">questa pagina</a>. *Inizierò subito a fare i primi esperimenti*.

Per chi volesse invece pubblicare le proprie applicazioni dovrà pagare una quota di **99$ per il programma Standard**, e **299$ per il programma Enterprise**, entrambe daranno diritto al supporto tecnico di Apple.

### Le applicazioni come saranno distribuite?

Come previsto tutte le applicazioni saranno **distribuite tramite iTunes**, in una nuova sezione che prenderà il nome di **iTunes App Store** accessibile sia da iPhone che tramite iTunes su Mac e PC. E&#8217; interessante notare come sia state *prese in prestito idee* dalla famosa applicazione Installer.app, come ad esempio l&#8217;aggiornamento automatico delle applicazioni installate.

<p style="text-align: center">
  <img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/apple-sdk-04.jpg" />
</p>

<small> </small>

<p align="center">
  <small>(Foto di <a href="http://www.engadget.com/2008/03/06/live-from-apples-iphone-press-conference/" target="_blank">Engadget</a>)</small>
</p>

La politica commerciale è interessante e meno restrittiva di come si pensava. Lo sviluppatore *o la Software House* decideranno il prezzo di vendita, a loro andrà il **70% del ricavato** ed il restante **30% entrerà di diritto nelle casse di Apple**, mentre **tutte le applicazioni freeware saranno disponibili ed ospitate a livello gratuito. **Ottima mossa.

### Tutte queste novità sono già disponibili?

Per ora è stata rilasciata una versione beta del firmware 2.0 ad alcuni tester, mentre per la **versione definitiva ci sarà da aspettare Giugno**, con cui sono ripartiti le speculazioni (*rumors?*) per cui Apple presenterà in contemporanea una nuova versione UMTS e aggiornata di iPhone.

L&#8217;aggiornamento sarà **gratuito per i possessori di iPhone**, mentre **i possessori di iPod Touch pagheranno un prezzo &#8220;simbolico&#8221;**, dicono per *motivi fiscali*, non si capisce bene quali siano e perchè i possessori di iPod Touch debbano pagare ogni tot una penale ad Apple, come il recente aggiornamento delle nuove applicazioni. Vedremo come la faccenda verrà gestita.

### C&#8217;è altro da sapere?

Ti consiglio di leggere le domande fatte dai giornalisti presenti e [prontamente tradotte][1] da **Kiro** di Melamorsicata.

Tutti si aspettavano che venisse annunciato **l&#8217;iPhone in Italia**, visti i recenti accordi con Tim, ma anche questa volta siamo rimasti tutti a **bocca asciutta**, ma possiamo consolarci con la supervalutazione dell&#8217;euro sul dollaro che ci permette di acquistare un iPhone da 8Gb dagli USA a **poco meno di 270€**, *a mali estremi estremi rimedi*.

 [1]: http://www.melamorsicata.it/mela/2008/03/06/domande-e-risposte-alla-conferenza-apple-iphone-software-roadmap%e2%80%9d/