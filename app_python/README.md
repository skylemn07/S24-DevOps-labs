## Moscow Time Flask Web Application Documentation

### Description
The Moscow Time Flask Web Application is a simple web application that displays the current time in Moscow. The application is built using the Flask web framework.

### Installation
To install the application, you will need to have Python and pip installed on your system. You can then install the application using the following command:

- Clone the repository
- Install the requirements
- Run the application

```bash
cd app_python
pip install -r requirements.txt
python main.py
```

### Unit Test
To run the tests, you can use the following command:

```bash 
python app-test.py
```

### Docker
- How to build?

```bash
docker build -t skylemn07/app .
```
- How to pull?

```bash
docker pull skylemn07/app:latest
```
- How to run?

```bash
docker run -p 5000:5000 --name app skylemn07/app:latest
```
After running the command, you can access the application by visiting `http://localhost:5000` in your web browser.

### Visits
The service counts the numbers of visits. It can be accessed via following command:
```
% curl http://127.0.0.1:5000/visits
{
  "visits": 3
}
```
### Stack
- Python
- Flask
- HTML
- Docker