# mai23_cds_segmentation_nuages

Ce dossier contient des notebooks pour la conception et l'entraînement des premiers modèles basés sur l'architecture EfficientNet.
Il y a les notebooks de pré-process dans process_csv, et les notebooks de conception et d'entrainement, et de test dans 'train_models_efficientNet. Attention, ils ont été exportés de googleCollab, certain chemin sont à revoir et certaines commandes ne sont pas nécessaires.

- Contenu initial du dossier

1. process_csv/cloudiatlas.ipynb
    Il permet notamment de créer les données de Bounding Box à partir des RLE, de définir la ou les classes par images, et le ratio entre la surface du masque des RLE et la surface des bbox
2. train_models_efficientNet/first_model.ipynb
    Premier modèle qui fait une régession sur les données des bbox
3. train_models_efficientNet/first_model_avecClassification.ipynb
    Deuxième modèle qui fait une classification des images
4. train_models_efficientNet/test_models_surImages.ipynb
    Permet d'utiliser les deux modèles entraînés pour prédire sur une image la région nuageuse et sa classe.
