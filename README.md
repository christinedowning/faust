# faust
 //Lo stetoscopio ci mostra il contenuto del suono nel dominio della frequenza
 //Sull'asse delle x le frequenze sull'asse delle y l'ampienza
 //L'oscilloscopio ci mostra il contenuto del suono nel dominio del tempo sull'asse delle X il tempo e sull'asse delle Y le ampiezze.
 //Lowpasse uno dei filtri più semplici da usare e significa "passa basso".
 import("stdfaust.lib");
process = no.noise : fi.lowpass(2,6000) : fi.highpass(2,6000);
