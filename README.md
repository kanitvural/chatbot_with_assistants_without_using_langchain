**.env contents**

```
OPENAI_API_KEY=

AIRTABLE_API_KEY=
```

**CRM Template**

https://airtable.com/apph7PZRJZdsP0Skw/shrHwajwaShy0IpjH

**AWS EC2 Setup**


```
ssh -i rag.pem ec2-user@ec2_ip

sudo dnf update -y
sudo dnf install git python3.11 python3.11-pip -y

git clone https://github.com/kntvrl/chatbot_with_assistants_without_using_langchain.git

cd chatbot_with_assistants_without_using_langchain


python3.11 -m venv venv

source venv/bin/activate

pip install -r requirements.txt

nano .env

nohup python3 main.py
```
