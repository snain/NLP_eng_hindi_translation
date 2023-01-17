# NLP_eng_hindi_translation
Converting english text into hindi text

Instruction for the Hindi Transliteration Model<br>
<b>1.</b>
<pre>

eng-hindi-trans.ipynb
	Is the jupyter notebook file in which I use the XML file for test, validate and training of data.
Before passing this data directly to the model. I have converted this xml file into the pandas data frame to ease the pre-processing.
In last of notebook, I have shown some examples to showcase the results.
As the data from training the model was less therefore model need to run for more epochs.

for 100 epoch’s the BLEU Score: 0.4131308522495705<br>
for 200 epoch’s the BLEU Score: 0.5087270435881411<br>
so, as the epoch’s are increasing the accuracy of the model is also increasing.
</pre>
<b>2.</b>
<pre>
NEWS2018_M-EnHi_trn.xml 	NEWS2018_M-EnHi_dev.xml  	NEWS2018_M-EnHi_tst.xml 
	train data 		validate data			test data

</pre>
<b>3. work flow</b>
<pre>
read the data from the xml file and convert it into the pandas data frame 
converting sentence from the data frame into the characters to see the frequency 
then we will convert these char into id's 
converting the ids into vector matrix

<b>Making the RNN model</b>
1.Encoding layer
2.Decording layer
3.Dropout for regularization
4.Dense layer
5.output layer with optimizer as Adam learning rate=0.0001

passing the data into list form as (eng_word,hindi_word) and splitting it into 95% and 5% for training and validation.
running the model for 200 epochs’

<b>making a test function (transliterate (input English word))</b>
1.converting the word into the id
2.passing ids to the RNN model
3.we will get the predicted output into the id format 
4.convert back these ids into the Hindi word

</pre>
