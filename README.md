## **COVID19 - Predirre i nuovi positivi nei prossimi 7 giorni**

# **Introduzione**
Nell'ambito dei miei studi professionali e personali, mi sto cimentando nelle reti neurali e in particolare ora mi sto dedicando alle Long Short Term Memory. 

Ho deciso di provare a predirre l'andamento della pandemia, partendo da una considerazione, il tempo di incubazione di 14 giorni, ovvero, non è errato astrarre che i nuovi positivi di oggi sono una conseguenza dei positivi dei 14 giorni scorsi.

Partendo da questa ipotesi ho trainato una rete neurale LSTM con i dati del dipartimento della protezione civile e, una volta finito di lavorare alla rete, hofatto una previsione ed ho poi analizzato i risultati. 

La previsione era sul periodo 21 Settembre - 28 Settembre; il primo giorno (21 Settembre) il dato viene predetto utilizzando i dati dei 14 giorni precedenti, dati reali e misurati, il secondo giorno in realta utilizza 13/14 di dati reali e 1/14 di dati predetti, ovvero quelli del giorno precedente.

# *Cosa mi sarei aspettato?*
Dai risultati del training della rete neurale avevo un errore che è fisiologico e me lo sarei aspettato analogo per il primo giorno, quello che mi metteva paura era la previsione del secondo e del terzo giorno, perchè i dati con cui viene fatto il forecast, a differenza di quelli del primo giorno, portano oltre l'errore intrinseco della previsione, anche l'errore dei giorni precedenti, per cui più si va avanti nel tempo con dati stimati dalla rete neurale, maggiore è la possibilità di errore.

# *Cosa ho riscontrato?*
Con un certo stupore ho riscontrato che il dato predetto ogni giorno, aveva un errore inferiore al 10% dal dato reale, questo mi ha colto di sorpresa ma mi ha portato a condividere con voi i miei risultati.

# *Cosa farò adesso?*
Il prossimo step è riscrivere la documentazione, questo README lascia a desiderare e soprattutto vorrei scriverlo in inglese così che possa essere di aiuto a tutti, intanto vi invito a scaricare il notebook o provarlo direttamente sul mio spazio Google colab a [questo link](https://colab.research.google.com/drive/1M_oZ0tVbpQ9wQ2Iypu1qTBfR99la0rkL?usp=sharing)
