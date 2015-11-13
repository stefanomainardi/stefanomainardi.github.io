---
title: Il mio Macbook artigianale
author: Stefano Mainardi
layout: post
permalink: /2008/08/31/il-mio-macbook-artigianale/
podPressPostSpecific:
  - 's:245:"a:6:{s:15:"itunes:subtitle";s:15:"##PostExcerpt##";s:14:"itunes:summary";s:15:"##PostExcerpt##";s:15:"itunes:keywords";s:17:"##WordPressCats##";s:13:"itunes:author";s:10:"##Global##";s:15:"itunes:explicit";s:2:"No";s:12:"itunes:block";s:2:"No";}";'
btc_comment_counts:
  - 'a:0:{}'
btc_comment_summary:
  - 'a:0:{}'
dsq_thread_id:
  - 2185842029
categories:
  - Hi-tech
tags:
  - apple
  - hackintosh
  - macbook
  - msi wind u100
  - netbook
---
Mi riallaccio al titolo dei uno dei *<a href="http://www.stefanomainardi.com/2006/04/10/il-mio-macintel-artigianale/" target="_blank">miglori post</a> *(<acronym title="A mio modesto parere">IMHO</acronym>) che è apparso sulle pagine di questo blog, ormai più di due anni fa, quando la Apple inizio la svolta verso processori x86, oggi la rivoluzione è stata fatta e i Mac con processori Intel sono realtà, ma con qualche effetto indesiderato.

In quel post spiegavo come ero risucito a costruirmi un **vero clone mac** totalmente amatoriale, ma **completamente funzionante** e con prestazioni identiche (*se non superiori in tanti casi*) ai Macpro venduti a peso d&#8217;oro.

Questa volta vi presento il mio Macbook Nano (*si il nome l&#8217;ho inventato io*), ovvero un **clone perfetto** di un Macbook costruito su hardware generico e su uno stupendo <a href="http://global.msi.com.tw/index.php?func=proddesc&prod_no=1474&maincat_no=135" target="_blank">Msi Wind U100</a>, il nuovo ultracorazzato netbook (*che nome osceno*) di casa MSI. Le caratteristiche sono di tutto rispetto, processore Intel Ato, 1Gb di Ram, 80Gb di HD, Wifi, Bluetooth, Webcam da 1,3 Megapixel.

L&#8217;unico neo attuale è la batteria a 3 celle, che **non supera le due** ore di autonomia, ma sul mercato sono arrivati gli stessi modelli con **batteria a 6 celle**, superando l&#8217;**autonomia di cinque ore.** Insomma un passo in avanti rispetto agli EeePC di Asus. La qualità del design e la cura dei dettagli non è minimamente paragonabile a quella dei prodotti Apple, anche se devo dire che **il design di questo piccolletto è davvero ben curato**. Il portatile viene fornito di default con XP SP3, MSI <a href="http://www.suseitalia.org/modules/news/article.php?storyid=971" target="_blank">aveva annunciato</a> una versione con Linux Novell Desktop (ndr. Suse) ma pare che nel mercato italiano non arriverà, come al solito direi.

<!--more-->

### Cosa devo fare per installare MacOSX sull&#8217;MSI WIND U100?

Premetto che attualmente è un&#8217;operazione illegale installare copie di MacOSX su hardware non Apple, la <a href="http://images.apple.com/legal/sla/docs/macosx105.pdf" target="_blank">EULA di Apple</a> non lo permette. Pare ci sia una [causa in corso][1] con l&#8217;antitrust tra Apple e la [Psystar][2] che ha commercializzato negli ultimi mesi computer pienamente compatibili con Leopard, aggiornamenti di sistema inclusi.L&#8217;installazione di Leopard è davvero semplicissima. Dovete sapere però che la scheda wifi integrata, non funzionerà su Mac e dovete quindi provvedere a sostituirla. Si tratta di schedine Mini Pci-Express, su Ebay se ne trovano a bizzeffe, io ho trovato una [Apple Airport Extreme][3] su Ebay al costo di 25 Euro. Trovate qui <a href="http://wind-osx86.wikispaces.com/Working+Wifi+cards+(substitutes)" target="_blank">una lista</a> di schedine compatibili. Visto che ho dovuto aprirlo ho aggiunto anche un banco da 1GB di Ram, qui trovate <a href="http://netbookmag.com/2008/07/07/tutorial-advent-4211-memory-upgrade-msi-wind/" target="_blank" title="Msi WIND Ram Upgrade">i dettagli</a> su come procedere.

Nota importante: Prima di installare la memoria vi consiglio di annotarvi i dettagli (Marca, Modello, Numero di serie), li dovrete inviare via mail all’ indirizzo ***notebook@msi-computer.it , ***inserendo anche il seriale del notebook, in modo tale da preservare la garanzia ed avere l&#8217;approvazione di MSI per procedere autonomamente all&#8217;aggiornamento.

Ma veniamo al dunque.

Quello che ci serve è sostanzialmente : una copia di Leopard *oppurtanamente patchata*, reperibile presso i famosi motori di ricerca torrent (*Kalyway 10.5.2*), ed una manciata di <acronym title="Estensioni del kernel">kext</acronym> da installare (*driver in soldoni*) per l&#8217;hardware specifico. Qualcuno oltreoceano mi ha preceduto ed <a href="http://www.modaco.com/content/asus-eee-pc-http-www-eeeasy-com/270099/pauls-complete-guide-to-installing-osx-leopard-on-your-msi-wind-advent-4211/" target="_blank">ha scritto una guida</a> passo passo, con tanto di link e zip contentente tutto l&#8217;occorrente. Vi assicuro che tutto **è più semplice** di quanto vi aspettiate, nel giro di un&#8217;ora avrete il vostro Leopard pronto all&#8217;uso.

Ho fatto un piccolo video a corredo di quello che ho scritto, perdonate la scarsa qualità (come si dice in questi casi)



Le cuffie che (non) faccio vedere nel video sono le [Logitech Notebook Headset][4]

### Perchè dovrei installarci MacOSX?!

Uhm, le risposte potrebbero essere molteplici.

Per quanto mi riguarda, oltre ad essere un divertente esperimento stilistico, negli ultimi tempi ho avuto modo di lavorare molto su MacOS e devo dire che lo trovo un&#8217;ottimo compromesso fra stabilità e flessibilità. E sinceramente non riuscirei più a fare a meno di Textmate, una vera killerapp.

Non mi dilungo sulle motivazioni, il flamewar sui vari SO è sempre alle porte, ed è meglio evitarlo <img src="http://www.stefanomainardi.com/wp-includes/images/smilies/icon_wink.gif" alt=";)" class="wp-smiley" />

### Qualche link utile?

Sono nate delle community attorno a questi nuovi portatilini, quella di Modaco ve l&#8217;ho segnalata ed è dove trovate la guida, l&#8217;altra è [Msiwind.net][5] e l&#8217;ottima comunità italiana [EEEPc.it][6].

Per il resto l&#8217;area commenti è a vostra disposizione. (so che mi pentirò di averlo scritto&#8230;)

 [1]: http://www.melablog.it/post/6619/psystar-confermata-la-carta-antitrust
 [2]: http://www.psystar.com/
 [3]: http://cgi.ebay.it/ws/eBayISAPI.dll?ViewItem&item=120299385675&ssPageName=ADME:X:RTQ:IT:1123
 [4]: http://www.logitech.com/index.cfm/webcam_communications/internet_headsets_phones/devices/223&#038;cl=us,en
 [5]: http://www.msiwind.net
 [6]: http://www.eeepc.it