# fast-api-token-authentication(jwt token)

This project demonstrates use of jwt token for authentication.



Project Setup

##  1. Clone the Repository

```bash
git clone https://github.com/PhoebeMarcie/jwt-token-fast-api.git

cd jwt-token-fast-api
```
## 2. Create Virtual Environment.

On Windows:

```bash
py -m venv .venv
.venv\Scripts\activate
```
On macOS/Linux:
```bash
python3 -m venv venv
source venv/bin/activate
```
## 3. Install dependencies
```bash
py -m pip install -r requirements.txt  

or 

pip install -r requirements.txt

```
## 4. Start Project
```bash
uvicorn main:app --reload
```

## 5. Additional steps
1. Generate encryption key 
```bash
openssl rand -hex 32
```
and add it to SECRET_KEY in main.py

2. Generate password hash(Since we're using a dummy use and not a real db.)

```bash
uncomment within code and run python program. 
pwd = get_password_hash()
print(pwd)
```
add pwd hash to hashed_password
and then re-comment out 


## 6. Api Documentation

Accesed on:

[http://127.0.0.1:8000/docs#/](http://127.0.0.1:8000/docs#/) or [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)


##
## N/B This is not production type of code