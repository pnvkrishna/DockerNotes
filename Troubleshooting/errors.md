## Error1 

![useradd to docker group](Images/Docker1.png)


* “Why did you get docker.sock permission denied?”
    - Answer: “Because my user was not part of the docker group. Docker daemon runs as root, so non-root   users must be added to the docker group to access it.”