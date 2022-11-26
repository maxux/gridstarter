# gridstarter

## install 

```bash
curl https://raw.githubusercontent.com/despiegk/gridstarter/main/scripts/install.sh > /tmp/install.sh && bash /tmp/install.sh

#if you want to debug do
curl https://raw.githubusercontent.com/despiegk/gridstarter/main/scripts/install.sh > /tmp/install.sh && bash -x /tmp/install.sh
```

## install on remote server over ssh

You need ssh-key loaded in ssh-agent

```bash
#add your ip addr here
export ME='195.192.213.92'

#do the install
ssh -A root@$ME "curl https://raw.githubusercontent.com/despiegk/gridstarter/main/scripts/install.sh > /tmp/install.sh && bash -x /tmp/install.sh"

#to login to your machine
ssh -A root@$ME

#to reset all (same as install but will restart)
ssh -A root@$ME "export RESET=1 && curl https://raw.githubusercontent.com/despiegk/gridstarter/main/scripts/install.sh > /tmp/install.sh && bash -x /tmp/install.sh"

```
