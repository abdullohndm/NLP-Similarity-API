# RESTful API For Similarity Check Using Natural Language Processing

### Documents similarity
Document similarity (or distance between documents) is a one of the central themes in Information Retrieval. How humans usually define how similar are documents? Usually documents treated as similar if they are semantically close and describe similar concepts. On other hand “similarity” can be used in context of duplicate detection. We will review several common approaches.

#### OBJECTIVE
The objective of this API is to handle Similarity of text

## API ARCHITECTURE
|RESOURCES |URL(PATH) |METHOD |PARAMETERS |STATUSCODE|
|----------|-------|--------|--------------|----------|
|Register a user | /register | POST | username, password | 200:OK,  301:INVALID USERNAME |
|Detect Similarity of docs | /detect | POST | username, password , text1 & text2 |200:OK RETURN SIMILARITY ,   301:INVALID USERNAME,    302:INVALID PASSWORD,    303:OUT OF TOKENS
|Refill | /refill | POST | username,  admin_pw,  refill_amount |  200:OK,  301:INVALID USERNAME , 304:INVALID ADMIN_PW


## REQUIREMENTS

- [Spacy.io](https://spacy.io/models/en)

- [Spacy Model](https://github.com/explosion/spacy-models/releases//tag/en_core_web_sm-2.1.0)

- [Flask framework](https://github.com/pallets/flask), for more [Details](https://www.fullstackpython.com/flask.html)

- [PyMongo](https://api.mongodb.com/python/current/)

- [Docker](https://www.docker.com/) and Docker-compose.yml
