# Nework Intrusion Detection using ML and DL

Hardware used - 


* For getting results on the CSV dataset - use `Anomaly_based_IDS.ipynb` notebook. 

* For getting results on the CICIDS2017 datasubset using nprintML, use the following steps - 
  * Download the subset data provided in the paper
  * Run `pcapml -M file.pcapng -O output-dir/ ` to get pcaps seperated by labels
  * Run the `IDSSubset.ipynb ` notebook to get any subset of pcaps from the pcap output directory
  * Run nprintml command `nprintml -a pcap --pcap_dir pcaps/ -L labels.csv -4 -t -c 25` to run nprintML

* For getting results on the CICIDS2017 datasubset using Doc2Vec, use the following steps -
  * Use the same subset as used for nprintML and run the `pcap_to_embeddings.ipynb` notebook for converting pcap files into hex documents
  * Now, run the `Pcap Embeddings.ipynb` to run the Doc2Vec model

