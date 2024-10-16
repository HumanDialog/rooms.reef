# <img src="https://objectreef.dev/reef.png" width="25" />  Rooms booking app
This is simple demonstration application made with ObjectReef technology. Although it is very simple and does not contain much source code, it meets the requirements of a complete and functional service. The sample is released under the terms of the MIT license, the content of which you can find [here](./LICENSE.md).

**NOTE:** This is only backend part of the application. Frontend can be found at:
- [Rooms booking app (Svelte)](https://github.com/HumanDialog/rooms.svelte)

## Service launch
The most convinient way to develop ObjectReef solutions is to use [Visual Studio Code](https://code.visualstudio.com/) with [Reefs Language support extension](https://marketplace.visualstudio.com/items?itemName=humandialog.object-reef).

To run the service on the local machine, type the following command at the command line in the project directory:  
`reef dev`  

The first time you use it, or after a long break, ObjectReef may ask you for credentials to install the certificate you need to use ObjectReef on your local machine.

ObjectReef will try to start the web service by opening an unsecured port **1996**. If the port is not used by any other process, then the message `local service:  http://localhost:1996/` will appear, indicating that the service is ready for use and the running `reef dev` process is in interactive mode.

Before we move on to testing, the source code still needs to be compiled, so let's type:  
`build`  
or press `Ctrl+Shift+B`

This command reads the project settings file **.refs** and all source files with extension **.reef**. The compiler creates intermediate executable code, executed by ObjectReef run-time environment.  

Although the application model is ready the service does not have any data yet. We can quickly fix this by calling the operation:  
`app/InitSample`

At the end of the preparation, it is worth saving the data just created, so as not to call  this operation in the future.  
`sys/save`

Now that our service is ready to use, you can send HTTP requests to it using any client, i.e. cURL, Postman or using one of the sample fronteds listed above.

## About ObjectReef
ObjectReef is a complete platform to design, test and deploy any high performance backend service. It ensures robust, scalability and security with zero tech debt. That Low Code Backend as a Services (BaaS) solution offers you everything you need to develop, maintain, integrate and run the software without the advanced technical knowledge.

No matter, if you are creating the simple or complex and critical product, ObjectReef is the platform, that simplifies the process of delivering the application backend. It has never been so quick and so robust.

More info you'll find at [https://objectreef.dev/](https://objectreef.dev/)

 