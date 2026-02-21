# kommunalwahl_darmstadt_voto_analyse  
Analysiere die Fragen und Parteiantworten von [Voto](https://app.voto.vote/de/elections/9271389) für die Kommunalwahl in Darmstadt.  

In `extract_data_from_html.ipynb` werden die Daten aus einem HTML File extrahiert. Dazu sollte man in Voto alle Fragen beantworten, um zur Result-Seite zu kommen. Dort wählt man alle Listen aus und geht dann auf die Übersicht. Diese Seite speichert man sich nun lokal ab. Voto nutzt scheinbar keine API, um die Antworten der Listen zu laden. Alle benötigten Daten sind im HTML File gespeichert.  

Das Notebook `create_clustermap.ipynb` erzeugt basierend auf den Fragen und Antworten der Listen eine Seaborn Clustermap.  

`calculate_party_similarity.ipynb` berechnet die Ähnlichkeiten der Parteien, basierend auf den Voto-Antworten. Dabei wird so getan, als würden die Parteien Voto beantworten.  

Wer sich nur für die Daten und Plots interessiert, kann direkt in die entsprechenden Ordner einsteigen. 