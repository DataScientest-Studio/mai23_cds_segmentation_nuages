# mai23_cds_segmentation_nuages

Ce répertoire regroupe l'ensemble des ressources qui vous permettront d'éffectuer l'exploration du jeu de données, sa préparation ainsi que la conception d'un modèle basé l'algorithme Yolo.
Les Notebooks présentés ci-après on été conçus sous Anaconda / JupyterLab :

1. **Explotation.ipynb** : Il prend en entrée le dataset source brut clouds_0_large.csv. Ce Notebook fait appel au module de support utils_explo_prepa.ipynb
2. **Preparation.ipynb** : Il prend en entrée le dataset issu de l'exploration (clouds_1_large.csv) après que ce dernier ait été mis en forme. Ce Notebook fait appel au module de support utils_explo_prepa.ipynb
3. **Modelisation.ipynb** : Il prend en entrée le dataset source (clouds_0_large.csv) et produit le dataset clouds_2_large.csv après que ce dernier ait été enrichi de variables explicatives et expliquées supplémentaires. Ce Notebook fait appel au module de support utility.ipynb
4. **Les modules utils_explo_prepa.ipynb et utility.ipynb** regroupent un ensemble de fonctions personnalisées
5. **model.h5** : Enregistrement du modèle Yolo entrainé sur la base d'images au format 256 x 256, un LR de 1e-3 et avec de l'augmentation (translation d'image), Batchsize = 64 et Epoch = 20
6. **training_history.csv** :  Il s'agit de la courbe d'apprentissage à l'issu de l'entraiînement du modèle Yolo
7. **Le répertoire images/** contient un échantillon de 100 images satellite qui ont servi à cette étude. La racine de ce répertoire images/ contient des images aux dimensions 2100 x 1400 alors que le sous-répertoire contient un échantillon de 100 images aux dimensions réduites (256 x 256) et adaptées au modèle Yolo. Le dataset et les images d'origine peuvent être téléchargés à partir de kaggle à l'adresse suivante : https://www.kaggle.com/competitions/understanding_cloud_organization/data
