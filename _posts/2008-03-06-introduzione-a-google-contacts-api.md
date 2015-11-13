---
title: Introduzione a Google Contacts API
author: Stefano Mainardi
layout: post
permalink: /2008/03/06/introduzione-a-google-contacts-api/
podPressPostSpecific:
  - 's:255:"a:6:{s:15:"itunes:subtitle";s:15:"##PostExcerpt##";s:14:"itunes:summary";s:15:"##PostExcerpt##";s:15:"itunes:keywords";s:17:"##WordPressCats##";s:13:"itunes:author";s:10:"##Global##";s:15:"itunes:explicit";s:7:"Default";s:12:"itunes:block";s:7:"Default";}";'
btc_comment_counts:
  - 'a:0:{}'
btc_comment_summary:
  - 'a:0:{}'
dsq_thread_id:
  - 2185840964
categories:
  - Tech
  - Web 2.0
tags:
  - api
  - google
---
<img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/google_rubrica.png" align="left" height="132" width="166" />Un nuovo rilascio in grande stile da parte di Google per la comunità di sviluppatori che richiedevano a gran voce, e da tempo, la possibilità di **far dialogare** le proprie applicazioni con il DB della &#8220;rubrica&#8221; dei contatti degli utenti. Vi sarà capitato di entrare in qualche Social Network e lasciare le vostre credenziali per far importare automaticamente i vostri contatti, ora con queste API il processo sarà **completamente trasparente**.

E&#8217; interessante vedere come Google sta rilasciando a gran velocità API per far dialogare le applicazioni esistenti con i propri servizi, come **<a href="http://www.stefanomainardi.com/2008/02/01/introduzione-a-google-socialgraph-api/" target="_blank">SocialGraph</a>** o ancora **<a href="http://www.stefanomainardi.com/2007/12/15/introduzione-a-google-chart/" target="_blank">GoogleChart</a>**, o anche tutto il resto del software disponibile con licenze Open Source nel <a href="http://code.google.com/more/" target="_blank">loro repository</a>. Pare che il progetto [OpenSocial][1] si stia **piano piano delineando**, lasciando a Google il ruolo di **Sistema operativo collettore** fra l&#8217;ecosistema di applicazioni online.

<!--more-->

### Quali sono le caratteristiche?

Innanzitutto dobbiamo sottolineare, che la gestione contatti **non è subordinata solamente a Gmail** come è facile pensare, bensì all&#8217;**intero account Google**. Se utilizzate Google Reader difatti avrete notato come negli ultimi aggiornamenti sono apparsi i **feed condivisi dagli &#8220;amici&#8221;**, ovvero le persone con cui ci scambiamo più frequentemente email. Ma questo anche su Calendar e Docs, insomma** tutte le applicazioni di punta di Google**.

**<a href="http://code.google.com/apis/contacts/" target="_blank">Queste API</a>** possono essere utilizzate per la gestione completa dei contatti, ad esempio :

*   Importare la lista contatti nelle proprie applicazioni Web o Desktop
*   Esportare la propria lista contatti sul nostro account Google
*   Creare applicazioni per dispositivi mobili o desktop per la sincronizzazione dei contatti

Una prima applicazione per la **sincronizzazione dei contatti** è stata <a href="http://www.google.com/support/calendar/bin/answer.py?answer=89955" target="_blank">appena rilasciata</a> ufficialmente, ma si limita alla sincronizzazione di Outlook con l&#8217;account Google, di sicuro presto i maggiori programmi **<acronym title="Personal Information Manager">PIM</acronym>** avranno i loro plugin di sincronizzazione.

Attraverso queste API gli sviluppatori possono creare, leggere e aggiornare la lista contatti usando il <a href="http://code.google.com/apis/gdata/overview.html" target="_blank">Google Data Protocol</a> , nella pagina [degli esempi][2] sono mostrati chiaramente casi reali di utilizzo.

Sono stati messi a disposizione una <a href="http://code.google.com/apis/contacts/reference.html" target="_blank">Reference Guide</a> e una [Guida per gli sviluppatori][3], come sempre del materiale di **grandissima qualità**, ed utile per iniziare a fare i **primi esperimenti** con queste nuove API.

Come sempre è stato creato un gruppo su Google Groups per riunire gli sviluppatori e cercare feedback, aiuto e quant&#8217;altro a <a href="http://groups.google.com/group/google-contacts-api" target="_blank">questo indirizzo</a>.

### Conclusioni

Come sempre **sono entusiasta** di questi rilasci da parte di Google, visto che sono un grande utilizzatore dei servizi Google, e credo che questo sia un **rilascio appetibile per molti sviluppatori** che avranno in questo modo vita facile per la gestione contatti esterna al loro servizio.

Per ora le mie uniche perplessità **rimangono sulla gestione di questi contatti**, soprattutto in Gmail, nella mia rubrica ho una marea di contatti **automaticamente inseriti** con cui avrò scambiato al massimo *una o due mail* rendendo quindi caotica la gestione, sarebbe gradita quindi una gestione più efficace o un controllo per evitare questo fastidioso automatismo.

 [1]: http://code.google.com/apis/opensocial/
 [2]: http://code.google.com/apis/gdata/basics.html
 [3]: http://code.google.com/apis/contacts/developers_guide_protocol.html#create_account