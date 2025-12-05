# Driver_attention

Ce projet utilise un modèle MobileNetV2 entraîné pour détecter si un conducteur est **attentif** ou **distrait**.  
Il combine deep learning et Mediapipe pour vérifier la présence du visage et le comptage des mains, ce qui permet de corriger certaines prédictions.

 Dataset **StateFarm Distracted Driver** téléchargé et placé dans le dossier `data/`
 https://www.kaggle.com/c/state-FARM-distracted-driver-detection
 Dataset a télécharge avant, et adapté le chemin sur Colab si besoin

 ## Utilisation

Le projet est prévu pour être utilisé directement sur **Google Colab**.  
Pour tester ou entraîner le modèle, il suffit de lancer les cellules du notebook **une par une**.

1. Ouvrir le notebook `driver_distraction.ipynb` sur Colab.
2. Monter Google Drive si besoin pour accéder aux images ou au dataset.
3. Exécuter les cellules dans l’ordre indiqué (prétraitement, entraînement, tests).
4. Vous pouvez uploader vos propres images pour tester le modèle.

## Résultats

- Précision finale sur validation : ~92,7%.
- Matrice de confusion et courbes d’évolution des performances disponibles dans le notebook.

## Notes

- Le notebook contient toutes les cellules pour l’entraînement, l’évaluation et les tests.  
- Assurez-vous d’avoir téléchargé le dataset avant de lancer l’exécution.  
- Le modèle corrige certaines prédictions grâce à Mediapipe (vérification visage/mains).
