# microsoft-sample-app-azureAD-DT

Here is the sample build.gradle file to build out the sample app from: 
https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-v2-android#how-the-sample-works

follow steps above and then copy the build.gradle file in this repo into android studio to instrument the app with Dynatrace. You can capture user calls through the emulator also.

![image](https://user-images.githubusercontent.com/21251848/114133333-c3b9ba00-98ba-11eb-9393-0e0a21c2ff98.png)


Basically this app will make a graph API call through azure AD using an existing login through android and then pull back your AD info into the app. the build.gradle file has the necessary Dynatrace instrumentation to actually instrument the app and then have those calls show up in your Dynatrace tenant: 
https://www.dynatrace.com/support/help/technology-support/operating-systems/android/instrumentation-via-plugin/instrumentation-via-plugin/

FYI this is using groovy NOT kotlin you can see below the azure AD calls and response time:

<img width="1177" alt="Screen Shot 2021-04-08 at 10 40 50 PM" src="https://user-images.githubusercontent.com/21251848/114133807-7ab63580-98bb-11eb-8066-44982d3baafe.png">

<img width="1192" alt="Screen Shot 2021-04-08 at 10 36 22 PM" src="https://user-images.githubusercontent.com/21251848/114133392-dc29d480-98ba-11eb-9fd2-bcc784401f24.png">

