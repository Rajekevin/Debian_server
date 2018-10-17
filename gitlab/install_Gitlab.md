## Install Gitlab Server on Debian 9


###  Install and configure the necessary dependencies
```bash
sudo apt-get update
sudo apt-get install -y curl openssh-server ca-certificates
```

```bash
sudo apt-get install -y postfix
```

### Add the GitLab package repository and install the package
```bash
curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.deb.sh | sudo bash
```

### Change `http://gitlab.example.com` to the URL at which you want to access your GitLab instance. 
```bash
sudo EXTERNAL_URL="http://gitlab.example.com" apt-get install gitlab-ee
```

# Ressource
https://about.gitlab.com/installation/#debian

