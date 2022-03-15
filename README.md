# Practicum Project 3

## From Portland to Portland

This is a responsive, single page website about a coast-to-coast trip of the US.

### [Deployed site](https://deserie-portland-to-portland.netlify.app/)

---

## Pipeline with Packer by HashiCorp, Ansible, GitHub Actions

1. Created a Packer template (aws-ubuntu.pkr.hcl) that builds a t2.micro Amazon EC2 AMI. I added 2 provisioners to the build block, the first being a shell provisioner that installs Ansible, and the next one runs the Ansible playbook (ansible_playbook).yml.

2. Inside my terminal I had to first authenticate to AWS using my credentials, then ran the following commands to actually build the AMI:

```
packer init .
packer fmt .
packer validate .
packer build aws-ubuntu.pkr.hcl
```

---

![](/images/pkr-1.png)

---

![](/images/pkr-2.png)
