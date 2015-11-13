---
title: Introduzione a Google Chart API
author: Stefano Mainardi
layout: post
permalink: /2007/12/15/introduzione-a-google-chart/
podPressPostSpecific:
  - 's:255:"a:6:{s:15:"itunes:subtitle";s:15:"##PostExcerpt##";s:14:"itunes:summary";s:15:"##PostExcerpt##";s:15:"itunes:keywords";s:17:"##WordPressCats##";s:13:"itunes:author";s:10:"##Global##";s:15:"itunes:explicit";s:7:"Default";s:12:"itunes:block";s:7:"Default";}";'
btc_comment_counts:
  - 'a:0:{}'
btc_comment_summary:
  - 'a:0:{}'
dsq_thread_id:
  - 2446263597
categories:
  - Web 2.0
tags:
  - google
  - programmazione
  - web2.0
---
<img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/google_rubrica.png" align="left" />*BigG* nel 2007 ci ha *regalato* **una valanga di servizi**, comprese una serie di acquisizioni strategiche, facendolo diventare a buon titolo il futuro &#8220;***Sistema Operativo***&#8221; della rete. Potrebbe sembrare una definizione **un po azzardata** ma se ci pensiamo allo stato attuale ci permette di svolgere una quantità di task consueti **senza il bisogno di avere applicazioni installate**, pensiamo ad esempio a Docs che ultimamente ha introdotto anche il software per creare e gestire presentazioni, oppure l&#8217;imminente [storage online][1] che ci permetterà di accedere ad uno** spazio remoto e sincronizzare i nostri files in tempo reale**, forse il mito dei computer &#8220;thin&#8221; senza hd presto potrebbe essere di nuovo un argomento cool.

Ricordo che se ne parlava gia moltissimi anni fa, quando si *filosofeggiava* su una rete fatta di un aggregazione di piccoli computer con ridotte capacità (a basso costo) in grado di reperire funzionalità e servizi completamente in rete interagendo con server remoti di grandissime potenzialità (Google?). **Privacy permettendo** e DigitalDivide in Italia, l&#8217;argomento è ancora molto interessante.

Tornando a noi, proprio in questi giorni Google ha rilasciato un&#8217;<acronym>API</acronym> per sviluppatori per generare grafici &#8220;on-the-fly&#8221; semplicemente partendo [da un URL][2] del vostro browser.

<!--more-->

### Come usare Google Chart API

Il funzionamento è molto semplice ed intuitivo. Le API restituiscono un immagine in formato PNG a seguito ad una richiesta via URL. Possono essere generati diversi tipi di grafici: a [linee][3], [barre][4], a [torta][5] ed [altro ancora][6]. Per ogni immagine possono essere specificati attributi come la dimensione, il colore e le etichette di testo.

E&#8217; possibile includere in una pagina web un grafico semplicemente racchiudendo l&#8217;url in un tag `<img>`. L&#8217;immagine verrà renderizzata in tempo reale alla visualizzazione della pagina web. **Tutto molto semplice ed efficace**.

Ad esempio se io volessi inserire un grafico, in questo post dovrei semplicemente inserire queste poche linee di codice :

    <img src="http://chart.apis.google.com/chart?
    cht=p3&chd=s:hW&chs=500x200&chl=Stefano|Mainardi">

Ed avrei in *risposta* la seguente immagine generata dinamicamente

<p style="text-align: center">
  <img src="http://chart.apis.google.com/chart?cht=p3&chd=s:hW&chs=500x200&chl=Stefano%7CMainardi" />
</p>

Attraverso il browser possiamo vedere in che modo queste immagini vengono generate, andando a vedere l&#8217;URL della stessa. Provate ad esempio con firefox andando sul menù contestuale &#8220;**Visualizza Immagine**&#8221; per vederne le proprietà.

Lo schema di default con cui lavorano queste API è il seguente :

<pre class="long"><code>http://chart.apis.google.com/chart?&lt;parameter 1&gt;&&lt;parameter 2&gt;</code><code>&&lt;parameter n&gt;</code></pre>

Analizziamo un po il codice demo per capire come quel grafico è stato generato:

*   `cht=p3`  
    Qui viene selezionato il tipo di grafico in questo caso a torta
*   `chd=t:90,49`  
    I valori assegnati per creare il grafico
*   `chs=500x200`  
    Le dimensioni del grafico
*   `chl=Stefano|Mainardi`  
    Le etichette applicate al grafico

Nella [guida per sviluppatori][7] troverete comunque una serie di esempi molto esplicativi all&#8217;uso di questo API e sulle loro funzionalità.

### Possibili scenari di utilizzo

E&#8217; vero che esistono una marea di script in PHP per creare grafici via [GD][8], e di sicuro per progetti grandi sono la scelta obbligata e più sicura, visto e considerato che non è garantita nel tempo la vita di queste API, è gia successo [altre volte][9] che alcune librerie venissero dismesse senza avvertimento e lasciando a piedi chi aveva creato applicazioni ad esse collegate. Va considerata anche la limitazione di **50.000 query** giornaliere, e l&#8217;assenza di una **modalità pro** per avere accesso illimitato, che vanno quindi ad escluderlo per utilizzi in ambiti professionali.

Però di sicuro può essere utile per applicazioni web intranet che non sviluppano molto traffico, oppure per creare facilmente grafici da inserire in blog, portali e presentazioni. Ad esempio sarebbe possibile creare **grafici parametrici aggiornati in tempo reale** in una presentazione, attraverso l&#8217;[utilizzo di Javascript][10].

Un applicazione su tutte in cui si possono vedere le potenzialità di questo strumento è [Google Finance][11] , credo basti per dimostrarne le potenzialità.

### Conclusioni

Mi piace il modo con cui Google **restituisce alla comunità** software sviluppato internamente, lasciando **spazio di creatività** agli ingegneri di lavorare a progetti in totale libertà, quel famoso &#8220;[20-percent-of-time][12]&#8221; sembra funzionare.

E&#8217; stato creato un **[gruppo di discussione][13]** ufficiale per gli sviluppatori e gli utilizzatori, dove ho trovato un [generatore di grafici][14] automatizzato, è impressionante vedere a che **velocità** si muove la comunità intorno ai servizi di Google e i mashup ad essa collegati.

 [1]: http://www.tomshw.it/news.php?newsid=12141
 [2]: http://chart.apis.google.com/chart?cht=p3&chd=t:90,49&chs=350x150&chl=Stefano%7CMainardi
 [3]: http://code.google.com/apis/chart/#line_charts
 [4]: http://code.google.com/apis/chart/#bar_charts
 [5]: http://code.google.com/apis/chart/#pie_charts
 [6]: http://code.google.com/apis/chart/#chart_type
 [7]: http://code.google.com/apis/chart/
 [8]: http://it2.php.net/gd
 [9]: http://code.google.com/apis/soapsearch/
 [10]: http://code.google.com/apis/chart/#encoding_data
 [11]: http://finance.google.com/finance
 [12]: http://www.google.com/support/jobs/bin/static.py?page=about.html&about=eng
 [13]: http://groups.google.com/group/google-chart-api
 [14]: http://www.style.org/chartapi/