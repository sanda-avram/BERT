# BERT
## Fine-tunning the pretraied BERT model on ROST

The source code for the tests mentioned in  "[BERT-based Authorship Attribution on the Romanian Dataset called ROST are processed with BERT](https://www.researchgate.net/publication/367557751_BERT-based_Authorship_Attribution_on_the_Romanian_Dataset_called_ROST)"  and use the BERT pretrained model: "dumitrescustefan/bert-base-romanian-cased-v1"

The texts used for fine-tuning the pretrained model are those described in the paper called "[A comparison of several AI techniques for authorship attribution on Romanian texts](https://www.researchgate.net/publication/365299177_A_comparison_of_several_AI_techniques_for_authorship_attribution_on_Romanian_texts)".

The initial texts varied in length from 91 to 39195 words. In order to have proper inputs for the BERT pretrained model, they needed to be split into fixed length sizes. Preliminary test run on lengths of 91, 200, and 400 words gave better results for 200 words. 


* **ROST_200tokens_Set1.ipynb** + **ROST_200tokens_Set1_run2.ipynb** + **ROST3.ipynb** - are the source codes used for executing the first shuffle, named Set1
* **ROST_200tokens_Set2.ipynb** + **ROST4.ipynb** - are the source codes used for executing the second shuffle, named Set2
* **ROST_200tokens_Set3.ipynb** + **ROST5.ipynb** - are the source codes used for executing the third shuffle, named Set3

For the next set of texts we considered to limit the text fragments to have the minim lentgh of 100 words (tokens). Therefore, the only text that was 91 words was adjusted to the length of 114 words ("[Ziua Apocalipsei] (http://www.povesti.org/#ziua_apocalipsei)" written by Mihai Oltean). 

We will post as soon as possible the source codes for the new dataset used for fine-tuning. 
