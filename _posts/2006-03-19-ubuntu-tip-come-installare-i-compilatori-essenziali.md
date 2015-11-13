---
title: 'Ubuntu-Tip: Come installare i compilatori essenziali?'
author: Stefano Mainardi
layout: post
permalink: /2006/03/19/ubuntu-tip-come-installare-i-compilatori-essenziali/
podPressPostSpecific:
  - 's:180:"a:6:{s:15:"itunes:subtitle";s:0:"";s:14:"itunes:summary";s:0:"";s:15:"itunes:keywords";s:0:"";s:13:"itunes:author";s:0:"";s:15:"itunes:explicit";s:0:"";s:12:"itunes:block";s:0:"";}";'
btc_comment_counts:
  - 'a:0:{}'
btc_comment_summary:
  - 'a:0:{}'
dsq_thread_id:
  - 2097759713
categories:
  - Free Software
  - Informatica
  - 'Linux &amp; Co.'
---
![Ubuntu][1]  
Questo piccolo tip lo dedico al mio amico [PabloMoroe][2] il quale dopo aver installato Ubuntu (credo sia uno dei miei CD che ho fatto circolare all&#8217;interno della distratta Facoltà di Informatica dell&#8217;Aquila, dove di Software Libero e GNU/Linux proprio non se ne parla) mi chiedeva dove trovare e come installare gli strumenti di sviluppo essenziali. Ad esempio il buon [**GCC**][3].  
Bene, essendo Ubuntu una derivata di Debian di cui ha preso tutti i pregi, ci viene in aiuto il carissimo tool da linea di comando **[apt-get][4] **il quale con semplici passi ci permette di modellare al meglio il nostro parco software installato.

In UBUNTU ci sono i *metapackage, *ovvero quei **mega**pacchetti tematici che ci semplificano il lavoro e ci permettono di installare in pochi passi una serie di programmi della stessa serie, in questo caso i pacchetti di sviluppo.

Apriamo quindi il terminale da **Applicazioni **&#8212;-> **Accessori** &#8212;-> **Terminale**

**$ sudo apt-get update****  
$ sudo apt-get install build-essential**

(Ovviamente questa operazione va fatta con il PC connesso ad internet, visto che scaricheremo ed installeremo i pacchetti da remoto)

Se la linea di comando risulta ostica possiamo avvalerci del tool **Synaptic **(**Sistema**&#8212;> **Amministrazione**&#8212;> **Gestore Pacchetti Synaptic**) che non è altro che una GUI per APT. La procedura è identica, basta cercare il pacchetto &#8220;build-essential&#8221; spuntare la casella e fargli avviare l&#8217;installazione.

Avremo a disposizione dopo questa semplice e veloce operazione G++ (per compilare codice C++) e GCC aggiornati alle versioni più recenti.  
Davvero molto semplice, a dispetto di chi pensa che Linux sia solo per Guru.

 [1]: http://www.ubuntu.com/include/circle-510.png "Ubuntu"
 [2]: http://www.pablomoroe.com/blog "Pablomoroe"
 [3]: http://gcc.gnu.org/ "GCC"
 [4]: http://www.debian.org/doc/manuals/apt-howto/ "APT-GET HOW-TO"