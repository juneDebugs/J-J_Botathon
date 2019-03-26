# Create Your Bot Using C# & Node.js
## Prerequisites
- [ x ] Check Visual Studio 2017
- [ x ] Install Bot Emulator
- [ x ] Install Azure CLI
- [ x ] Setup Node.js (If Applicable)
- [ x ] (Optional) Python Configuration
## Environment Setup
## Visual Stuido Setup
1. Run `NDP471-DevPack-ENU.exe` as Administrator. This will Install the .NET SDK and Dependencies. 
2. Run `vs_community.exe` as Administrator, click modify, then ensure the packages shown in the image below are installed. if they are not, check them and click *Modify* in the bottom right.  
![Displays Modify Options in the installer](https://i.imgur.com/DVESxBn.jpg)  
After Modify Has Been Clicked, select these packages and select "Modify" in the Bottom Right. 
![Package to Check](https://i.imgur.com/AZ6lw1a.jpg)  
## Ngrok, Bot Emulator & Azure CLI
3. Navigate to *ngrok\ngrok-stable-windows-amd64* and run `ngrok.exe` as Administrator.  
4. Navigate to *\bot emulator* and run `botframework-emulator-3.5.37-windows-setup.exe` as Administrator.  
5. Run `azure-cli-2.0.59.msi` as Administrator

## Setup Node.js (Skip This If You Are Not Using Node.js)
1. Open MS PowerShell
2. Using `mkdir` and `cd` navigate to your projects directory, make sure the included `package.json` is in that directory.
3. Run `npm install --global`. This will take a few minutes. Read over the listed packages in this document and familiarize yourself with the documentation if you need to. 
4. Install any additional package locally that you will need for your technical stack. Included below are soem Microsoft recommended packages for Azure services, make sure to only install the ones to need to avoid conflicts.  
`npm install luis-apis`  
`npm install botdispatch`	
`npm install qnamaker`   
  
## Configuring Python (Optional)
For this competition, we recommend using the included Visual Studio, but you are free to develop in whatever you choose. 
**Adding Python to VS**:  
1. set these environment paths in Visual Studio 2017 Community, navigate to Tools > Python Tools > Python Environments. Then select + Custom.
2. Anaconda `Python 3.6` is installed under `C:\Anaconda`. Anaconda `Python 2.7` is installed under `c:\Anaconda\envs\python2`. 
*Developers may need to run “activate python2” command to bring up  Python2 runtime if they are more familiar working in Python 2.x*

## Samples
Bot Builder also provides several samples organized per SDKs with a suggested reading order.
`https://github.com/Microsoft/BotBuilder-Samples/tree/v3-sdk-samples`  
Run the following commands to download the sample code.  
`git clone https://github.com/Microsoft/BotBuilder-Samples.git`  
`cd BotBuilder-Samples`  
`git checkout v3-sdk-samples`  
**Note:**  
- The node.js version of samples require Python distributions 2.7. Developers need to run “activate python2” command to bring up  Python2 runtime for node.js samples.

- Tunneling (ngrok): The Bot Framework Emulator integrates tightly with ngrok, if you're running the Bot Framework Emulator behind a firewall or other network boundary. Developers need to follow up the following link to install and configure tunneling software.

- [Ngrok Wiki](https://github.com/Microsoft/BotFramework-Emulator/wiki/Tunneling-%28ngrok%29 "Ngrok Wiki")
- [Bot SDK V. 3](https://docs.microsoft.com/en-us/azure/bot-service/?view=azure-bot-service-3.0)

## Resources
 
- [Azure BotBuilder Documentation](https://github.com/Microsoft/BotBuilder-V3)

- [BOT SDK Documentation](https://docs.microsoft.com/en-us/dotnet/api/?view=botbuilder-dotnet-3.0)

- [Adaptive Cards](https://adaptivecards.io/)

## Logging into your VM
1. [Your Azure Portal](portal.azure.com)  
![Portal Picture](https://i.imgur.com/pOnm1md.jpg)  
2. Click on Virtual Machines and click on your machine  
![Finding your VM](https://i.imgur.com/LEbPizf.jpg)  
3. Click Connect  
![Clicking Connect](https://i.imgur.com/BVMM8sn.jpg) 
4. Click Download RDP File  
![Downloading RDP File](https://i.imgur.com/dXbxW9A.jpg)



## License
[MIT](https://choosealicense.com/licenses/mit/)
