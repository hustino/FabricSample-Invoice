
Please visit the [installation instructions](http://hyperledger-fabric.readthedocs.io/en/latest/install.html)
to ensure you have the correct prerequisites installed. Please use the
version of the documentation that matches the version of the software you
intend to use to ensure alignment.

Source Code: J. Zarate
Modified by: J. Berango

Environment:
Host: Windows 8.1 Pro / i3-4130 CPU @ 3.40 GHz / 4 GB RAM / 500 GB HDD
Virtualization software: Oracle VirtualBox 5.22 
Oracle VirtualBox Guest Operating System: Ubuntu 18.0.4 
  Virtual Machine Set-up: 2GB RAM / 26 GB Storage
  
Before running/using the system, you must have this.

Operating Systems: Ubuntu Linux 14.04 / 16.04 LTS (both 64-bit), or Mac OS 10.12
Docker Engine: Version 17.03 or higher
Docker-Compose: Version 1.8 or higher
Node: 8.9 or higher (note version 9 and higher is not supported)
npm: v5.x
git: 2.9.x or higher
Python: 2.7.x
A code editor of your choice, we recommend VSCode

if you dont have this, you can follow this steps and install it in your machine
https://hyperledger.github.io/composer/latest/installing/installing-prereqs

Introduction about FabricSample-Invoice
 This project is all about solving the payment process of the 3 partcipants in the network(Bank, Supplier, OEM) using the Hyperledger   Blockchain platform
 How to use:
 
 1. Open your terminal, go the the folder cd /fabric-sample/basic-network/
 2. In your terminal, type ./teardown.sh after that ./start.sh
 3. Back in your terminal again, type cd .. and then cd fabcar
 4. Back to your terminal again, type this command. ./openScm.sh after that npm install (this will take a few minutes depending to your internet connection).
 5. After the npm install, type this enrollAdmin.js after it is done. Type enrollAdmin.js
 6. Lastly type app_scm.js
 7. Open your postman to interact.
 
 To post/insert a data in the network, in your psotman set the method to POST and in the url type localhost:3000/invoice
 below that go to Body tab and select x-www-form-url-encoded in the key column paste this values
 KEY              
 billedTo
 invoiceDate
 invoiceAmount
 itemDescription
 gr
 isPaid
 paidAmount
 repaid
 repaymentAmount
 supplier
 
 VALUES
 INV1
 (you can enter any ex Dell)
 (any data ex 2/14/19)
 (any amount you wanted)
 (you can enter any description ex XPS Dell)
 (Good received either yes or no)
 (if paid either yes or no) note the paid amount must always be less than the invoiceAmount
 (repaid either yes or no)
 (repayment amount to be always greater then paid amount)
 (you can type any supplier ex Microsoft)
 
 
 
