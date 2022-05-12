# Text Prediction using Sequential Models

___

### Problem
Text prediction models utilize Natural Language Processing and Machine Learning to predict the subsequent word(s) in a sentence. The user inputs a few words and the model predicts the words that are most likely to come after them. Text predicition models have a lot of use, depending on the industry and field they are employed in. They are quite ubiquitious and assist us on a daily basis, sometimes without us even realizing. If you go to Google and type in a few words in the search bar, Google's autofill feature completes the sentence for you without making you type all the words- saving you precious time. On gmail, the model learns your writing style from the emails that you send and over time starts reccomending words/phrases. Instead of you having to type "Dear Prof. Morales, I hope you're doing well!", all you have to do is start typing "Dear Prof..." and gmail does the rest for you- again saving a lot of time.

The biggest problem models like these solve is that of speed. Text prediciton models increase efficiency in different processes, thus increasing the speed with which people conduct business, talk to each other, and live their lives. As these models keep getting faster and more accurate, the ease in our interactions and communication keeps improving. In a sense, text prediction models increase the speed of development of our economies by allowing people to find the right information and connect with the right people in an appropriate and efficient manner.

___

### Data:
I wanted to takle this problem in a slightly different way. I wanted to create a model that would be personalized to me and my writing style. Thus, I trained the model on papers, emails, and creative writings (short stories, poems, incomplete long-er stories, etc.) that I have over time. I thought it would be interesting to teach the model my style. I put all the texts in one single document and imported it to Python using the textract package.

In addition to my personal texts, I also decided to include a text corpus from the nltk library: the WSJ articles corpus in order to increase the number of unique tokens and expand the scope of the model. I didn't do any preprocessing other than combining all texts, removing blank spaces and punctuation, and converting all words to lowercase. The final dataset had a total of 168,719 words, out of which 13,673 were unique.

___

### Model:
In order to build a text prediciton model, we need to use a sequential model because the sequence of the words matter. If we tokenized all words and just treated them as separate points, we would not be able to get a model that would be able to predict the subsequent words. The Sequential Deep Learning models that I use in this project allow the model to actually learn the "right" order of words to output when given any words.

My best model, Model 7, performed really high with an accuracy score of ~0.98. The model is very personalized to me . It outputs phrases that I could use in emails/cover letters and other pieces that I write in the future. When I input "My name is", it outputs "my name is shreyans kothari and i am a dual degree masters..", words I would definitely use in a sentence that begins with "My name is". Connecting this model (or a slighly better version) to an app like my email browser will allow me to increase efficiency in my work by automating mundane tasks like responding to emails.
