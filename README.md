# A Serverless Rust API on AWS

###What do you need?

####Rust

To run Rust code locally, compile and create the binary file we need, you must have Rust installed.

For Unix based systems, rustup is recommended.

Run the following command in your shell:
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

---
####AWS Account

You can create a free tier account on AWS Website.

---
####AWS and SAM CLIs

To make it easier to deploy our code and create the needed AWS resources we need both [AWS](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) and [SAM](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html) CLIs installed.

Follow the instruction on the links to install them and then [configure](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html) your AWS CLI.

---
####Docker

Docker is needed if you are not running Linux. This project was created on MacOS and uses Docker and we're assuming you do too.

---

## Deploying the project to AWS

Log in to AWS Console with your account, create a new S3 bucket and change the name on the "package" command inside Makefile in the root of the project to the name of your bucket.

To deploy everything to AWS, simply run `make deploy` and wait until it's finished!

