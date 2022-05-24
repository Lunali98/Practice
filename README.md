# Practice
We automatically collected all the diary entries from the "Lived" web archive, filtered by the right dates, lemmatized the entries, and automatically generated topics using the LDA algorithm. 

I filtered those records in which the word "war" appeared, divided them into three stages: 
Before Great Patriotic War: 970 entries
Great Patriotic War: 8,063 entries	
After Patriotic War: 1,248 records

One of the main tasks of natural language processing is automatic extraction of topics from large volumes of text - topic modeling. I used the Latent Dirichlet Allocation (LDA) algorithm for topic modeling. The LDA approach to topic modeling is that each document is treated as a set of topics in a certain proportion. And each topic as a set of keywords, again, in a certain proportion.
Once you tell the algorithm the number of topics, all it will do is display the distribution of topics in the documents and the distribution of keywords by topic.
A topic is nothing more than a set of dominant keywords. Just by looking at the keywords, you can determine what the topic is about.
We are given three sets of 10 topics each. Each set is a cross-section of diary entries by time period: Before Great Patriotic War, Great Patriotic War, After Patriotic War. 
How do we interpret this?
Theme 0 is represented as '0.011*"война" + 0.007*"любовь" + 0.007*"мочь" + 0.006*"человек" + ''0.006*"ляля" + 0.006*"сказать" + 0.005*"жизнь" + 0.004*"говорить" + '
'0.004*"год" + 0.004*"знать"'.
This means that the top 10 keywords that make up this theme are 'война', 'любовь', 'мочь', 'человек', etc. The weight of the word 'война' in topic 0 is 0.011.
The weights reflect how important the keyword is to that topic. 
The number of topics we want to extract from each set is given by us arbitrarily; in this case this number is ten.

Dataset is available here https://disk.yandex.ru/d/hcrrRc2GrNq2aA
