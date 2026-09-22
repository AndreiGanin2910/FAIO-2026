# FAIO 2025 — финальные решения

Два воспроизводимых решения задач отборочного этапа FAIO. В каждой папке находится один финальный ноутбук с полным циклом от чтения данных до формирования `solution.csv`.

| Задача | Направление | Результат | Подход |
|---|---|---:|---|
| [Кто дал оценку](task-a-translation-annotator/) | NLP, бинарная классификация | ROC-AUC **0.7622** | COMETinho, pairwise features, ensemble |
| [Обратная нормализация текста](task-d-itn-bio/) | Token classification | span-level F1 **≈0.914** | RuBERT, vocabulary expansion, BIO-Viterbi |

## Запуск

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Перейдите в папку задачи, добавьте `train.csv` и `test.csv`, затем выполните ноутбук сверху вниз. Данные, веса, кэш и файлы отправки исключены из Git.

