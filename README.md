# infrrd_assignment
STEPS
Step1- for this task first we load the dataset in zip file in our colab enviorment and then unziping it
after unziping it we have to create our train datafraem from group of tsv files stored in train/boxes_transcripts_labels folder

STEP2- reading that folder and all the tsv files stored in it 
creating an dataframe with given column names given in the assignment for the train dataset having label named field

STEP3- now we have to study the dataset how many columns they have check for null values in the dataset and fill them if they are any

STEP4- perform EDA on the dataset which will tell the behaivour of the values present in the columns for example corelation matrix how 
values of one column affect others , box plots which shows us the outliers in the columns etc

STEP5- Pre-process the data like encoding, scaling for traing the model and assinging the weight as their was class imbalance in the dataset
so to overcome it we have to assigned class_weight_balance to each of the labels in the field

STEP6- divide data in X,Y Y is the field or the column on which we have to make the prediction 
Model traing now we have to train the model on the trained dataset to make the prediction 

STEP7- Prepare the validate set for predicting the value on the validate set

STEP8- Perform the same pre processing steps on the validate set same as of the training set with same columns so that the model can be fit on the 
validate dataset

STEP9- add the predictions as a column in the validate set for mapping in further steps

STEP10- Create the val_W_ann file by similar reading the folder and tsv files present in the folder it consists the answers of the validate set

STEP11- run the eval.py script to map the answers predicted by the model and given in the val_w_ann file

STEP12- it will generate the metrics.tsv file with precision,recall,f1score and support

NOTE- in my enviornment script was running fine it was showing me output too but file was not creted but it please consider it for evalution 
