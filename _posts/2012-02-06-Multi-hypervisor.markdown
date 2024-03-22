---
layout: post
title:  Multi-hypervisor 
date:   2012-02-06 
categories:  tech italiano 
---

# Multi-hypervisor


Siccome non mi riesce di commentare sul [sito originale](http://vinfrastructure.it/2012/02/virtualization-ecosystem-is-becoming-multi-hypervisor/), riporto qui un post interessante con i miei commenti.

> Uno dei trend visti nell’ultimo anno (ma in realtà iniziato qualche anno fa) è la crescita dell’ecosistema legato alla virtualizzazione (ossia tutti quei prodotti e vendor complementari ai prodotti di virtualizzazione veri e propri) al di fuori dei confini nei quali sono storiacamente nati: molti dei partner storici di VMware ora hanno esteso le loro soluzioni anche ad altri hypervisor, e nuovi prodotti sono nati specifici per gestire ambienti virtuali complessi o quanto meno eterogeni. Una bella definizione a questo fenomeno è stata data da VKernel nel suo post: “[Hypervisor Agnosticism](http://vinfrastructure.it/2012/02/virtualization-ecosystem-is-becoming-multi-hypervisor/reader/items/hypervisor-agnosticism)“.
> 
> Bisogna però specificare che non stiamo parlando di ottenre l’interoperabilità tra i vari tool di virtualizzazione, ma semplicemente l’utilizzo di tool comuni per alcuni particolari compiti, tipicamente la gestione, il monitoraggio e la protezione dei dati.

Esattamente d'accordo: il supporto multi-hypervisor non significa necessariamente piena interoperabilità, ma semplicemente un livello di astrazione che permette di portare a termine un compito senza dover scendere nel dettaglio di ciascuna tecnologia.

L'interoperabilità peraltro richiederebbe accordi fra concorrenti in un mercato che è ancora in rapida evoluzione, e rischierebbe così di rallentare o limitare la sana concorrenza.

> Ci si potrebbe chiedere se ha senso e se può portare qualche beneficio? Probabilmente per il singolo cliente no… che motivo potrebbe avere per introdurre nuovi costi legati all’ambiente eterogeneo (benché alcuni strumenti possono essere comuni, il formato delle VM, la loro mobilità, le competenze richieste, buona parte delle attività di amministrazione, … saranno diverse per ogni prodotto di virtualizzazione), costo per realtà medio-piccole non sarebbe facilmente giustificabile.

Su quest'altro punto però sono meno d'accordo: mentre per le piccole aziende è vero che ha senso concentrare le energie su un'unica piattaforma, già per le medie può succedere ad esempio che partano due progetti di virtualizzazione in parallelo, uno nel team Windows ed uno nel team Linux o Unix. Invece di obbligare tutti a convergere su un'unica piattaforma, può invece aver senso continuare ad usare ciascuna piattaforma per i propri punti di forza ed implementare un livello di astrazione che permetta la gestione e la visibilità unificata su tutte le diverse piattaforme.

C'è poi la dimensione dell'evoluzione da considerare. Se io oggi decido di concentrare tutte le mie energie sulla piattaforma A, ma domani mi fondo con, compro, o vengo comprato da una società che invece ha scelto la piattaforma B, potrei trovarmi in difficoltà. La fusione di sistemi e processi IT in questi casi è già abbastanza complessa senza mettere in campo anche una migrazione di piattaforma, per cui sarebbe utile avere a disposizione una piattaforma di astrazione che mi permetta di gestire nell'immediato le mie esigenze business e prendere con calma la decisione di migrare o meno le piattaforme di virtualizzazione.

Esiste infine anche la dimensione economica: se mi sono focalizzato su una sola piattaforma, ed improvvisamente il fornitore raddoppia i prezzi, non ho molte alternative. Se invece ho già in casa il materiale e le competenze su un'altra piattaforma, la migrazione è, se non indolore, comunque molto più semplice.

