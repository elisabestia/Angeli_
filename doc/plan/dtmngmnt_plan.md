# Indice 
- [Autrice](#Autrice)
- [Sommario esecutivo](#Sommarioesecutivo)
- [Introduzione](#Introduzione)
- [Descrizione dei dati](#Descrizionedeidati)
- [Documentazione e archiviazione dei dati](#Documentazioneearchiviazionedeidati)
- [Licenza](#Licenza)

 # Autrice
Elisabetta Sabattini, <https://orcid.org/0009-0007-9900-8895>, Università di Bologna 

 # Sommario esecutivo
1. Scelta dei brani dall'opera di Diego [Diego Angeli, Le Chiese di Roma, Roma, Società Editrice Dante Alighieri, 1922.](https://archive.org/details/lechiesediromagu00ange_0/page/n7/mode/2up)
2. Dai testi scelti in formato ```.txt```, estrazione manuale dei dati 
4. Organizzazione in forma tabellare tramite [Excel](https://excel.cloud.microsoft/)
5. Conversione in ```.csv```
6. Applicazione di [Open Refine](https://openrefine.org/) per riconciliare le authority di nomi delle chiese 
7. Sulla base dell'ultima tabella ```.csv```, marcatura seguendo [XML TEI](https://vscode.dev/)
8. Ipotesi di lavoro

 # Introduzione
_Quer pasticciaccio_ è il titolo del progetto d’esame per il corso di [DHDM](https://www.unibo.it/it/studiare/insegnamenti-competenze-trasversali-moocs/insegnamenti/insegnamento/2024/502386) (a.a. 2024/2025). Il progetto mira alla realizzazione di una pipeline capace di integrare i dati presenti nei file ```.csv```, verificarne le authority e convertirli secondo il formato XML TEI. Sebbene il risultato finale si discosti dall'obiettivo iniziale, il lavoro svolto ha offerto spunti significativi di riflessione e individuato possibili direzioni di sviluppo futuro.

 # Descrizione dei dati
![image](https://github.com/user-attachments/assets/b0b8f115-f4aa-44b0-927f-19f16f7aea75)

I dati sono stati raccolti a partire dalla versione formato ```.txt``` dell'opera di Diego Angeli, Le Chiese di Roma. 

Dai passaggi scelti sono stati identificati vari elementi d'interesse, come: 

- nome_chiesa
- altri_nomi
- posizione
- data_costruzione
- data_riedificazione_restauro
- responsabili_elementi_architettonici_interni
- elementi_scultorei_interni
- responsabili_elementi_scultorei_interni
- elementi_pittorici_destra
- responsabili_elementi_pittorici_destra
- elementi_pittorici_sinistra
- responsabili_elementi_ pittorici_sinistra

A partire da una strutturazione preliminare dei dati in formato tabellare (Excel), si è proceduto con la conversione in formato ```.csv``` e, attraverso l'impiego di Open Refine, è stato effettuato il controllo authority relative al campo _nome_chiesa_.   
Completata la fase di pulizia e verifica, il nuovo obiettivo è la marcatura dei testi selezionati secondo lo standard XML-TEI, utilizzando come riferimento i dati estratti e strutturati nel file ```.csv```. 

Tuttavia, il risultato ottenuto presenta una marcata disomogeneità e una scarsa coerenza tra le entità descritte nel file ```.csv``` e la loro rappresentazione nella codifica XML-TEI, con particolare riferimento agli elementi di natura scultorea e pittorica. Ciò compromette l'affidabilità e l'interoperabilità del dataset all'interno di un contesto di valorizzazione e analisi digitale del patrimonio.

In ultima analisi, _Quer pasticciaccio_ ha permesso alcune riflessioni e spunti di lavoro futuro: 

- partire dalla marcatura del testo utilizzando un thesaurus consolidato come quello del [Getty Research Institute](https://www.getty.edu/research/tools/vocabularies/aat/)
- procedere con l'estrazione e la strutturazione dei dati in ```.csv```
- completare il processo con la riconciliazione delle authority tramite OpenRefine.

Solo seguendo questo percorso sistematico si potrà ottenere un dataset affidabile, coerente e interoperabile, capace di valorizzare adeguatamente il patrimonio culturale analizzato e di supportare future ricerche digitali in ambito storico-artistico.

 # Documentazione e archiviazione dei dati 
I dati sono archiviati e resi accessibili su Git Hub, il cui dataset è composto da due cartelle:

1. data, che include due sotto cartelle, **csv** e **xml** ;
2. docs, al cui interno sono presenti la **fonte** utilizzata e il  **data management plan**

Inoltre si è provveduto a preservare i dataset tabellari pubblicandoli su [Zenodo](https://zenodo.org/) e creando un DOI per ognuno di essi. 

# Licenza 
La scelta della licenza ```CC0 1.0 Universal``` è stata presa rispetto alla volontà di rendere il tutto accessibile e disponibile. 
 
