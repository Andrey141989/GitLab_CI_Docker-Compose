# -DevOps-GitLab_CI_With_Docker-Compose
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

*Also we need to prepare target system:*  
--allow multiple sessions  
*$ sudo vi /etc/ssh/sshd_config*  
*MaxSessions 128*  
*$ sudo systemctl restart sshd*  

--add privileges
$ sudo usermod -aG docker user  
$ sudo usermod -aG sudo user  
$ sudo chmod 666 /var/run/docker.sock  

