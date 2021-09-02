# python_blockchain_app

This application creates transactions, and once you mine the transactions, all the nodes in the network update the chain. The chain of the nodes can also be inspected by inovking `/chain` endpoint using cURL.

## Instructions to run

Clone the project,

```sh
$ git clone https://github.com/bshivam2001/BlockchainApp.git
```

Install the dependencies,

```sh
$ cd python_blockchain_app
$ pip install -r requirements.txt
```

Start a blockchain node server,

```sh
# Windows users can follow this: https://flask.palletsprojects.com/en/1.1.x/cli/#application-discovery
$ export FLASK_APP=node_server.py
$ flask run --port 8000
```

One instance of our blockchain node is now up and running at port 8000.


Run the application on a different terminal session,

```sh
$ python run_app.py
```

The project is designed to be beginner friendly.
There are some conscious trade-offs that we've made to keep it simple.