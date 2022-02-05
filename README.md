# AgroCode_Hackathon
Решение задачи в рамках AgroCode Data Science Cup, где это решение заняло первое место.\n
Для решение задачи было необходимо классифицировать текста, и выделить спаны.\n
Score считался следующим образом:\n
  Score = 0.8*(1 - logloss) + 0.2*F1\n
  F1 - качество выделения спанов (задача NER)\n
  Logloss - качество multi-label классификации\n
Для multi-label и NER классификации использовалась модель LaBSE-en-ru (https://huggingface.co/cointegrated/LaBSE-en-ru).\n
Изначально было необходимо доразметить спаны в тексте.\n
Для аугментации текстовых данных использовался код из data_augmentation.ipynb.\n
