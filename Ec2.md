Certainly! Below is the `README.md` file for hosting a simple Node.js application on an AWS EC2 Ubuntu machine.

```markdown
# Node.js Hello World

This is a simple Node.js app that serves "A Monk in Cloud". It's great for testing simple deployments on the cloud.

## Step 1: Install Node.js and NPM using nvm

Install Node Version Manager (nvm) by typing the following at the command line:

```sh
sudo su -
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```

Activate nvm by typing the following at the command line:

```sh
. ~/.nvm/nvm.sh
```

Use nvm to install the latest version of Node.js by typing the following at the command line:

```sh
nvm install node
```

Test that node and npm are installed and running correctly by typing the following at the terminal:

```sh
node -v
npm -v
```

## Step 2: Install Git and Clone Repository from GitHub

To install git, run the below commands in the terminal window:

```sh
sudo apt-get update -y
sudo apt-get install git -y
```

Verify if the system has git installed by running the below command in the terminal:

```sh
git --version
```

This command will print the git version in the terminal.

Run the below command to clone the code repository from GitHub:

```sh
git clone https://github.com/yeshwanthlm/nodejs-on-ec2.git
```

Get inside the directory and install packages:

```sh
cd nodejs-on-ec2
npm install
```

## Step 3: Start the Application

To start the application, run the below command in the terminal:

```sh
npm start
```

## Conclusion

This README.md file guides you through the steps to host a new Node.js project on an AWS EC2 Ubuntu machine.
```

Replace the `nodejs-on-ec2` GitHub URL with your own repository if needed. This README.md file provides a clear step-by-step guide to set up and run your Node.js application on an AWS EC2 Ubuntu machine.