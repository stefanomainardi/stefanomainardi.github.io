---
title: Il mio Mac(Intel) artigianale
author: Stefano Mainardi
layout: post
permalink: /2006/04/10/il-mio-macintel-artigianale/
podPressPostSpecific:
  - 's:245:"a:6:{s:15:"itunes:subtitle";s:15:"##PostExcerpt##";s:14:"itunes:summary";s:15:"##PostExcerpt##";s:15:"itunes:keywords";s:17:"##WordPressCats##";s:13:"itunes:author";s:10:"##Global##";s:15:"itunes:explicit";s:2:"No";s:12:"itunes:block";s:2:"No";}";'
btc_comment_counts:
  - 'a:0:{}'
btc_comment_summary:
  - 'a:0:{}'
dsq_thread_id:
  - 2185796360
categories:
  - All the rest
  - Informatica
---
Sono stato sempre affascinato dalla grande mela, dai suoi prodotti, dalla qualità del design e dalla cura con cui vengono pensati e definiti i dettagli dei loro prodotti, sia software che hardware. Basti pensare all&#8217;Ipod, il gadget high-tech più venduto della storia.

L&#8217;interfaccia del loro sistema operativo è stata sempre il meglio per quanto riguarda l&#8217;usabilità, e l&#8217;invidiabile parco software annovera quanto ci sia di meglio per la grafica professionale, e l&#8217;editing audio/video. Negli anni avere un Mac in alcuni ambiti è diventato uno standard <span style="font-style: italic; font-weight: bold">de facto</span>, basta entrare in qualsiasi studio grafico o studio di registrazione per vedere in bella mostra i Mac, dalle macchine più antiche sino a quelle più recenti. Ovviamente sto parlando di tutti coloro che hanno un <span style="font-weight: bold">budget cospicuo</span> da potersi permettere di acquistare queste <span style="font-style: italic">salatissime</span> (in termini di prezzo) macchine. Per tutti gli altri &#8220;comuni mortali&#8221;, pc assemblati, e il più delle volte con copia pirata di Windows XP Professional (che di Professional, sappiamo bene, non ha proprio nulla se non il nome). A mio parere, <span style="font-weight: bold">prezzi davvero esagerati</span>.  
Di recente la Apple, con una mossa a sopresa (?) ha abbandonato il &#8220;vecchio&#8221; fornitore di Hardware che per anni li ha serviti egregiamente, sto parlando della IBM con i suoi processori (PowerPC G3,G4,G5) di cui Apple andava così fiera e si vantava delle performance al dispetto dei &#8220;lenti&#8221; Pentium della Intel. (<span style="font-style: italic">Chi si ricorda la pubblicità all&#8217;uscita del G4 con un lumaca che trasportava sulle spalle un Pentium?</span>)  
Oggi però per Apple questi processori non sono più ne lenti, ne tantomeno inadatti per il loro sistema operativo. Tant&#8217;è che da un po di tempo tutti i nuovi prodotti di casa Jobs escono fuori con i nuovi processori **Intel Core Duo**, sto parlando dei nuovi **MacbookPRO**, **Imac** e **Macmini**. Sono i primi prodotti che hanno &#8220;subito&#8221; lo switch, nei prossimi mesi tutte le macchine avranno processori Intel.

<div style="text-align: center">
  <img width="400" height="168" border="0" title="indextop20060306.jpg" alt="indextop20060306.jpg" src="http://www.stefanomainardi.com/wp-content/uploads/linux/indextop20060306.jpg" />
</div>

<div align="left" style="text-align: center">
  (<em>Questo lo slogan con cui la Apple ha deciso di lanciare i nuovi prodotti</em>)
</div>

Per alcuni (<span style="font-style: italic">i fanatici</span>) questa mossa di Apple è stata un salto nel vuoto, per me è stata una mossa azzeccata ed i dati finanziari lo dimostrano. Ok, ora le macchine sono dei &#8220;comunissimi&#8221; PC, non si ha più la sensazione di avere una macchina <span style="font-style: italic">diversa, </span>un qualsiasi assemblato può eguagliare le prestazioni di un modello di casa Apple. Sappiamo bene che è possibile acquistare un Processore Intel anche in uno di quei &#8220;agglomerati commerciali&#8221; che vendono un pò di tutto.

Senza fare disquisizioni di sorta sul cambio di architettura, cerco di spiegarvi brevemente come tutto questo sia stato possibile, visto che si è fatto un salto da un&#8217;architettura [PowerPC][1] (in gergo, PPC) ad un&#8217;architettura [X86][2], le quali ovviamente lavorano in modo totalmente diverso. Si è dovuto quindi provvedere a <span style="font-weight: bold">ricompilare </span><em style="font-weight: bold">nativamente</em> sulla nuova architettura il core del sistema operativo, compresi software e driver per le periferiche.

Un vero lavoraccio penserete voi, ma il passo è stato in un certo senso *breve* e poco doloroso.  
Il perchè è semplice da spiegare. Sin dalle [prime versioni][3] di MacOSX, è stato rilasciato il [codice sorgente dell&#8217;intero Sistema operativo][4] sia per <span style="font-weight: bold">PPC</span> che per <span style="font-weight: bold">X86</span>, escludendo di fatto (<span style="font-style: italic">mossa molto abile</span>) l&#8217;interfaccia grafica e le [librerie chiave][5] per riprodurre il look&#038;feel del sistema di casa Apple. Molti si sono chiesti negli anni a che <span style="font-style: italic">pro</span> avere il core del sistema compilato nativamente anche per X86, il tempo ed i fatti hanno spiegato le mosse di Apple, forse sin dall&#8217;inizio si aveva in previsione un cambio di architettura di questo tipo. <span style="font-style: italic">In verità si è sempre vociferato che nei laboratori di Apple ci fosse questa fantomatica versione di MacosX compilata interamente per X86, i cosidetti </span><a title="Macrumors" style="font-style: italic" href="http://www.macrumors.com/">Rumors</a><span style="font-style: italic"> .</span>

Oggi tutto questo è realtà, dall&#8217;annuncio ufficiale sono passati diversi mesi, e le prime macchine X86 sono già in produzione e disponibili presso lo store di Apple. Prima della commercializzazione sono state date in comodato d&#8217;uso agli sviluppatori le cosidette &#8220;<span style="font-weight: bold">Apple Development Platform</span>&#8221; equipaggiate con processore Pentium 4 a 3,6GHz con 2MB di cache L2, 800MHz di front side bus e due moduli di memoria dual channel DDR2 533MHz da 512MB l&#8217;uno. Insomma un normale PC.

La prima versione completamente X86 data in bundle con queste macchine è stata la versione 10.4.1 (<span style="font-style: italic">oggi siamo alla 10.4.6</span>), ovviamente non potevano mancare i primi exploit per installare su qualsiasi PC il tanto famigerato Macosx, eludendo di fatto le <span style="font-style: italic">pallide</span> protezioni (ad esempio il [TPM][6]) e permettere l&#8217;installazione su qualsiasi PC, relativamente simile alla piattaforma di sviluppo mandata agli sviluppatori.

Con il passare del tempo, c&#8217;è stata una *lotta *fra Apple e il noto hacker [Maxxuss][7] , il quale di volta in volta è riuscito a superare egregiamente le nuove protezioni ([ad esempio eludendo il Firmware EFI][8]) e rilasciando patch (scaricabili dal suo sito) per rendere universali le copie di Macosx dato in bundle con un Mac appena acquistato. Intorno a questo &#8220;fenomeno&#8221; sono nate delle [comunità][9] , con un [forum][10] molto attivo ed un [wiki][11] denso di informazioni interessanti.

Allora ho deciso di vedere se realmente quello che si diceva era reale e facilmente fruibile. Visto che un mio caro amico (musicista) era intenzionato a fare un aggiornamento del suo sistema l&#8217;ho indirizzato a comprare un Hardware di qualità e nel contempo compatibile con il mio &#8220;esperimento&#8221;.

Documentandomi sul Wiki ho acquistato una nuova Motherboard:

<img width="400" height="300" border="0" align="bottom" alt="mb_1.JPG" title="mb_1.JPG" src="http://www.stefanomainardi.com/wp-content/uploads/linux/mb_1.JPG" />

Un nuovo Pentium4 Dual-Core:

<img width="400" height="300" border="0" align="bottom" title="cpu_1.JPG" alt="cpu_1.JPG" src="http://www.stefanomainardi.com/wp-content/uploads/linux/cpu_1.JPG" />  
Ed una scheda video ATI X550:

<img width="400" height="300" border="0" align="bottom" alt="mb_video_proc_1.JPG" title="mb_video_proc_1.JPG" src="http://www.stefanomainardi.com/wp-content/uploads/linux/mb_video_proc_1.JPG" />  
Ram (1Gb &#8211; DDR2) e Case li avevo ed abbiamo così ulteriormente risparmiato. Costo di questa operazione **350Euro**.

Ci siamo (legalmente) procurati una versione di Macosx 10.4.5, che abbiamo provveduto a &#8220;patchare&#8221; per testare il nostro sistema. Le operazioni sono state davvero facili, ed al primo boot del DVD &#8220;patched&#8221; ci siamo trovati (con non poco stupore)  
davanti l&#8217;installazione di Macosx, durata poco più di 30 Minuti.

Finita l&#8217;installazione un semplice riavvio ed ecco pronto il nostro Mac &#8220;artigianale&#8221;.

<img width="380" height="156" border="0" align="bottom" alt="macosx86.jpg" title="macosx86.jpg" src="http://www.stefanomainardi.com/wp-content/uploads/linux/macosx86.jpg" />

Le prestazioni sono ottime, paragonabili a quelle di un PowerMacG5 (se non superiori&#8230;), con l&#8217;ottimo tool di benchmarking Xbench abbiamo totalizzato un &#8220;punteggio&#8221; di 120,0. I software che abbiamo provato in nostro possesso con licenza, purtroppo hanno dato scarsi risultati, sto parlando di Software ancora non [Universal Binaries][12] ovvero non ancora compilati per piattaforma X86. Funzionanti quindi in Emulazione trasparente all&#8217;utente, con [Rosetta][13], il &#8220;traduttore&#8221; real-time di istruzioni da PPC a X86. Anche se il software funziona in maniera eccelsa, per applicazioni &#8220;cpu-bound&#8221; (avide di cicli CPU) dimostra tutti i suoi limiti.  
C&#8217;è da dire però, che quasi tutte le software house, stanno rilasciando freneticamente le versioni Universal dei loro software di punta.

Direi che in ambito professionale sarebbe opportuno quindi aspettare ancora qualche mesetto prima di acquistare un nuovo Mac, non avendo così la brutta sorpresa che il software che usate tutti i giorni ancora non sia <span style="font-style: italic">pronto</span> per i <span style="font-weight: bold">nuovi </span>Mac. Basti pensare, per fare un&#8217;esempio, che l&#8217;intera suite Adobe (Illustrator, photoshop, indesign ecc&#8230;) non è ancora Universal Binaries.

Concludendo questo post, davvero troppo lungo, tiro le mie somme e penso che un sistema operativo del genere dovrebbe essere venduto <span style="font-style: italic">unbundle, </span>non legandolo perforza ad un macchina Apple. Ovviamente mi rendo conto che quanto dico è <span style="font-weight: bold">pura fantasia</span>, visto e considerato che Apple fonda il proprio fatturato sulla vendita Hardware (vedi Ipod) ed entrare in un&#8217;ipotetica competizione con Microsoft nella vendita dei sistemi operativi potrebbe decretarne il fallimento in breve termine.

Dal lato puramente informatico devo riconoscere che MacosX è un bel sistema operativo, stabile e visivamente molto gradevole. Devo dire però che non mi è piaciuto per nulla constatare che infondo è un sistema operativo chiuso, implementa il TPM e ne fa massiccio uso nelle Syscall del kernel, e che di &#8220;open&#8221; ha ben poco, ad esempio è impossibile montare o fargli riconoscere un HD con una partizione Linux EXT2/3, cosa che mi ha sconcertato non poco considerando che MacOSX è fondamentalmente uno Unix della famiglia *BSD. Esiste solamente un [progetto esterno][14] che cerca di implementarne il supporto, ma non si assicura il corretto funzionamento. Inutilizzabile quindi in ambiti lavorativi.  
In un mondo dove come non mai l&#8217;interoperabilità e lo scambio libero di informazioni è una cosa fondamentale, fare certe scelte mi sembra anacronistico e privo di utilità, atte solamente a rafforzare e chiudere un mercato creando quindi dei monopoli dominanti nell&#8217;industria software di cui Microsoft già ne fa da padrona ed ha fatto scuola.  
La vera concorrenza di oggi è la **libertà**, GNU/Linux ne è un&#8217;ottimo esempio e sono sempre più convinto che sia questa la strada da seguire.

E&#8217; stato solamente un&#8217;esperimento divertente, preferisco però essere padrone e cosciente in quello che faccio, e non avere un *grande marca* che influenzi il mio modo di essere &#8220;libero&#8221; e di pensare anche se si tratta di usare &#8220;solamente&#8221; un Personal Computer.

> <span style="font-weight: bold">Think Freedom</span> (per fare il verso alla Apple) è il mio motto.

 [1]: http://it.wikipedia.org/wiki/PowerPC "PowerPC"
 [2]: http://it.wikipedia.org/wiki/X86 "X86"
 [3]: http://www.opensource.apple.com/darwinsource/images/release-notes-1.4.1.txt "Macosx 10.0 Release Notes"
 [4]: http://developer.apple.com/opensource/ "Darwin"
 [5]: http://developer.apple.com/documentation/Cocoa/Conceptual/CarbonCocoaDoc/Articles/CarbonCocoaComm.html "Carbon_Cocoa"
 [6]: http://it.wikipedia.org/wiki/Trusted_Computing_Platform_Alliance "tpm"
 [7]: http://www.maxxuss.org "Maxxuss Homepage"
 [8]: http://punto-informatico.it/p.asp?i=57909&#038;r=PI "10.4.4 Cracked"
 [9]: http://www.osx86project.org "Osx86 Homepage"
 [10]: http://forum.osx86project.org "Forum OSX86"
 [11]: http://wiki.osx86project.org
 [12]: http://www.apple.com/universal/ "Universal Binaries"
 [13]: http://www.apple.com/rosetta/ "Rosetta"
 [14]: http://sourceforge.net/projects/ext2fsx/ "Ext2fsx"