# Modeling: Good default choices

## For all problems

- `rmsprop` as optimizer
- `Dense` layers
- `relu` activations for intermediate layers

## If data is limited

- k-fold cross-validation can help with better estimates of out of sample performance

## By task

| task    | binary | multiclass | regression |
| ------- | ------ | ---------- | ---------- |
| loss    | binary_crossentropy  | categorical_crossentropy | [mse](https://en.wikipedia.org/wiki/Mean_squared_error) |
| metrics | accuracy | accuracy | [mae](https://en.wikipedia.org/wiki/Mean_absolute_error) |
| output  | 1, sigmoid | k, softmax | 1, no activation |
