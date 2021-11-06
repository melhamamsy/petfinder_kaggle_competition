# petfinder_kaggle_competition
This is a team approach to solving the petfinder competition using 3 types of data (Images, Text, and tabular)

## Link
https://www.kaggle.com/c/petfinder-pawpularity-score

## Approach
a. Image Data:
> Use InceptionV3 as base, train the last layers only, and extract features to represent images.

b. Text Data:
> Use Glove embeddings to embed words, and then learn an embedding for the whole document using LSTM

c. Tabular Data:
> Use ANN to extract latent features

d. Concat all of them and feed them to another model that predicts the final label (1,2,3,4) as continuous varibale

e. Clip the prediction [1,4] and round to nearest int.

![image](https://user-images.githubusercontent.com/63168028/140625228-89a4c864-3bbf-45f4-a04f-e43177768145.png)
