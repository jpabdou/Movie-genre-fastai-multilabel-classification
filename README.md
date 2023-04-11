This was a side project I started in 2021 in which I used movie poster images and IMDB data (all data and images were downloaded from the kaggle dataset here: https://www.kaggle.com/datasets/neha1703/movie-genre-from-its-poster). The purpose of this project was to identify the genres of movies from their posters as a means to get familiar with fastai's dataloader and learner functions.

Originally, I had identified posters by their first genre, but this led to an overselection of "dramas" and "comedies" as shown in the confusion matrix below. This makes sense as these terms can be broadly applied to many stories ("action comedy", "war drama", "romance drama", "romance comedy",etc.)
<img src="/first label confusion matrix.png" alt="confusion matrix generated from fastai training of movie posters and first genre labels"/>


Reattempting this project, I trained ResNet-50 model on 10 cycles with following results:
<img src="/Screenshot 2023-04-10 at 23-12-10 movie poster project multilabel - Jupyter Notebook.png" alt="fastai training and validation losses for 10 cycles"/>