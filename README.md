# Network3-Node

1.Create a Network 3 account. I will appreciate it if you create one using my referral link below.

  https://account.network3.ai/register_page?rc=081b3da7

2. Connect to your VPS server and update the Ubuntu Operating system

~~~~
sudo apt update && sudo apt upgrade -y
~~~~

3. Install Required Applications

You’ll need to install a few essential applications for managing your node. Execute the following commands:
~~~~
sudo apt install -y screen net-tools
~~~~
4. Download the Network 3 Node Software

Next, download the Network 3 node software using the appropriate link. The download link may vary depending on the latest version available. Follow these steps to get the correct link:

    1.Visit the Network 3 download portal.
    2.Locate the “Linux Download” button.
    3.Right-click the “Linux Download” button and select “Copy Link Address.”
    4.Replace the URL in the wget command below with the one you copied.

Example link for downloading version 2.1.0:
~~~~
wget https://network3.io/ubuntu-node-v2.1.0.tar
~~~~
5. Extract the Downloaded Software

After downloading, extract the software archive using the following command:
~~~~
tar -xvf ubuntu-node-v2.1.0.tar
~~~~
6. Create a Screen Session for Network 3

To keep your node running in the background, create a screen session named “Network3”:
~~~~
screen -S network3
~~~~
7. Navigate to the Application Directory

Move into the directory where the application was extracted:
~~~~
cd ubuntu-node
~~~~
8. Start the Network 3 Node Application

Start the node application with the following command:
~~~~
sudo bash manager.sh up
~~~~
If everything is set up correctly, you should see a message indicating that the node is running.

9. Retrieve Your Node’s Secret Key

To link your node to your Network 3 account, you’ll need the node’s secret key. Retrieve it using this command:
~~~~
sudo bash manager.sh key
~~~~
Copy this key and store it in a safe location.

10. Link the Node to Your Network 3 Account

1. Log in to your Network 3 account via the dashboard.

2. After logging in, enter the following URL in your browser, replacing xx.xx.xx.xx with the IP address of your VPS server:
  https://account.network3.ai/main?o=xx.xx.xx.xx:8080

3. Once the page loads, click the “+” symbol to add your node.

4. When prompted, enter the secret key you retrieved earlier.

If the process is successful, you will receive a notification confirming that the miner has been successfully added to your account.

11. Manage the Screen Session

To minimize the screen running your verifier node:

Press `Ctrl + A`, then `D`.

To re-enter the screen session:
~~~~
screen -r network3
~~~~
Congratulations!

You have successfully set up your Network 3 node. You should begin to see rewards reflected on your dashboard shortly.

Link to Official guide from Network3
