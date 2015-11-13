---
title: Introduzione a Google SocialGraph API
author: Stefano Mainardi
layout: post
permalink: /2008/02/01/introduzione-a-google-socialgraph-api/
podPressPostSpecific:
  - 's:245:"a:6:{s:15:"itunes:subtitle";s:15:"##PostExcerpt##";s:14:"itunes:summary";s:15:"##PostExcerpt##";s:15:"itunes:keywords";s:17:"##WordPressCats##";s:13:"itunes:author";s:10:"##Global##";s:15:"itunes:explicit";s:2:"No";s:12:"itunes:block";s:2:"No";}";'
btc_comment_counts:
  - 'a:0:{}'
btc_comment_summary:
  - 'a:0:{}'
dsq_thread_id:
  - 2185840067
categories:
  - Tech
  - Web 2.0
tags:
  - api
  - google
  - programmazione
  - sviluppo
---
<img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/google_rubrica.png" align="left" height="132" width="166" />Google ha appena [rilasciato][1] un interessantissima API dedicata al mondo dei Social Network, non si tratta di un ennesimo Facebook o *<strike>vaccate</strike>* servizi simili &#8220;2.0&#8221;, bensì di un software in grado di ricostruire la nostra rete di contatti utilizzando *semplicemente* il crawler di Google, software molto utile per gli sviluppatori di Social Network per non far ricostruire ogni volta la propria rete di contatti all&#8217;utente.

Pare che la mossa di oggi di <a href="http://mashable.com/2008/02/01/microsoft-wants-to-acquire-yahoo-for-446-billion/" target="_blank">Microsoft e Yahoo</a> non abbia fatto paura a Google, tanto da rilasciare in giornata un&#8217;altra API che va a riempire **il sacco pieno di servizi** interessanti di *BigG, *e che molto probabilmente andrà ad arricchire il consorzio <a href="http://dataportability.org/" target="_blank">Dataportability</a> per la creazione di un **tool omogeneo** di servizi a *formato aperto* per la gestione delle informazioni in rete.

<!--more-->

### Come Funziona?

Lo sviluppatore Brad Fitzpatrick in questo video spiega in maniera molto semplice il funzionamento.  
<center>
  <br /> <br />
</center>

  
In sostanza il crawler di Google scandaglia i **dati pubblici** degli attuali Social Network pubblicati sotto forma di <acronym title="XHTML Friends Network"><strong>XFN</strong></acronym> o <acronym title="Friend of a friend"><strong>FOAF</strong></acronym> e dopodichè restituisce le relazioni esistenti attraverso l&#8217;API stessa.

Le relazioni potrebbero essere di questo tipo:

*   &#8220;Stefano è un twitter-friend di Giovanni&#8221;
*   &#8220;Stefano ha Giovanni nel suo Blogroll&#8221;

Anche in WordPress i dati del blogroll vengono pubblicati sotto forma di [XFN][2], credo che in pochi abbiano avuto la pazienza di riempire ogni volta tutti i campi, ma sono dati fondamentali affinchè queste applicazioni possano esistere. Infondo **il vero Social Network è la rete stessa**, ed i blog nella loro semplicità lo hanno dimostrato.

<p style="text-align: center">
  <img src="http://code.google.com/apis/socialgraph/images/the-web.png" height="389" width="375" />
</p>

Il software potrebbe tornare molto utile a livello di interfaccia utente, facciamo un esempio.

Ora con i Social Network attuali abbiamo, *più o meno*, questo approccio :

*   Registrazione
*   Profilazione utente
*   Ricerca contatti/amici
*   Import dei dati della nostra casella di posta per trovare conoscenti già registrati/presenti (**problema di privacy?**)

Ovviamente il tutto **risulta macchinoso**, anche se le attuali interfacce utente tentano *di nascondere il più possibile*, e potrebbe scoraggiare l&#8217;utilizzo di servizio.

Attraverso l&#8217;utilizzo di questa API, *o altre di questo tipo,* l&#8217;approccio ne risulterebbe** molto più snello ed efficace** :

*   Registrazione
*   Profilazione utente
*   **Ricerca automatica di relazioni** nella rete e popolamento automatico della nostra lista amici

L&#8217;ultimo punto potrebbe essere completamente **trasparente all&#8217;utente**, e non dovrebbe interagire con **nessun servizio di terze parti**, utilizzando quindi quello che la rete mette gia a disposizione.

Per comprenderne meglio il funzionamento sono state rilasciate delle <a href="http://code.google.com/apis/socialgraph/docs/examples.html" target="_blank">applicazioni esemplificative</a>, e vi **invito a provarle** voi stessi per capire al meglio di cosa stiamo parlando.

### Conclusioni

E&#8217; interessante vedere come in questo periodo i più grandi player del settore **stanno promuovendo standard aperti**, ad esempio l&#8217;adozione di [OpenID in Yahoo!][3] , e l&#8217;interesse creatosi attorno al progetto Dataportability. Si sente quindi l&#8217;esigenza di trovare **soluzioni univoche e aperte** per la gestione delle identità in rete e dei flussi di informazioni create dagli utenti.

Sembra che i primi passi verso un **approccio <a href="http://it.wikipedia.org/wiki/Web_3.0#La_realizzazione_del_Web_semantico_e_del_SOA" target="_blank">semantico</a> alla rete** stiano iniziando, ***un progetto sicuramente da seguire***.

 [1]: http://google-code-updates.blogspot.com/2008/02/urls-are-people-too.html
 [2]: http://gmpg.org/xfn/
 [3]: http://openid.yahoo.com/