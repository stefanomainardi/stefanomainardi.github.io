---
title: Customizzare il widget di Mybloglog
author: Stefano Mainardi
layout: post
permalink: /2007/10/18/customizzare-il-widget-mybloglog/
podPressPostSpecific:
  - 's:245:"a:6:{s:15:"itunes:subtitle";s:15:"##PostExcerpt##";s:14:"itunes:summary";s:15:"##PostExcerpt##";s:15:"itunes:keywords";s:17:"##WordPressCats##";s:13:"itunes:author";s:10:"##Global##";s:15:"itunes:explicit";s:2:"No";s:12:"itunes:block";s:2:"No";}";'
btc_comment_counts:
  - 'a:0:{}'
btc_comment_summary:
  - 'a:0:{}'
categories:
  - Web 2.0
  - Wordpress
tags:
  - css
  - mybloglog
  - web2.0
  - widget
---
<img src="http://farm3.static.flickr.com/2269/1618368428_00fe6d534b.jpg?v=0" align="left" height="62" width="210" /> Probabilmente la maggior parte di voi conoscerà questo servizio, che permette di conoscere in tempo reale **le *facce*** di chi sta visitando il nostro blog e creare quindi piccole community intorno ad esso. Personalmente lo trovo un **ottimo servizio** che mi ha fatto conoscere blog di cui ignoravo l&#8217;esistenza, e con cui ho stretto legami.

Nel post non vorrei dilungarmi sui benefici dell&#8217;utilizzo di tale *utility* bensì spiegare **come adattare** questo widget al vostro template utilizzando i fogli di stile: visto e considerato che lo stile di default **non permette grandi configurazioni** se non giocando con piccole scelte cromatiche.

La mia esigenza è nata in seno alla [**ristrutturazione grafica**][1] fatta intorno al mio blog negli ultimi tempi, e documentandomi [in][2] [giro][3] per la rete ho trovato diverse informazioni utili e non documentate nell&#8217;*helpdesk* di Mybloglog.

<!--more-->

### La struttura

Il widget è basato su tabelle, una scelta forse anacronistica, di seguito un estratto di come il codice è strutturato:

    <table cellspacing='0' cellpadding='0' id='MBL_COMM'>
    <tr><td colspan='2' class='mbl_h'>Recent Readers</td></tr>
    <tr id='tr1'>
    <td id='tdd11' class='mbl_img'><img /></td>
    <td id='tdd21' class='mbl_mem'><a href='#></a></td>
    </tr>
    </table>

Lo schema è molto facile, c&#8217;è una colonna header con il titolo (*seconda riga*), e le successive colonne con due celle rispettivamente per l&#8217;avatar e il link al profilo su Mybloglog. Esiste anche una colonna visibile solo ai non membri con link e riferimento per la registrazione alla Community.

### Le classi CSS

Per modificare l&#8217;aspetto attraverso i fogli di stile queste sono tutte le classi che abbiamo a disposizione:

**body .widget_mybloglog**  
* Questo è il wrapper del widget, utilizzatela per impostarne la larghezza*  
**body table#MBL_COMM**  
* La tabella principale del widget, qui puoi settare di nuovo la larghezza ed il bordo esterno*  
**body table#MBL\_COMM th.mbl\_h**  
* La colonna del titolo, quella che contiene per intenderci il &#8220;Recent Readers&#8221;*  
**body table#MBL\_COMM td.mbl\_img**  
* La cella contenente l&#8217;avatar*  
**body table#MBL\_COMM td.mbl\_mem**  
* La cella contentente il link al profilo Mybloglog*  
**body table#MBL\_COMM td.mbl\_join_img**  
* La cella contenente l&#8217;immagine che appare ai non membri quando visitano la pagina*  
**body table#MBL\_COMM td.mbl\_join**  
* Il testo che appare ai non membri di MyBlogLog*  
**body table#MBL\_COMM td.mbl\_fo_hidden**  
* Le ultime due colonne della tabella contenenti i riferimenti, ovvero: &#8220;View Readers Community&#8221; e &#8220;Provided bu MyBlogLog&#8221;*

Basterà inserire le opportune dichiarazioni all&#8217;interno del vostro foglio di stile per adattarlo come volete al template.

### Come ho modificato il mio widget?

Semplice, ed i passaggi sono brevi.

Sono andato sul mio profilo Mybloglog, ho raggiunto la pagina dei Widget e ho impostato:

*   larghezza di 995 pixel (in base al mio template)
*   Half size per le immagini (immagini piccole)
*   2 Colonne
*   Nessun titolo

<p style="text-align: center">
  <img src="http://www.stefanomainardi.com/wp-content/uploads/Varie/myblog_impostazioni.gif" height="373" width="516" />
</p>

Il mio intento era quello di avere solamente gli avatar, senza nessun testo evitando anche il testo che appare per gli utenti non iscritti al servizio, ed ho risolto agendo in questo modo sul foglio di stile:

    #mybloglog {
    border-bottom:5px solid #FFB03B;
    margin-bottom:0px;
    margin-top:4px;
    padding-bottom:4px;
    text-align:center;
    padding-left:8px;
    }
    
    body table#MBL_COMM {
    background:white repeat-x scroll 0%;
    margin:0pt auto;
    }
    
    body table#MBL_COMM td.mbl_fo_hidden {
    display:none;
    }
    
    body table#MBL_COMM td.mbl_join_img {
    display:none;
    }
    
    body table#MBL_COMM td.mbl_join {
    display:none;
    }
    
    body table#MBL_COMM #tr0 {
    display:none;
    }

Il risultato è quello che vedete lì in alto proprio sull&#8217;header, forse **leggermente invasivo** ma è esattamente quello che avevo intenzione di fare.

Spero che questi piccoli e semplici consigli vi siano utili, buona customizzazione (*che brutta parola*)

 [1]: http://www.stefanomainardi.com/2007/10/07/stiamo-lavorando-per-voi/
 [2]: http://blog.auinteractive.com/style-your-mybloglog-widget
 [3]: http://www.unintentionallyblank.co.uk/2007/03/06/making-mybloglog-pretty-how-to-style-the-recent-readers-widget/