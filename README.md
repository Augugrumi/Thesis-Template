# Thesis-Template
Repository per il template della tesi

---

# Compilazione
Il template è compilabile, in ambiente Linux, dando il comando :
```bash
../Thesis-Template$ make
```
oppure
```bash
../Thesis-Template$ make PRINT=n
```
dalla directory principale del progetto. È possibile compilare il documento per avere una versione per la stampa anche nel
caso in cui si voglia stampare il frontespizio su pelle dando il comando:
```bash
../Thesis-Template$ make PRINT=y
```

---

# Configurazione
Nel file `Thesis-Template/config/config.tex` è possibile configurare il template con i propri dati personali settando il 
valore delle seguenti variabili:
```TeX
\newcommand{\myName}{Nome Cognome}                              % nome e cognome dell'autore della tesi
\newcommand{\myTitle}{Una tesi bellissima}                      % titolo della tesi
\newcommand{\mySupervisor}{Nome cognome}                        % nome e cognome del relatore
\newcommand{\myCoSupervisor}{Nome Cognome}                      % nome e cognome del co-relatore
% -----------------------------------------------------------------------------
% lasciare solo \booltrue{ifCoSupervisor} o \boolfalse{ifCoSupervisor}
% rispettivamente se è presente o meno un co-relatore
\newbool{ifCoSupervisor}
\booltrue{ifCoSupervisor}
\boolfalse{ifCoSupervisor}
% -----------------------------------------------------------------------------
\newcommand{\myDegree}{Tesi di laurea magistrale}               % tipo di tesi
\newcommand{\myUni}{Università degli Studi di Padova}           % università
\newcommand{\myFaculty}{Corso di Laurea in Informatica}         % facoltà
\newcommand{\myDepartment}{Dipartimento di Matematica}          % dipartimento
\newcommand{\myLocation}{Padova}                                % dove
\newcommand{\myAA}{2017-2018}                                   % anno
\newcommand{\myTime}{Sett 2018}
```
