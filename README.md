# Executing Ray on the Slashbin Cluster

ray-on-slashbin.ipynb notebook provides a simple example of how to run a distributed Ray application our cluster.

## How to view the notebook remotely

1. Install [sshuttle](https://github.com/sshuttle/sshuttle) locally
2. Connect to the cluster with sshuttle (e.g. `sshuttle -NHr --dns slashbin`*)
3. Open a new terminal window and ssh to the login node (e.g. `ssh ct01`)
4. Clone this repository (`git clone https://github.com/ValHayot/slashbin-ray`) and cd to it
5. Create a virtual environment which will contain Jupter and all the other libraries installed within the notebook (e.g. `python3.8 -m venv venv`)
6. Source the virtual environment (e.g. `source venv/bin/activate`)
7. Install jupyter (`pip install jupyterlab`)
8. Start Jupyter `jupyter lab`
9. On a local browser window, enter the Jupyter URL provided. Should be something along the lines of `http://ct01:8888/lab?token=<your token>`
10. Open the notebook `ray-on-slashbin.ipynb` and execute!

***Note**: `slashbin` in step 2 assumes you ssh config is formatted as specified in the [lab website](https://big-data-lab-team.github.io/get_start.html#labcluster)