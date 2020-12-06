# BD_0087_0196_0230_0252_Project
<h2>Folder Structure</h2>
 - src

    - Master.py
  
    - Worker.py
  
    - Analysis.py
    
    - config.json and requests.py 
  
-logs

    - log_RR.txt
  
    - log_LL.txt
  
    - log_RA.txt
  

<h3>Steps to run:</h3>

- Run the Master.py with command 
 ```python
    $ python3 Master.py <Config.json> <Scheduling Algo(RR/LL/RA)>
  ```
 - Run three workers with the following commands
 ```python
    $ python3 Worker.py <port[4000/4001/4002]> <worker_id[1/2/3]>
 ```
 - Then run the requests.py to generate task queue
 ```python
    $ python3 requests.py <no_of_requests>
 ```
- 3 log files are then created and Analysis.py helps in analysing them. To run it
 ```python
    $ python3 Analysis.py
 ```
 
 #The logs folder contains logs generated in our tests. U could as well use them to process the analysis.py.
