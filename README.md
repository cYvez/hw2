# homework 2

## environment
- easily use google colab to run `Homework_2.ipynb`
![colab](https://github.com/cYvez/hw2/tree/master/figures/colab.png)
- if your want to use your local environment to run this code, make sure you have tensorflow 2.x (that is because we use google colab to save the model, resulting in model files which are not compatible with tensorflow1.x)

## how to run the code
1. down this repo
2. Download the validation and test datasets from [here](https://drive.google.com/drive/folders/1Rs68uH8Xqa4j6UxG53wzD0uyI8347dSq?usp=sharing) and put the `.h5` datafile into `/data`:
```bash
├── data 
    └── cl
        └── valid.h5 // this is clean validation data used to design the defense
        └── test.h5  // this is clean test data used to evaluate the BadNet
    └── bd
        └── bd_valid.h5 // this is sunglasses poisoned validation data
        └── bd_test.h5  // this is sunglasses poisoned test data
```
3. open this project in google colab, and run `Homework_2.ipynb`, after run all code, you will see the repaired networks under `/goodnets`, goodnet_2, goodnet_4, goodnet_10 denote the repaired networks for `X`={2%, 4%, 10%}, respectively.


## how to evaluate my repaired model
I have provided the code of the evaluation at the end of Homework_2.ipynb, you can check the evaluation results or run it with google colab
![eval](https://github.com/cYvez/hw2/tree/master/figures/eval.png)
