# Slurm RPM Repository

## Slurm 22.05.8

Set the slurm repo file on CentOS 7:

```
sudo vi /etc/yum.repos.d/slurm.repo
```

Adding:

```
[slurm-22.05.8]
name=Slurm RPM Repository
baseurl=https://omnivector-solutions.github.io/slurm-repo/22.05.8/centos7/x86_64
enabled=1
gpgcheck=0
```

After that, install Slurm with yum:

Slurmdbd:

```
sudo yum install slurm slurm-slurmdbd -y
```

Slurmctld:

```
sudo yum install slurm slurm-slurmctld -y
```

Slurmrestd:

```
sudo yum install slurm slurm-slurmrestd -y
```

Slurmd:

```
sudo yum install slurm slurm-slurmd -y
```
