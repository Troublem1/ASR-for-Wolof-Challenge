# ASR-for-Wolof-Challenge

## BRIEF DESCRIPION
In a country such as Senegal, where about 50% of the population is illiterate, technologies and applications that are designed to be used by people who can read are not as effective as they could be. In this competition, your aim is to use Automatic Speech Recognition (ASR) techniques in the Wolof language to help illiterate people to interact with apps with just their voice, in a language they can already speak.

The goal of this competition is to build an ASR model that will help illiterate people use existing apps to find which bus they can take to reach their destination, without having to know how to read or write. check it out on [Zindi](https://zindi.africa/competitions/ai4d-baamtu-datamation-automatic-speech-recognition-in-wolof)

## Environment
- Conda Python 3.7.9
- cuda Tesla P100
- Kaggle

### input data should be structured as follows

<!-- .
|─ baamtu-asr
  ├─ clips                   #clips directory (alternatively `clip`)
  ├─ SampleSubmission.csv    #submission file  (alternatively `doc`)
  ├─ Train.csv               #train file with train id's to be updated to sn_train.csv after bamtu_ds_final.ipynb is run  (alternatively `train`)
  └─ Test.csv                #test file with test id's to be updated to ns_test.csv after bamtu_ds_final.ipynb is run  (alternatively `test`)

 -->

## How to run the code
having the data in te input directory, run Bamtu full ds.ipynb to create for new directory containing varients of the dataset.

Run Bamtu Full ds json.ipynb to generate manifet files train and test for all 4 variants of dataset.
Run in order
- fork_of_prep_files_before_major_training_on_00_asr .ipynb to output  trainedmodel2_v9.nemo
- run 10-retrain-fork-prepfilesbeforemajortraining.ipynb  to output  forktrainedmodel10_v1.nemo
- 10-1-reretrain-fork-prepfilesbeforemajortraining.ipynb  to output  forktrainedmodel11_v1.nemo
- 10-1-1-reretrain-fork-prepfilesbeforemajortraining .ipynb  to output  forktrainedmodel111_v1.nemo
- 10-1-1-5reretrain-fork-prepfilesbeforemajortrain.ipynb  to output  forktrainedmodel1115_v1.nemo
