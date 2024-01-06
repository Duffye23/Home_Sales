# Home_Sales

The task for this challenge was to use pyspark in order to query a database and to ultimately see the difference in speed between cold calling, caching, and calling a parquet. Since I was having problems installing pyspark/java onto my personal machine Google Colab was used to run this challenge.

After importing the dependecies, I had to load the data from the aws server.
![image](https://github.com/Duffye23/Home_Sales/assets/58863493/f366d28a-5e48-4370-8257-d87b60e7ed0f)</br>

From there, there were a few practice queries before evaluating the same query with the use of cold calling from the database, calling from a cached view, and calling from a partitioned dataset. The difference in time was noticeable, and the difference would only grow with larger and larger datasets.</br>
Cold Calling the data:</br>
![image](https://github.com/Duffye23/Home_Sales/assets/58863493/3aa9ff5f-6f2c-48c5-aa98-424f4a32da56)</br>
![image](https://github.com/Duffye23/Home_Sales/assets/58863493/37d82d0b-22e8-4f14-ada9-be310ff9c345)</br>

Calling from a cached view:</br>
![image](https://github.com/Duffye23/Home_Sales/assets/58863493/ea7c115e-e3fe-41ac-8af1-5a26958e5095)</br>
![image](https://github.com/Duffye23/Home_Sales/assets/58863493/8ee0ac0d-8e04-4b21-b86a-4577b9c2df6b)</br>

Calling from a partitioned dataset:</br>
![image](https://github.com/Duffye23/Home_Sales/assets/58863493/2a875d16-e263-4716-afd8-e858d6991b6c)</br>
![image](https://github.com/Duffye23/Home_Sales/assets/58863493/49e19267-22cd-4a7d-b88b-f45328ee3c0a)</br>
![image](https://github.com/Duffye23/Home_Sales/assets/58863493/3b8ebf47-b951-43ca-bde0-01b43bac1ade)</br>

As can be seen, each new way to store the data leads to quicker calls. 

Sources used:
- Carleton Bootcamp zoom recordings and activities.
- AskBCS Learning Assistant for helping with Google Colab issues.
