# Information

You have 3 accounts, please make sure to use the correct account:
- FZI: XXX@fzi.de, for VPN, e-mail (if it doesn't work, try with/without `@fzi.de`)
- Server: Ubuntu user on specific server, e.g. `ipe-monster`. Can only be used to connect to server
- Gitlab: Credentials to access the Gitlab https://ipe-wim-gitlab.fzi.de/

You can use the following services
- Cloud: https://cloud.fzi.de/
- Mail: https://mail.fzi.de/


## Using Servers

- Main GPU server `ipe-monster.fzi.de` with credentials provided by Laura Doerr/Lucas Cazonelli. Note: this account has no relation to your FZI account!
- Connect to server using VS Code: Explained in this [video](https://www.youtube.com/watch?v=y9iM0lYAQD0)
- Or connect directly via `ssh`: `ssh USERNAME@ipe-monster.fzi.de`

### Create Virtual Environment

```
pip install virtualenv
virtualenv -p /usr/bin/python3.9 YOUR_ENV_NAME
source YOUR_ENV_NAME/bin/activate
```

### Using GPUs

please **always** use only a single GPU by pasting (at the very top of the file)
```
import os
os.environ["CUDA_VISIBLE_DEVICES"] = "2"  # use 2, 3, 4 or 5
```
check usage of current GPU with (only use free GPUs)
```
nvtop
```
and check if GPUs are blocked/reserved [here](https://cloud.fzi.de/apps/onlyoffice/85194?filePath=%2Fipe-computing-resources.xlsx)

### Using Sessions

To detach a session, you can use `tmux`. This allows you to continue training without an active `ssh` connection to the server.
```
tmux new-session -s training1
```
check sessions with
```
tmux ls
```
attach exisiting session
```
tmux attach -t training1
```
