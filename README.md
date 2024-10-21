# Intro to Zig Workshop in collaborazione con Crafted Software

## About
Il workshop e' stato creato in collaborazione con l'associazione culturale non a scopo di lucro di [Crafted Software](https://craftedsoftware.org).

Il workshop sara' tenuto dal sottoscritto, Loris Cro. Sul [mio profilo GitHub](https://github.com/kristoff-it/) potete trovare la mia bio completa con tanto di link. 

Per quanto concerne questo workshop piu' direttamente, sono laureato in informatica dal 2014 e lavoro full time alla Zig Software Foundation dalla sua fondazione (circa 4 anni fa). Mi e' gia' capitato di tenere workshop di Zig in passato e cercando il mio nome su YouTube potete trovare diversi talk a tema. Infine, potete trovarmi regolarmente [live su Twitch](https://twitch.tv/kristoff_it) a programmare in Zig mentre lavoro a vari progetti open source.

## Intro
Questo workshop di sei ore totali, divise in due incontri da tre ore l'uno, e' finalizzato a fornire una introduzione alla programmazione di basso livello ed al linguaggio di programmazione Zig.

Ogni incontro si struttura in 3 momenti principali:
1. Parte espositiva
2. Esercizi pratici
3. Q&A e presentazione di progetti open source concreti

Alla fine del corso i partecipanti avranno un'idea delle principali proprieta' della programmazione di basso livello e di 
come questa aiuti a realizzare software che sarebbe diversamente impossibile da realizzare con l'utilizzo esclusivo di 
linguaggi di alto livello, partendo dalla teoria, proseguendo per semplici esempi pratici, fino a leggere il codice di 
reali progetti open source scritti in Zig.

## Per chi e' questo workshop?
Ai partecipanti di questo workshop e' richiesto avere gia' esperienza di programmazione di alto livello [1], in quanto il workshop
si concentrera' sul descrivere la programmazione di basso livello in termini di paralleli e differenze respetto alla programmazione
di alto livello.

[1]: Ad esempio uno qualsiasi tra Python, JavaScript, Java, C#, PHP, Ruby, etc. 
     Esperienza di C/C++/Rust puo' essere d'aiuto ma non e' necessaria.

## Agenda
### Sabato 23
1. Introduzione a Zig
	1. Il progetto Zig
	2. Perche' imparare la programmazione di sistemi?
	3. Il workflow Zig (dev tools, compilatore, etc)
2. Esercizi
	1. Hello World
	2. Puntatori
	3. Corruzione della memoria
	4. Stack Vs Heap
3. Showcase:
	1. Zine: generatore di siti web statici scritto in Zig
	2. D2: WIP app di messaggistica istantanea 
4. Note conclusive
 
### Sabato 30
1. Introduzione a Zig (continua)
	1. Comptime
	2. Build System, Crosscompilazione
	3. Package manager
2. Esercizi
	1. Generics
	2. ArrayList, SegmentedList
	3. Crosscompilare per WASM
	4. Hello World GUI con DVUI
3. Q&A
4. Note Conclusive

## Prerequisiti
L'unico prerequisito per partecipare al workshop e' di avere installato il compilatore Zig **versione 0.13.0**.

>[!NOTE]
>Avrete installato Zig correttamente quando potrete aprire un terminale / prompt dei comandi / powershell e il comando `zig version` viene eseguito con successo e riporta la versione 0.13.0

Zig e' disponibile su tutti i principali OS e consiste in un singolo archivio senza ulteriori dipendenze che richiede solo di essere estratto da qualche parte per poter essere utilizzato.

Pagina dei download:  
https://ziglang.org/download/

Istruzioni iniziali:
https://ziglang.org/learn/getting-started/

Qualora vogliate usare il package manager del vostro sistema operativo, sentitevi liberi di farlo fintanto che abbiate modo di ottenere la versione 0.13.0.

Per chi lo preferisse, esiste un manager di versioni di Zig creato dalla community chiamato zigup:  
https://github.com/marler8997/zigup

Alcuni suggerimenti specifici per alcuni OS:

- NixOS: Zig crea di default eseguibili con static linking quindi non preoccupatevi di dover ottenere una versione speciale del compilatore (il compilatore stesso e' un eseguibile statico).
- Windows: Zig funziona su windows senza bisogno di ricorrere a WSL, docker, o altre forme di virtualizzazione.

In generale sconsiglio fortemente l'uso di Docker o VM varie per ottenere Zig.

### Editor Tooling

Tutti gli editor principali hanno qualche forma di supporto per Zig, assicuratevi che almeno sia supportata la colorazione della sintassi.

Opzionalmente:
- Se il vostro editor supporta LSP, installate ZLS (https://github.com/zigtools/zls) per ottenere un po' di aiuto in-editor.
- Se non usate LSP, impostate `zig fmt` come comando da eseguire on save.
- Se usate VSCode, installando l'estensione ufficiale di Zig, potete far gestire all'estensione sia l'installazione di Zig che di ZLS. Raccomanderei comunque di gestire voi manualmente almeno l'installazione del compilatore.


## Community
Zig descrive la propria community come "decentralizzata", nel senso che non esiste un luogo ufficiale di discussione. Di conseguenza sta alla sensibilita' del singolo utente la scielta di a quale/i community unirsi.

L'elenco delle community "conosciute" e' una pagina sulla wiki del repository ufficiale:  
https://github.com/ziglang/zig/wiki/Community

Per le finalita' di questo workshop, e' fortemente consigliato unirsi al gruppo telegram "Zig Italia" creato dal sottoscritto: https://t.me/ziglang_it

**Qualora abbiate problemi a fare il setup iniziale, chiedete aiuto nel gruppo Telegram.**

A presto,
Loris Cro


