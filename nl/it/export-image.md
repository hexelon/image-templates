---

copyright:
  years: 2014, 2018
lastupdated: "2018-09-19"

keywords:

subcollection: image-templates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Esportazione di un'immagine in OpenStack Swift
{: #exporting-an-image-to-openstack-swift}

Dalla pagina Template dell'immagine, puoi esportare un template dell'immagine in un account [Object Storage OpenStack Swift](/docs/infrastructure/objectstorage-swift?topic=objectstorage-swift-GettingStarted#getting-started-with-object-storage-openstack-swift).
{:shortdesc}

Il processo di esportazione dell'immagine prende un template dell'immagine standard privato preesistente e converte l'immagine in un
file immagine memorizzato in una specifica ubicazione in un account Object Storage OpenStack Swift. Utilizza i seguenti passi per esportare un template dell'immagine.

1. Dal menu **Dispositivi** nel [{{site.data.keyword.slportal_full}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/), seleziona **Gestisci > Immagini**.
2. Fai clic su **Azioni** per il template dell'immagine che desideri esportare e seleziona **Esporta immagine**. Se un template dell'immagine con la configurazione che desideri non è ancora
disponibile, vedi [Creazione di un template dell'immagine](/docs/infrastructure/image-templates?topic=image-templates-creating-an-image-template).
3. Nella pagina Esporta immagine, immetti il nome file dell'immagine nel campo **Nome file**.
5. Dall'elenco a discesa **Account**, seleziona un **Account Object Storage**.
6. Dall'elenco a discesa **Cluster**, seleziona un **Cluster Object Storage**.
7. Dall'elenco a discesa **Contenitore**, seleziona un **Contenitore Object Storage**.
8. Fai clic su **Esporta immagine** per esportare l'immagine nell'ubicazione specificata nell'Account Object Storage. Fai clic su **Chiudi** per annullare l'azione.

## Passi successivi

Una volta che hai esportato un'immagine, rimane nell'elenco dei template dell'immagine, ma è disponibile anche come file nell'ubicazione Object Storage OpenStack Swift specificata durante il processo di esportazione. Per ulteriori informazioni sulla visualizzazione di un file
esportato in un Account Object Storage, vedi [Visualizzazione e modifica dei dettagli del file](/docs/infrastructure/objectstorage-swift?topic=objectstorage-swift-OSSSLPortal#viewing-and-editing-file-details). Poiché ciascuna immagine ha dimensione e caratteristiche diverse,
il completamento del processo di esportazione potrebbe richiedere diversi minuti. La velocità media di esportazione è di 2 GB al minuto. Se trascorrono diversi minuti e l'immagine non è ancora
disponibile nell'Account Object Storage OpenStack Swift, [contatta il supporto](/docs/get-support?topic=get-support-getting-customer-support).
