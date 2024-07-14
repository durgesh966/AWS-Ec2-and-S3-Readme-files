This is the updated `README.md` file with instructions to add an inbound rule to your AWS EC2 security group.

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
apt-get update -y
apt-get install git -y
```
OR

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

## Step 3: Configure AWS EC2 Security Group Inbound Rules

To allow inbound traffic to your Node.js application, you need to add an inbound rule to your EC2 instance's security group.

1. Go to the [AWS Management Console](https://aws.amazon.com/console/).
2. Navigate to the EC2 Dashboard.
3. In the left-hand menu, click on `Instances` and select your instance.
4. In the Description tab, find the `Security groups` and click on the security group associated with your instance.
5. In the security group details, go to the `Inbound rules` tab and click on `Edit inbound rules`.
6. Click on `Add rule` and set the following values:
    - **Type:** Custom TCP
    - **Protocol:** TCP
    - **Port range:** 3000 (or whichever port your Node.js app is running on)
    - **Source:** Custom (0.0.0.0/0 to allow traffic from anywhere, or specify an IP range)
7. Click on `Save rules`.

## Step 4: Start the Application

To start the application, run the below command in the terminal:

```sh
npm start
```

## Conclusion

This README.md file guides you through the steps to host a new Node.js project on an AWS EC2 Ubuntu machine, including setting up necessary inbound rules in the security group.
```

This updated README includes the steps to configure inbound rules for your EC2 instance, ensuring that your Node.js application can be accessed over the network.