python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
pip freeze > requirements.txt
docker build -t test . 
docker run -p 5000:5000 test
ssh-keygen #enter
cat ~/.ssh/id_rsa.pub
#zkopirovat otisk klice do githubu -
profile>settings>ssh&gpg key