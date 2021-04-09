# microsoft-sample-app-azureAD-DT

Here is the sample build.gradle file to build out the sample app from: 
https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-v2-android#how-the-sample-works

Basically this app will make a graph API call through azure AD using an existing login through android and then pull back your AD info into the app. the buold.gradle file has the necessary Dynatrace instrumentation to actually instrument the app and then have those calls show up in your Dynatrace tenant: 
https://www.dynatrace.com/support/help/technology-support/operating-systems/android/instrumentation-via-plugin/instrumentation-via-plugin/

FYI this is using groovy NOT kotlin 
