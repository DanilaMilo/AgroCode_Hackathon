# AgroCode_Hackathon
Решение задачи в рамках AgroCode Data Science Cup, где это решение заняло первое место.
Для решение задачи было необходимо классифицировать текста, и выделить спаны.
Score считался следующим образом:
  Score = 0.8*(1 - logloss) + 0.2*F1
  F1 - качество выделения спанов (задача NER)
  Logloss - качество multi-label классификации
Для multi-label и NER классификации использовалась модель LaBSE-en-ru (https://huggingface.co/cointegrated/LaBSE-en-ru).
Изначально было необходимо доразметить спаны в тексте.
Для аугментации текстовых данных использовался код из data_augmentation.ipynb.
