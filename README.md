# Texture-segmentation
## Modeling and segmentation images that described by causal autoregressive model with mask [(0,-1),(-1,0),(-1,-1)]  
autoreg_img() - моделирует изображение, описываемых quarter-plane каузальной моделью авторегрессии с маской [(0, -1), (-1, 0), (-1, -1)]  
autocov() – считает выборочную автокорреляционную функцию по входной матрице и заданному лагу  
yule_walker_sol() - вычисляет оценки Юла-Уокера коэффициентов модели по входному изображению  
autoreg_img_half() - моделирует тестовое для алгоритма сегментации изображение с двумя однородными областями с горизонтальной границей  
autoreg_img_sq_of() - моделирует тестовое для алгоритма сегментации изображение с квадратом внутри фоновой области  
autoreg_img_tr_of() - моделирует тестовое для алгоритма сегментации изображение с прямоугольным треугольником внутри фоновой области  
segm_dict_sq_bound() - реализует алгоритм сегментации, основанный на Байесовском правиле проверки гипотез; возвращает словарь, где координатам каждого пикселя сопоставляется значение интенсивности либо 1, либо 255 (т.е. фактически определение принадлежности к одной из областей, черной или белой)  
segm_result() - возвращает результирующее сегментированное изображение и долю верно сегментированных пикселей в каждой области  
clust_coefs() - определяет параметры однородных областей по тестовому изображению на основе кластеризации k-means; визуализирует полученный набор коэффициентов и их принадлежность к кластерам
