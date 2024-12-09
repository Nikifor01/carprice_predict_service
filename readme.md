1. На первом этапе были загружены и визульно осмотренны данные, так же был сделан дашборд для наглядного представления данных. Была осущестлена проверка данных на пропуски, после чего пропуски были удалены. Так же была проведена визуализация в рамках EDA. При обучениее все модели измерялись с R^2 и MSE
2. Далее данные были подготовлены для построения модели только на вещественных признаках, в процессе они были приведены к правильному формату, в конечном итге данные были разделены на тренировочный и тестовый напоборы, на них была обучена пустая регрессия без всего
3. Применил StandardScaler и добавлена регуляризация L1 и обучена регрессия уже с ней для улучшения качества модели
4. Далее применил ElasticNet(L1 + L2 регуляризации), а так же применён GridSearch для подбора наилучших параметров
5. После я обработал категориальные фичи предварительно закодированные onehotencoding, обучил Ridge (L2) на категориальных переменных
6. Далее датасеты были объеденены, следующая модель уже обучалась на всех признаках и категориальных и численных
7. Решение бизнесовой задачи, а именно оценка кастомной метрики
8. В конце был реализован сервис на фастапи, чтобы можно было пользоваться моделей

<img width="1440" alt="Снимок экрана 2024-12-09 в 23 54 43" src="https://github.com/user-attachments/assets/78f3c3ec-07eb-4ccc-9bad-4986a55d001d">
<img width="1440" alt="Снимок экрана 2024-12-09 в 23 54 55" src="https://github.com/user-attachments/assets/bcc50095-5291-48c8-a0ea-b7b17de3c1af">
<img width="1440" alt="Снимок экрана 2024-12-09 в 23 54 36" src="https://github.com/user-attachments/assets/89f1a6d4-5e16-4662-a964-1ed9c3f3569b">
<img width="1440" alt="Снимок экрана 2024-12-09 в 23 54 23" src="https://github.com/user-attachments/assets/1592020f-b15f-4a39-9abc-dd78535f1a02">
<img width="1440" alt="Снимок экрана 2024-12-09 в 23 54 02" src="https://github.com/user-attachments/assets/110e1537-9e06-43e5-adb6-26a1a012e26e">
