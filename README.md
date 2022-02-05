# AgroCode_Hackathon
Решение задачи в рамках AgroCode Data Science Cup, где это решение заняло первое место.<br>
Для решение задачи было необходимо классифицировать текста, и выделить спаны.<br>
Score считался следующим образом:<br>
  Score = 0.8*(1 - logloss) + 0.2*F1<br>
  * F1 - качество выделения спанов (задача NER)<br>
  * Logloss - качество multi-label классификации<br>
Для multi-label и NER классификации использовалась модель LaBSE-en-ru (https://huggingface.co/cointegrated/LaBSE-en-ru).<br>
Изначально было необходимо доразметить спаны в тексте.<br>
Для аугментации текстовых данных использовался код из data_augmentation.ipynb.<br>
