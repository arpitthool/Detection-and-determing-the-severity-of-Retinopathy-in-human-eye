
Transfer learning is the process of transferring the knowledge gained in one task in a
specific domain to a related task in a similar domain. 


#### Goal 

- [x] To leverage transfer learning in solving real world problems
- [x] Look at the achitecture of Standard CNN architectures that can be used for Transfer Learning
- [x] Be comfortable on various facets of performing Transfer learning 

#### Dataset Link
[Data] (https://www.kaggle.com/c/classroom-diabetic-retinopathy-detection-competition/data)

#### Command to execute TransferLearning.py 

```bash

python TransferLearning.py --path '/media/santanu/9eb9b6dc-b380-486e-b4fd-c424a325b976/book AI/Diabetic Retinopathy/Extra/assignment2_train_dataset/' --class_folders '["class0","class1","class2","class3","class4"]' --dim 224 --lr 1e-4 --batch_size 16 --epochs 20 --initial_layers_to_freeze 10 --model InceptionV3 --folds 5 --outdir '/home/santanu/ML_DS_Catalog-/Transfer_Learning_DR/'

```

#### Command to execute TransferLearning_ffd.py 



```bash
python TransferLearning_ffd.py --path '/media/santanu/9eb9b6dc-b380-486e-b4fd-c424a325b976/book AI/Diabetic Retinopathy/Extra/assignment2_train_dataset/' --class_folders '["class0","class1","class2","class3","class4"]' --dim 224 --lr 1e-4 --batch_size 32 --epochs 50 --initial_layers_to_freeze 10 --model InceptionV3 --outdir '/home/santanu/ML_DS_Catalog-/Transfer_Learning_DR/'

```

#### TransferLearning_reg.py for Training 
```bash
python TransferLearning_reg.py --path '/media/santanu/9eb9b6dc-b380-486e-b4fd-c424a325b976/book AI/Diabetic Retinopathy/Extra/assignment2_train_dataset/' --class_folders '["class0","class1","class2","class3","class4"]' --dim 224 --lr 1e-4 --batch_size 32 --epochs 5 --initial_layers_to_freeze 10 --model InceptionV3 --folds 5 --outdir '/home/santanu/ML_DS_Catalog-/Transfer_Learning_DR/Regression/'

```
#### TransferLearning_reg.py for Validation 

```bash

python TransferLearning_reg.py --path '/media/santanu/9eb9b6dc-b380-486e-b4fd-c424a325b976/book AI/Diabetic Retinopathy/Extra/assignment2_train_dataset/' --class_folders '["class0","class1","class2","class3","class4"]' --dim 224 --lr 1e-4 --batch_size 32 --model InceptionV3 --outdir '/home/santanu/ML_DS_Catalog-/Transfer_Learning_DR/Regression/' --mode validation --model_save_dest --'/home/santanu/ML_DS_Catalog-/Transfer_Learning_DR/Regression/model_dict.pkl' --folds 5

