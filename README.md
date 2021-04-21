# sagemaker-tutorial

AWS tutorial on building, training and deploying a ML model using SageMaker.

This tutorial is at https://aws.amazon.com/getting-started/hands-on/build-train-deploy-machine-learning-model-sagemaker/

Instructions to associate a Git repository with SageMaker notebook instances at https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html

## Create an Amazon SageMaker notebook instance

1. Sign in to the console: https://console.aws.amazon.com/sagemaker/ with your account ID, IAM user and password. Select your preferred region (e.g. `us-east-1`).
2. On the left pane, select **Notebook** -> **Notebook instances** -> **Create notebook instance**.
3. On the **Create notebook instance** page: enter a name, choose type (`ml.t2.medium`) and for **Elastic inference** choose 'None'.
4. On the same page, in the **Permissions and Encryption** section, for IAM role choose 'Create new role'. In the box that appears, select 'Any S3 bucket' (unless you already have a bucket that you'd like to use - in that case choose 'Specific S3 buckets' instead). Click 'Create role' -> SageMaker creates a role with a name like `AmazonSageMaker-ExecutionRole-###`.
5. Associate a Git repository: in the **Git repositories** section, you can select to clone a public repository, add a repository to SageMaker or choose a repository previously added.
6. Keep all other settings at their default values and click 'Create notebook instance'.
