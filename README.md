# Slurm RPM Repository

## Slurm 25.05.1

Set the slurm repo file on Rocky Linux 9:

```
sudo vi /etc/yum.repos.d/slurm.repo
```

Adding:

```
[slurm-25.05.1]
name=Slurm RPM Repository
baseurl=https://omnivector-solutions.github.io/slurm-repo/25.05.1/rocky9/x86_64
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
