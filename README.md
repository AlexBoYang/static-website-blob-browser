---
services: storage
platforms: javascript
author: seguler
---

# Static Website Sample - File Browser app for Blob Storage 

This sample application can be used as a static website on Azure Storage to list the contents of a Blob container (anonymously). The project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app). The sample assumes your blob container is made public, however it can be modified to use Azure Active Directory authentication. The file browser also allows downloading each file with a single click.

## Pre-requsites
- Create an [Azure Storage account](https://ms.portal.azure.com/#create/Microsoft.StorageAccount-ARM.3.0.5) (GPv2) and enable [Static Websites](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blob-static-website)
- Install VSCode, and Azure Storage extension (optional)
- Install git

## Deploy the sample - step by step
Follow the following steps to deploy the sample on your Azure Storage account. Once deployed, the sample app will provide you a file browser view of your **$web** container. If you desire so, you can change the container in the `index.js` to any other public container.

- Clone the repository to your PC
`git clone https://github.com/seguler/static-website-blob-browser`
- Launch VS Code. Log on to the Azure Storage extension.
- Install create-react-app using a terminal (VSCode)
`npm install -g create-react-app`
- Open the sample in VSCode using `File>Open Folder` menu
- On the terminal, run `npm run build` to build the React app
- Right click `build` folder in VSCode, and click `Deploy to Static Website`
- Choose your storage account

![Blob browser - Static website](https://raw.githubusercontent.com/seguler/static-website-blob-browser/master/staticwebsitedemo.jpg)

## More information
- [Azure Storage SDK for JS](https://github.com/azure/azure-storage-js)
- [Static Websites on Azure Storage](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blob-static-website)
- [Deploy a Static Website with VSCode](https://code.visualstudio.com/tutorials/static-website/getting-started)