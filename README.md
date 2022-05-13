# -DevOps-GitLab_CI_With_Docker-Compose

This  is a manual how to build infrastructure for software development,
using GitLab for DevOps and Docker Compose as orchestrator.

Project has following files structure:
```bash
.
├── app
│   ├── Dockerfile
│   ├── app.py
│   └── requirements.txt
│   └── docker-compose.yml
├──.gitlab-ci.yml
```

*prepare target system:*  
 --allow multiple sessions  
*$ sudo vi /etc/ssh/sshd_config*  
*MaxSessions 128*  
*$ sudo systemctl restart sshd*  

 --add privileges  
$ sudo usermod -aG docker user  
$ sudo usermod -aG sudo user  
$ sudo chmod 666 /var/run/docker.sock  

--generate keys  
*$ ssh-keygen*  
*$ ssh-copy-id user@xxx.xxx.xxx.xxx*

