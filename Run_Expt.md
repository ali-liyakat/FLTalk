# How to RUN the FLTalk
        <For Local testing>

        Check the MAIN_SERVER_URL in app.js, experiment.html and experiment.js files  (keep local server url)
        Start front end in browser (index.html)
            Go to Run Experiment Tab and keep desired number of clients
        Start FLTalk Main server from Backend (FLTalk_Server.py) (uvicorn FLTalk_Server:app --reload)
        Go to client_agent and server_agent files and check the SERVER_URL there (set to local server url)
        Go to federated_server.py, choose No. of clients, Rounds and Aggregation Algorithm
        Go to federated_client.py files and choose configs(like Model, Dataset, etc). Keep ROUNDS same as federated_server

        Run Federated server (python federated_server.py)
        Run Federated Clients (federated_client.py)


# How to run the FedDeepSMOTE Experiment.

--> 1:- Running Local DeepSMOTE Experiment:

            Run Local FedDeepSMOTE for all clients  (python localdeepsmote_train.py)
            Run Data Generation Files for all clients  (localdeepsmote_generate.py)


--> 2:- Running FedDeepSMOTE Experiment:

            (If Local Testing) Start FLTalk Main server from Backend (FLTalk_Server.py) (uvicorn FLTalk_Server:app --reload)

            Run FedDeepSMOTE Server file from FLTalk_Server folder  (python feddeepsmote_server.py)
            Run FedDeepSMOTE clinet files for all clients (python feddeepsmote_client.py)
            Run data generation files for all clients (GenerateSamples.py)
            Run Evaluate CNN files from all clients  (evaluate_CNN.py)