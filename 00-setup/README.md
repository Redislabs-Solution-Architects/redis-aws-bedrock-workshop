# SetUp your Redis Environment (< 10 minutes)

This notebook serves as a guide for setting up a Redis environment, including creating a Redis Cloud subscription, configuring a database, and installing RedisInsight Desktop for database management. 

It also provides instructions for preparing the Python environment for the workshop by installing the required packages and setting up the connection to the Redis database.

## 1. Sign up for Redis Cloud trial

Visit [https://redis.com/try-free/](https://redis.com/try-free/) and sign-up for a free trial:

![alt_text](images/image1.png "Redis Cloud")

## 2. Verify your account via email

![alt_text](images/image2.png "Verify your account via email")

## 3. Login with your new credentials

![alt_text](images/image3.png "login with your new new credentials")

## 4. Click "+ New Subscription" to add a new subscription to your account

![alt_text](images/image4.png "new subscription")

## 5. Choose a free Fixed plan with your preferred cloud provider and region

![alt_text](images/image5.png "free fixed plan")

## 6. Name your subscription and click "Create Subscription"

![alt_text](images/image6.png "name your subscription")

## 7. Create a new database under your subscription

![alt_text](images/image7.png "create a new database")

## 8. Name your database and select type "Redis Stack"

![alt_text](images/image8.png "select redis stack")

## 9. Set a password for your database

![alt_text](images/image9.png "set a password")

## 10. Activate your new database

![alt_text](images/image10.png "activate your database")

## 11. Download RedisInsight Desktop on your laptop

![alt_text](images/image11.png "download & install redisinsight")

## 12. Install RedisInsight Desktop on your laptop

![alt_text](images/image12.png "install RedisInsight")

## 13. Open RedisInsight Desktop and add a new database

![alt_text](images/image13.png "add a new database")

## 14. Copy the URI details of your new database and paste it in RedisInsight

![alt_text](images/image14.png "copy URI")

![alt_text](images/image15.png "Paste URI")

## 15. Your Redis database is now added and ready to use

![alt_text](images/image16.png "database added")

## 16. Your environment is prepared for the workshop labs

![alt_text](images/image17.png "environment ready")

## 17. Python Setup

### Virtual Environment

```bash
python3 -m venv .venv
source ./.venv/bin/activate
pip install redis
```

### Modules Needed

``` python
from redis import from_url
```

### Connect Client

```python
        user = 'your user'
        pwd = 'your password'
        url = 'your url'
        port = 'your port'
    
        client = from_url(f'redis://{user}:{pwd}@{url}:{port}')
        print(client.ping())
```

### Result

```bash
True
```