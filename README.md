# vsc-tutorial

This is a tutorial on how to use the vsc-connector.
It assumes you have already set up your VSC account and ran `vsc.py` with the ``--setup`` argument.

## 1. Setting up the config
1. Please copy ``configs/config.yaml`` into this folder. (The configs dir is located in the dir above)
2. Then, open the ``config.yaml`` file 
3. Edit the ``src_dir`` variable to the current path of this dir (on linux you can get this with the command ``pwd``) + either ``/0-pytorch`` or ``/1-tensorflow``.
   Example: ``/Users/thierryderuyttere/Documents/vsc-connector/vsc-tutorial/0-pytorch``
   
## 2. Running the config file
exectue ``python vsc.py run-experiment <path_to_config>`` where ``<path_to_config>`` is the path to the config from step 1.
Executing this command should give you a `job-id`. 
Please store it somewhere! In case you would forget it, you can always run ``python vsc.py get-stats`` to display all your submitted/running tasks on the VSC.

And that's it! You should now have a submitted job on the VSC!