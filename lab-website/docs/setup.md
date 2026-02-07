## For local development on windows 10/11:
### 1. Requirements:
- Python 3.10+
- Git
- Node.js (for frontend)
- pip

### 2. Clone the repository
```
git clone https://github.com/Yash-1-tech/Team-Daedalus-Lab.git
cd lab-website
```

### 3. Backend setup
#### Enter backend folder
```
cd backend
```
#### Create virtual environment (first time only)

Windows powershell:
```
python -m venv venv
```
Run the activation script:
```
.\venv\Scripts\Activate.ps1   
```
You should see (venv) in your terminal.

visit [Help with venv-stackoverflow](https://stackoverflow.com/questions/1365081/virtualenv-in-powershell) if you run into any errors! 

### NOTE: Activate the virtual environment each time you restart the terminal.

#### Install dependencies
```
pip install -r requirements.txt
```

### 4. Environment variables
Create a .env file in the project root.

You can copy the example:
```
cp .env.example .env
```

### 5. Run migrations
```
rav run migrate
```

### 6. Start the backend server
From the project root ( /lab-website ):
```
rav run server
``` 
Server will run at:
```
http://127.0.0.1:8001
```

### 7. Django admin
``` 
http://127.0.0.1:8001/admin
```

### 8. Common commands

Run from project root:
```
rav run server          # start dev server
rav run migrate         # apply migrations
```

### 9. Troubleshooting
#### Q. Command not found?

Make sure venv is activated.

#### Q. Port already in use?

Kill other Django instances or change port.