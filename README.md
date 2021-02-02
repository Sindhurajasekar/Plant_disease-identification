### Execution steps:

#### Training Process
```
1. Place 'data_extraction.py' in Train folder of the selected leaf folder. e.g..
cp data_extraction.py Bell\ Pepper\ Data\ Set/Train_pep_bac/.
2. Create a text file in leaf folder( eg. Bell Pepper Data Set) with naming 'DiseaseType_result.txt'. e.g..
touch Bell\ Pepper\ Data\ Set/bacterial_result.txt
3. Go to Train folder. eg..
cd Bell\ Pepper\ Data\ Set/Train_pep_bac/
4. Update filename on line 162, with file name created in step 2.
5. Execute the data_extraction file
python data_extraction.py
6. Repeat for each Train folder in selected leaf folder
```
At the end of the text file such as 'bacterial_result.txt', the average infection percentage for that particular disease for the selected leaf type will be mentioned.

After creating training text file for each training folder.

### Test Process
```
1. Place 'data_marking.py' and 'leaf_classification.py' in Test folder of the selected leaf folder. e.g..
cp data_marking.py Bell\ Pepper\ Data\ Set/Test_pep_bac/.
cp leaf_classification.py Bell\ Pepper\ Data\ Set/Test_pep_bac/.

2. Create a text file in leaf folder( eg. Bell Pepper Data Set/Test_pep_healthy/) with naming 'DiseaseType__test_result.txt'. e.g..
touch Bell\ Pepper\ Data\ Set/Test_pep_healthy/healthy_test_result.txt

3. Go to Train folder. eg..
cd Bell\ Pepper\ Data\ Set/Test_pep_healthy/

4. Update filename on line 134 of data_marking, with file name created in step 2.

5. Change leaf marking as 'Healthy' or 'Infected' at line 151 and 164 of data_marking.

6. Execute the data_marking file
python data_marking.py

7. Execute the leaf_classification file
python leaf_classification.py

8. Repeat for each test folder
```

At the end of the text file such as 'healthy_test_result.txt', the classification accuracy for that particular disease for the selected leaf type will be mentioned.


