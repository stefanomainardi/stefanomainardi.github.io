---
title: Drupal 8, cosa ci sarà da aspettarsi
author: Stefano Mainardi
layout: post
permalink: /2014/01/13/drupal-8-cosa-ci-sara-da-aspettarsi/
dsq_thread_id:
  - 2186057743
categories:
  - Tech
---
[<img class="size-full wp-image-567 aligncenter" alt="Drupal8Tablet" src="http://www.stefanomainardi.com/wp-content/uploads/2014/01/Drupal8Tablet.jpg" width="620" height="412" />][1]

<p style="text-align: center;">
  <small>(Foto di <a href="http://drupal.org" target="_blank">Drupal.org</a>)</small>
</p>

<p class="lead drop-cap">
  Per chi lavora nel settore, ma sopratutto chi usa questo strumento, sta aspettando con ansia il rilascio della <a href="https://drupal.org/drupal-8.0" target="_blank">nuova versione di Drupal</a>, che a tutti gli effetti sarà una vera rivoluzione sotto molti aspetti.
</p>

Negli anni mi è capitato molte volte di imbattermi con colleghi che hanno sempre denigrato e visto con sospetto Drupal, a volte a ragione, molte volte a torto. L&#8217;evoluzione è un processo complicato, sopratutto quando da micro sistemi si diventa &#8220;macro&#8221;, quando le decisioni devono passare attraverso molti canali prima di essere prese, quando tecnicamente la codebase diventa onerosa e quando si decide negli anni di avere una retro-compatibilità.  
Allo stato attuale Drupal è uno strumento molto potente, ma soffre di lacune lato architetturale tanto da rendere molto difficile avere delle strette best-practices di sviluppo, ad esempio il TDD. In Twinbit siamo riusciti ad avere un workflow completo che ci riesce a garantire affidabilità e testing, ma in molte occasioni ci siamo dovuti piegare allo strumento piuttosto che piegare lo strumento alle nostre esigenze.

<!--more-->Con il nuovo rilascio previsto per la fine del 2014, le cose cambieranno in meglio, o almeno si spera. Molto del codice core legacy è diventato Object Oriented, molte funzioni custom sono state sostituite con componenti di terze parti, vedi l&#8217;introduzione di 

<a href="http://symfony.com/blog/symfony2-meets-drupal-8" target="_blank">Symfony</a>, <a href="http://twig.sensiolabs.org/" target="_blank">Twig</a> per il templating, <a href="http://backbonejs.org/" target="_blank">Backbone</a> e <a href="http://underscorejs.org/" target="_blank">Undercore.js</a> per il frontend, e per finire l&#8217;integrazione di <a href="http://phpunit.de/" target="_blank">PHPUnit</a>. Molti i miglioramenti anche per i site builder, ad esempio l&#8217;introduzione di temi responsive per il backend, e l&#8217;integrazione nativa di un editor WYSIWYG. Direi che finalmente abbiamo iniziato a giocare sul serio in diversi ambiti, portando lo strumento ad un nuovo livello.

Mi piacerebbe, senza entrare troppo nel dettaglio, fare una carrellata di quelle che ritengo le migliorie degne di nota, determinati per iniziare a progettare gli upgrade dei nostri applicativi, o di proporre nuove soluzioni ai nostri clienti.

## Accessibilità

Uno dei punti cruciali su cui si è dibattuto negli anni per quanto riguarda Drupal, è la ripida curva di apprendimento per gli editors e il backend non propriamente user friendly se confrontato con altri CMS Open Source, uno su tutti WordPress.

Per questo una delle iniziative prima della partenza dello sviluppo di questa nuova release, era quella di migliorare sensibilmente l&#8217;esperienza d&#8217;uso, fornire nuovi strumenti più accessibili, ed essere finalmente compatibile con dispositivi mobile.

L&#8217;inziativa che ne è nata è stata chiamata &#8220;[Spark][2]&#8220;, coordinata e sponsorizzata da Acquia, azienda a cui fa capo il fondatore di Drupal

Dai test che ho effettuato, direi che il risultato è ottimo e praticamente raggiunto, l&#8217;esperienza backend inizia a livellarsi finalmente verso standard alti di usabilità, mettendo delle solide fondazioni per il futuro.

Le caratteristiche promesse inizialmente e ad oggi attive sono:

*   Toolbar di amministrazione responsive
*   Editor WYSWYG integrato nel core, con integrazione nativa ai formati del testo. *Finalmente dopo anni, anche Drupal si fornisce di uno strumento indispensabile senza dover ricorrere a integrazioni esterne*
*   <span style="line-height: 1.5em;">In-Place content editing. </span><em style="line-height: 1.5em;">Questa funzionalità è in realtà molto controversa, direi che è utile in pochi casi, sicuramente aiuta l&#8217;esperienza utente dell&#8217;editor nel momento in cui le modifiche da fare ai contenuti siano di piccola entità </em>

[<img class="size-full wp-image-608 aligncenter" alt="in_place_editing" src="http://www.stefanomainardi.com/wp-content/uploads/2014/01/in_place_editing.png" width="772" height="317" />][3]

<p style="text-align: center;">
  <span class="label">Drupal 8 In place content editing. Da frontend sarà possibile editare gli elementi presenti all&#8217;interno del contenuto </span>
</p>

*   [Mobile preview tool][4]. *Un tool che permette attraverso una serie di configurazioni predefinite, ed altre configurabili, di testare in modalità preview il contenuto su diverse risoluzioni*

[<img class="size-full wp-image-605 aligncenter" alt="Drupal 8 - Mobile preview tool" src="http://www.stefanomainardi.com/wp-content/uploads/2014/01/Drupal-8-Mobile-preview-tool.png" width="747" height="849" />][5]

<p style="text-align: center;">
   <span class="label">Mobile preview tool</span>
</p>

*   [A responsive page layout editor][6]. *Un tool integrato con [Panels][7] per la generazione di layout responsive. Personalmente non sono un fanatico di Panels, ma a ad un primo test mi sembra un ottimo strumento per i site builders*
*   Un nuovo tema di amministrazione responsive [Ember][8]
*   Possibilità finalmente di avere delle &#8220;preview&#8221; reali dei contenuti
*   Eliminazione degli orribili &#8220;overlay&#8221; di amministrazione introdotti in Drupal 7
*   Integrazione in core di alcune utili funzionalità, ad esempio il [module filtering ][9]

Moltissime sono le novità, oltre le più rilevanti che ho indicato. Vi consiglio di seguire direttamente le [iniziative collegate][10] e se ne avete le capacità e la voglia di contribuire per migliorare il progetto o portare nuove idee, la community Drupal è piuttosto accogliente e ricettiva

## Site builders

Anche per i site builders le novità sono diverse ed interessanti. Devo dire che su questo fronte Drupal è stato sempre un gradino più in alto rispetto ad altri CMS, tante volte anche a soluzioni più blasonate o soluzioni commerciali closed.

L&#8217;estrema flessibilità è stata da sempre una caratteristica che ho apprezzato, nonostante quest&#8217;ultima ha sempre un grande prezzo da pagare in favore della curva di apprendimento per chi si accinge le prime volte a lavorare con questo strumento.

Le novità che ritengo più interessanti sono le seguenti.

*   **Nuovi &#8220;Field types&#8221;**. La modellazione dei nostri dati, quindi in gergo Drupal, dei nostri Content Type si arricchisce ulteriormente portando nel core nuovi oggetti senza dover più ricorrere a moduli esterni, ad esempio i nuovi fields: Data, Entity Reference, Link, Phone, Email. Un enorme passo avanti, rendendo sempre più ampio e configurabile lo strumento alla prima installazione. Ottimo lavoro!
*   **Nuovi &#8220;Entity Types&#8221;**. Se sui sistemi Unix tutto è un file, su Drupal tutto è un nodo, o meglio una Entity. Finalmente anche i blocchi potranno essere &#8220;fieldable&#8221;, ovvero avremo la possibilità di aggiungere &#8220;fields&#8221; ai blocchi, rendendoli adatti alle nostre esigenze senza dover essere limitati dal titolo e un body. Anche la &#8220;contact form&#8221; di default eredita questa possibilità.
*   **Possibilità di customizzare da backend la visualizzazione delle form**. Per intenderci, ad esempio potrò configurarmi il numero di rows da mostrare nella textarea della form commenti

[<img class="alignnone size-full wp-image-581" alt="Screen Shot 2014-01-12 at 18.40.44 pm" src="http://www.stefanomainardi.com/wp-content/uploads/2014/01/Screen-Shot-2014-01-12-at-18.40.44-pm.png" width="794" height="466" />][11]

<p style="text-align: center;">
  <span class="label">Possibilità di customizzare da backend le caratteristiche delle form</span>
</p>

*   **Views in core**. Views è lo strumento per eccellenza che alza l&#8217;asticella di Drupal rispetto la concorrenza, per chi non lo conoscesse è un visual query builder che ci permette quindi di interrogare il DB attraverso un interfaccia ad-hoc, da query molto semplici fino a query molto complesse che possono coinvolgere più *particelle* del sistema. Ad esempio possiamo generare feed, o fornire *output REST *senza dover scrivere nessuna linea di codice.  
    Si tratta di uno di quei moduli che viene installato di default, averlo nel core ci farà risparmiare tempo e offrirà uno strumento nativo per l&#8217;estrazione dei contenuti

Anche qui le novità sono moltissime e quelle indicate sono solamente un subset delle più interessanti, anche qui vi invito a partecipare ad uno dei progetti attualmente aperti

## Gestione multilingua

La gestione multilingua su Drupal è stata sempre un po&#8217; croce e delizia. Su Drupal 7 gli strumenti a disposizione sono moltissimi, e anche molto  avanzati e completi. In Twinbit abbiamo sviluppato un ottimo know-how nella gestione e nella creazione di siti multilingua complessi, ad esempio [Antinori][12], e [Tim International][13], abbiamo avuto modo quindi di testarne in modo molto approfondito gli aspetti positivi e negativi, e migliorando in molti casi ai moduli stessi inviando patch o nuove funzionalità. Posso affermare con certezza che Drupal è uno dei CMS open source più avanzati riguardo la gestione del multilingua.

I punti dolenti della gestione multilingua è trovarsi di fronte a situazioni in cui alcune parti del core hanno bisogno di *workaround *per essere tradotti correttamente, ad esempio i blocchi di sistema, o molte volte moduli contrib. Se è vero che ad ogni problema si può ricorrere ad una soluzione fatta in-house, o attraverso moduli contrib, molte volte la situazione è frustrante. L&#8217;altro grande problema storico è l&#8217;impossibilità attualmente di rimuovere la lingua base Inglese, anche qui costringendo il site builder a ricorrere a soluzioni poco ortodosse per impostare una lingua base diversa dall&#8217;inglese. A livello di usabilità ci sono diversi moduli contrib che possono aiutare l&#8217;editor ad orientarsi, ma sicuramente il lavoro da fare di razionalizzazione è molto alto e da un sistema così avanzato ci si aspetterebbe un interfaccia di sistema che esponga le potenzialità espresse dal sistema.

Tutte queste problematiche sono state** identificate e raccolte** nell&#8217;iniziativa [Drupal 8 Multilangual][14], dai miei test attuali il livello raggiunto** è davvero stupefacente**, ogni pezzo del sistema è traducibile ed esportabile. Inutile che vi scriva quali sono le novità, mi limito a linkarvi la [documentazione scritta][15] dal coordinatore dell&#8217;iniziativa multilngua per rendervi conto della mole di lavoro che c&#8217;è stata dietro.

**Sono davvero entusiasta**, e il mio spirito nerd non vede l&#8217;ora di poter lavorare ad un progetto multilingua con D8.

## Designers & Themers

Drupal oggi offre infinite possibilità per i themers, anche se attualmente il core soffre di alcune lacune che possono essere colmate attraverso moduli contrib. Ad esempio D7 non offre supporto nativo ad elementi HTML5, oppure fornisce di default una versione vecchia di Jquery. Lacune colmabili in [pochissimo][16] [tempo][17], ma sono cose che non ci si aspetterebbe da un software in linea con i tempi.

Allo scorso DrupalDay, [Andrea][18] il nostro Senior Frontend developer in Twinbit ha tenuto un [interessante sessione][19] per fare fotografia di quale sia lo stato dei &#8220;base theme&#8221; Drupal, confrontando pregi e difetti delle varie soluzioni e portando il suo punto di vista sullo sviluppo frontend con Drupal, visto che si è trovato molte volte a dover integrare design molti spinti su Drupal spingendolo quasi al limite delle sue potenzialità, vi consiglio di perdere qualche minuto per ascoltare la sessione.

Anche in questo campo Drupal 8 porterà una ventata di freschezza. Avremo finalmente disponibili gli elementi HTML5 di default, ad esempio su tutte le form di sistema e non, e nuove librerie di frontend: [Backbone.js][20], [Modernizr][21], [Twig][22] come template engine, [Normalize.css][23] come alternativa ai classici css reset. Insomma ora anche i frontend developer avranno un sistema all&#8217;altezza delle lore aspettative.

Probabilmente uno degli aspetti più interessanti, ma più impegnativi, sarà il passaggio a Twig. Chi lavora con Symfony lo conosce molto bene, per Drupal è un assoluta novità. Oggi la separazione tra presentazione e business logic è molto a discrezione delle capacità dello sviluppatore, con Twig scrivere codice più *consono* e meno *spaghetti-code *sarà nettamente più semplice.

Un piccolo esempio di come sarà strutturato il classico template del nodo per mostrarvene la leggibilità che è praticamente autoesplicativa se confrontata con i *vecchi modelli. Il codice mostrato è il template &#8220;node&#8221; del tema Bartik fornito con Drupal 8:*

<pre class="font-size:14 lang:default decode:true">&lt;article id="node-{{ node.id }}" class="{{ attributes.class }} clearfix"{{ attributes }}&gt;

  {{ title_prefix }}
    &lt;h2{{ title_attributes }}&gt;
      &lt;a href="{{ node_url }}" rel="bookmark"&gt;{{ label }}&lt;/a&gt;
    &lt;/h2&gt;
  {{ title_suffix }}

  {% if display_submitted %}
    &lt;footer&gt;
      {{ user_picture }}
      &lt;p class="submitted"&gt;{{ submitted }}&lt;/p&gt;
    &lt;/footer&gt;
  {% endif %}

  &lt;div{{ content_attributes }}&gt;
    {# We hide links now so that we can render them later. #}
    {{ content }}
  &lt;/div&gt;

  {{ content.links }}

&lt;/article&gt;</pre>

Chi si è trovato a lavorare con template Drupal, sono certo che migliorerà profondamente il workflow lavorativo.  
Dedicherò un post ad-hoc su Twig nei prossimi giorni per mostrarvene le potenzialità, credo ne valga assolutamente la pena.

Altro punto interessante è l&#8217;abbandono del supporto completo per IE 6/7, e gran parte anche per l&#8217;ultimo baluardo da sconfiggere per i web developer il vetusto IE8. Sarà un motivo in più per convincere i clienti ad abbandonare nei loro piani il supporto a tale pezzo d&#8217;antiquariato.

## Developers

Qui davvero c&#8217;è moltissimo di cui parlare, le novità introdotte sono moltissime ed interessanti e di sicuro avrò modo di parlarne in maniera più approfondita e con esempi d&#8217;uso nei prossimi post dedicati a Drupal, ma voglio riportare alcuni degli aspetti salienti.

Le novità più interessanti sono sicuramente il [Configuration management][24] per *spostare e sincronizzare *le configurazioni da un ambiente all&#8217;altro, pensate al problema di dover gestire più ambienti di sviluppo, o dover gestire il deploy da un ambiente di staging ad un ambiente di produzione. Ad oggi l&#8217;unica soluzione era quella di utilizzare l&#8217;ottimo modulo [Features][25] per portare su file system tutto quello che risiede su DB, ma non tutte la configurazioni di sistema erano esportabili, anche qui costringendo lo sviluppatore a workaround per poter tener sincronizzati gli ambienti senza dover toccare il DB. Un enorme passo avanti che pochi CMS open e commerciali possono vantare.

L&#8217;integrazione nativa con [Drush][26], il tool da CLI per automatizzare e velocizzare tutte le attività di sviluppo e di manutenzione del sistema. Nato inizialmente come utility di gestione, divenuto nel tempo uno strumento fondamentale per chi sviluppa codice.

Un altro aspetto molto interessante di Drupal 8 sarà l&#8217;aspetto Web Services. L&#8217;iniziativa recita &#8220;***The Web Services and Context Core Initiative (WSCCI) aims to transform Drupal from a first-class CMS to a first-class REST server with a first-class CMS on top of it**&#8220;. *Da un sistema moderno ci si aspetta che che l&#8217;HTML è solamente uno dei possibili output che il sistema debba restituire, è ora questo succederà nativamente, senza dover ricorrere a moduli contrib esterni, ad esempio [Services][27]. Ad esempio è uon scenario davvero molto interessante nel caso decidessimo di utilizzare Drupal come backend per applicazioni mobile, [vi linko una sessione][28] che abbiamo tenuto io e [Paolo][29] allo scorso Phpday in cui abbiamo parlato dell&#8217;argomento.

Sulle componenti Symfony e del testing ci torneremo invece con post di dettaglio corredati di esempi.

<span style="font-size: 1.5em; line-height: 1.5em;">Conclusioni finali</span>

Le aspettative sono molte, e sono certo che poche saranno tradite. Direi che questo è il salto più radicale da una major release all&#8217;altra che Drupal abbia mai fatto, trasformando molto del codice vecchio e legacy in codice first-class, portandolo in linea con quelle che sono le tecnologie moderne e le best practice di sviluppo.

Si esce finalmente dalla cosiddetta sindrome del **[Not invented here][30]** per passare ad un più sano e corretto &#8220;**Proudly Found Elsewhere**&#8220;. Personalmente ho apprezzato molto l&#8217;apertura verso progetti esterni e l&#8217;apertura alla contaminazione di mondi diversi e con altre regole rispetto a quelli a cui si è abituati. Questo approccio sta migliorando la sensibilità della community di sviluppatori, e la qualità del prodotto, non solo di Drupal ma anche dei progetti che sono stati abbracciati. La vera espressione del modello Open Source.

Proprio oggi mi è stato chiesto un parere sulla comunità Drupal, in generale sul progetto. Ci ho riflettuto un attimo e poi senza pensarci troppo mi è venuto da dire che **è uno degli esempi migliori di progetto Open Source**, direi paragonabile al kernel Linux in termini di governance e qualità.  Per chi mi ha chiesto come mai utilizzo WordPress e non Drupal su questo blog, risponderò anche a questo quesito :-)

 [1]: http://www.stefanomainardi.com/wp-content/uploads/2014/01/Drupal8Tablet.jpg
 [2]: https://drupal.org/project/spark
 [3]: http://www.stefanomainardi.com/wp-content/uploads/2014/01/in_place_editing.png
 [4]: https://drupal.org/project/responsive_preview
 [5]: http://www.stefanomainardi.com/wp-content/uploads/2014/01/Drupal-8-Mobile-preview-tool.png
 [6]: http://drupal.org/project/layout
 [7]: https://drupal.org/project/panels
 [8]: https://drupal.org/project/ember
 [9]: https://drupal.org/project/module_filter
 [10]: https://drupal.org/node/2107085
 [11]: http://www.stefanomainardi.com/wp-content/uploads/2014/01/Screen-Shot-2014-01-12-at-18.40.44-pm.png
 [12]: http://bit.ly/LPCe4Y
 [13]: http://bit.ly/1ahIXwp
 [14]: http://www.drupal8multilingual.org/
 [15]: http://hojtsy.hu/multilingual-drupal8
 [16]: https://drupal.org/project/html5_tools
 [17]: https://drupal.org/project/jquery_update
 [18]: http://twitter.com/andypanix
 [19]: http://bit.ly/1cStztz
 [20]: http://backbonejs.org/
 [21]: http://modernizr.com/
 [22]: http://twig.sensiolabs.org/
 [23]: http://necolas.github.io/normalize.css/
 [24]: https://drupal.org/documentation/administer/config
 [25]: https://drupal.org/project/features
 [26]: https://github.com/drush-ops/drush
 [27]: https://drupal.org/project/services
 [28]: http://vimeo.com/56972126
 [29]: http://www.paolomainardi.com
 [30]: http://en.wikipedia.org/wiki/Not_invented_here
