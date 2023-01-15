# NLP_eng_hindi_translation
Converting english text into hindi text

Instruction for the Hindi Transliteration Model

1.eng-hindi-trans.ipynb
	Is the jupyter notebook file in which I use the XML file for test, validate and training of data.
Before passing this data directly to the model. I have converted this xml file into the pandas data frame to ease the pre-processing.
In last of notebook, I have shown some examples to showcase the results.
As the data from training the model was less therefore model need to run for more epochs.
for 100 epoch’s the BLEU Score: 0.4131308522495705
for 200 epoch’s the BLEU Score: 0.5087270435881411

so, as the epoch’s are increasing the accuracy of the model is also increasing.


2.NEWS2018_M-EnHi_trn.xml 	NEWS2018_M-EnHi_dev.xml  	NEWS2018_M-EnHi_tst.xml 
	train data 		validate data			test data

