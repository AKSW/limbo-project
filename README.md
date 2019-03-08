# limbo-project
This a repository of the LIMBO project https://www.limbo-project.org/

It contains the dataset descriptions environment for hosting on a linux server and using datasets from https://gitlab.com/limbo-project

ATM I get 
```
2019-03-08 15:25:01,140 - quit - INFO - QuitStore Configuration initialized.
Traceback (most recent call last):
  File "./quit/run.py", line 15, in <module>
    objects = initialize(parsedArgs)
  File "./quit/application.py", line 117, in initialize
    logger.debug('Path of Gitrepo: ' + config.getRepoPath())
TypeError: can only concatenate str (not "NoneType") to str
unable to load app 0 (mountpoint='') (callable not found or import error)
*** no app loaded. going in full dynamic mode ***
*** uWSGI is running in multiple interpreter mode ***
```
