# End to end Text-Summarizer-Project

## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update entity
4. Update the configuration manager in src config
5. update the conponents
6. update the pipeline
7. update the main.py
8. update the app.py


# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/entbappy/End-to-end-Text-Summarization
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n summary python=3.8 -y
```

```bash
conda activate summary
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```


```bash
Author: Rounak Bhuiya

Email: rounakbhuiya@gmail.com

```



# AWS-CICD-Deployment-with-Github-Actions

Certainly, here are the steps broken down into very small points:

1. **Login to AWS Console.**

2. **Create an IAM User:**
   - Specify access for:
     1. EC2 (virtual machines).
     2. ECR (Elastic Container Registry).

3. **Create an ECR Repository:**
   - Save the ECR repository URI. 146937073414.dkr.ecr.eu-north-1.amazonaws.com/text-s

4. **Create an EC2 Instance (Ubuntu).**

5. **Install Docker on EC2:**
   - Update and upgrade (optional):
     - `sudo apt-get update -y`
     - `sudo apt-get upgrade`
   - Install Docker:
     - Download the script: `curl -fsSL https://get.docker.com -o get-docker.sh`
     - Execute the script:
       - `sudo sh get-docker.sh`
     - Add the user to the Docker group:
       - `sudo usermod -aG docker ubuntu`

6. **Configure EC2 as Self-Hosted Runner:** Set up as a GitHub Actions runner.

7. **Set GitHub Secrets:**
   - `AWS_ACCESS_KEY_ID`
   - `AWS_SECRET_ACCESS_KEY`
   - `AWS_REGION`
   - `AWS_ECR_LOGIN_URI`
   - `ECR_REPOSITORY_NAME`

These simplified steps should make it easier to follow the deployment process.