---
title: Controlla il tuo mac da remoto con iPhone
author: Stefano Mainardi
layout: post
permalink: /2008/01/24/controlla-il-tuo-mac-da-remoto-con-iphoneitouch/
podPressPostSpecific:
  - 's:245:"a:6:{s:15:"itunes:subtitle";s:15:"##PostExcerpt##";s:14:"itunes:summary";s:15:"##PostExcerpt##";s:15:"itunes:keywords";s:17:"##WordPressCats##";s:13:"itunes:author";s:10:"##Global##";s:15:"itunes:explicit";s:2:"No";s:12:"itunes:block";s:2:"No";}";'
btc_comment_counts:
  - 'a:0:{}'
btc_comment_summary:
  - 'a:0:{}'
dsq_thread_id:
  - 2185839954
categories:
  - Tech
tags:
  - apple
  - iphone
  - ipod touch
  - itouch
  - remote buddy
  - telekinesis
  - vnsea
---
Ed eccoci ad un altro appuntamento con la rubrica **iPhone/iTouch**, questa volta parleremo dei software in grado di rendere i nostri gioiellini dell&#8217;*estensioni remote* del nostro Mac, grazie alle quali potremmo controllare **moltissime delle funzioni del sistema operativo** e delle più **comuni applicazioni** del mondo Apple, come fosse un vero e proprio telecomando.

<p align="center">
  <img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/remote.png" />
</p>

Una delle applicazioni che vi andrò a presentare in realtà funziona anche su **altre piattaforme**, ad esempio *Windows o Linux *o tutti i sistemi che hanno la possibilità di avere un server [VNC][1] in ascolto, *di cui pochi sanno che il brevetto fino all&#8217;acquisto di AT&T era dell&#8217;italianissima Olivetti. ***Altri tempi per l&#8217;IT italico**.

Ormai manca pochissimo al rilascio delle SDK e quindi applicazioni &#8220;**ufficiali**&#8221; e *certificate* per questi dispositivi, il che significa che a breve avremo una serie di **applicazioni installabili via Itunes** senza dover fare il Jailbreak del nostro dispositivo. Io attualmente sono rimasto al firmware 1.1.1 visto e considerato che con la politica di **chiusura estrema** di Apple facendo un aggiornamento firmware mi troverei tra le mani **un dispositivo mozzato delle sue potenzialità**.

<!--more-->

### Vnsea

Vnsea è un port per iPhone del famoso &#8220;[Chicken of the VNC][2]&#8221; per MacOSX, non è altro che un client grafico per connettersi ad un qualsiasi server VNC, come dicevo nella premessa del post. La peculiarità di VNC è quella di poter collegarci al nostro pc ed usare il nostro desktop **graficamente** come se ci trovassimo di fronte ad esso, *questo detto in parole poverissime*.

Le funzionalità sono ottime, ed è stato sfruttato ottimamente il multitouch facendo uso di *gestures *oltre al classico &#8220;**tap**&#8221; che emula un click, ed il &#8220;**pinch**&#8221; per zoomare lo schermo, possiamo scorrere il nostro desktop **usando le due dita**, ed il tutto è spiegato in un menù contestuale all&#8217;interno dell&#8217;applicazione.

<p style="text-align: center">
  <img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/vnsea.jpg" />
</p>

<p align="center">
  <small>(<strong>1.</strong> Configurazione dell&#8217;applicazione / <strong>2.</strong> Zommatta del desktop / <strong>3.</strong> Vista generale dell&#8217;applicazione)</small>
</p>

In realtà il suo utilizzo, è **poco più di un giochino** non credo che in ambiti produttivi si abbia bisogno di un applicazione del genere viste **le ridotte dimensioni dello schermo**, auspico di più ad **applicazioni web **residenti sulle nostre macchine ed accessibili da **interfacce studiate appositamente** per questi dispositivi. Ma è comunque **gratificante** dal punto di vista &#8220;**geek**&#8221; usare il proprio MAC **dal palmo della mano.**

L&#8217;applicazione come sempre **è disponibile in Installer.app**, aggiungendo i <a href="http://www.google.it/search?q=community+sources&ie=utf-8&oe=utf-8&aq=t&rls=org.mozilla:it:official&client=firefox-a" target="_blank">Community Sources</a> ai vostri repository, ovviamente questo richiede che il vostro Ipod sia gia <a href="http://www.stefanomainardi.com/2007/10/24/il-futuro-in-un-tocco/" title="Ne avevo parlato qui" target="_blank">Jailbreaked</a>.

L&#8217;Homepage da dove seguirne gli sviluppi è su [Google Code][3].

### Telekinesis

Il progetto è **molto interessante**, ed Opensource, trattasi di una **serie di <acronym>Webapp</acronym>** che andranno a **controllare** e **gestire** svariati aspetti e software di sistema. Il funzionamento **è tanto semplice** quanto banale, basterà installare un **piccolo server** sul vostro mac, scaricandolo dal [sito ufficiale][4] e mandarlo in start, aprire Safari sul vostro iPhone/iTouch e digitare l&#8217;indirizzo IP della vostra macchina seguito dalla porta :5010 , in questo modo :

<p align="center">
  <code>https://&lt;INDIRIZZO_IP_DEL_TUO_MAC&gt;:5010</code>
</p>

Il software in questione è ancora in **fase sperimentale** ma **perfettamente funzionante** e con un interfaccia scarna ma davvero intuitiva e semplice da usare. Le possibilità di controllo sono molteplici, ad esempio gestire Itunes (play, stop, volume), fare ricerche con Spotlight, fare stream di <a href="http://code.google.com/p/telekinesis/wiki/MediaStreaming" target="_blank">musica e video</a> e molto altro.

<p style="text-align: center">
  <img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/telekinesis.jpg" />
</p>

<p style="text-align: center">
  <small> (Interfaccia di Telekinesis dal browser di iPhone/iTouch)</small>
</p>

L&#8217;idea è **molto interessante** e non c&#8217;è bisogno di installare nessun software all&#8217;interno dell&#8217;iPod, il framework di sviluppo è ben fatto e [creare nuove applicazioni][5] da innestare è semplicissimo date un occhiata al codice. Potrebbe essere utile un&#8217;applicazione del genere per tenere sotto controllo un server remoto, o per far partire all&#8217;occorrenza uno script di recupero o cose del genere.

### Remotebuddy

[Remotebuddy][6], è il **software definitivo** per controllare il vostro mac da remoto, è un software commerciale ad un prezzo più che ragionevole, ma viene [offerto in trial][7] per periodo di 30 giorni.

<p style="text-align: center">
  <img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/remotebuddy.jpg" />
</p>

<p style="text-align: center">
  <small>(<strong>1.</strong> Schermata iniziale / <strong>2.</strong> Ricerca simile a Spotlight / <strong>3.</strong> Una presentazione)</small>
</p>

Può gestire praticamente tutto del vostro mac, con un webserver costruito ad-hoc e devo dire che la **velocità di risposta** è davvero ottima. L&#8217;interfaccia non ha nulla da invidiare ad un applicazione stand-alone, è l&#8217;usabilità complessiva è ottima.

La funzione che mi sembra più interessante è quella di poter **essere un telecomando per le presentazioni** usando Keynote, oltre a **scorrere le slides** abbiamo anche il **puntatore a schermo**, stupefacente! O anche l&#8217;integrazione con [EyeTV][8] per **programmare le registrazioni** dei nostri programmi preferiti da remoto.

Per tutte le altre features e possibilità vi invito caldamente a provarlo, e magari farvi un giro nel **[sito ufficiale][6]** per capirne effettivamente le potenzialità.

### Conclusioni

Come sempre **sono molto soddisfatto** delle applicazioni che stanno nascendo attorno a questo dispositivo, e vedo che l&#8217;attenzione si sta spostando anche in ambito business vedi l&#8217;<a href="http://biz.yahoo.com/ap/080115/apple_ibm.html?.v=1" target="_blank">ultima mossa</a> di IBM di offrire Lotus ottimizzato proprio per iPhone e iPod Touch.

Le famose **SDK** stanno arrivando, e con il nuovo **firmware 1.1.3** abbiamo avuto un assaggio, **assai costoso** e [indigesto][9], di come verranno acquistate le applicazioni prossime, **e certificate** da Apple, con Itunes. Spero che Apple lasci più spazio in futuro alle comunità di sviluppatori, i quali hanno creato dei Software in alcuni casi davvero al di sopra delle aspettative favorendone di conseguenza **le vendite**.

*ps: Facciamo una colletta per il povero [**Gioxx**][10]? :-)*

 [1]: http://it.wikipedia.org/wiki/Virtual_Network_Computing
 [2]: http://www.geekspiff.com/software/cotvnc/
 [3]: http://code.google.com/p/vnsea/
 [4]: http://code.google.com/p/telekinesis/
 [5]: http://code.google.com/p/telekinesis/wiki/CreatingApplications
 [6]: http://www.iospirit.com/index.php?mode=view&obj_type=infogroup&obj_id=24&o_infogroup_objcode=infogroup-23&o1_infogroup_objcode=html-141&sid=5405701Gb5c10722cdf2c0a7
 [7]: http://www.iospirit.com/remotebuddy/download/
 [8]: http://www.elgato.com/elgato/int/mainmenu/home.en.html
 [9]: http://www.melamorsicata.it/mela/2008/01/17/tangente-sulle-applicazioni-per-itouch-arriva-la-petizione/
 [10]: http://gioxx.org/2008/01/17/e-stato-bello-non-averti-incontrato/
