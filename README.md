# SMS_SpamDetector
Built a ML model using SVM to classify SMS messages as spam or ham (not spam). 
Email spam is usually different from SMS message spam; we tend to speak more casually on our phones, using more slang, incomplete sentences or even concocting words and phrases.
We used a public dataset available on the UCI ML repository consisting of 5572 messages, of which 4852 are labelled ham and 747 are labelled as spam messages.

Used RegEx to identify patterns such as email address, phone numbers, currency symbols, URL's in the SMS text and normalize them. Removed stop-words, performed Stemming using the
NLTK library, and used sklearn's TfidfVectorizer to generate n-grams.

Achieved a F1-score of 92% using SVM. Due to the class-imbalance in the dataset, recall for the 'Spam' class (87%) is much lower than than that for 'non-spam' (99.9%)

