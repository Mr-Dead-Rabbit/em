If you’re troubleshooting an issue with the Agora Chat SDK,Agora support team might ask you to send the SDK logs:

`SDK logs` : Record information about events that have occurred in SDK. They can include errors and warnings as well as informational events.

## How to Collect SDK logs
SDK logs can be found in the following directories, depending on your operating system.

### Android
1. Enable debug Mode : ChatClient.getInstance().setDebugMode(true);
2. open the logs directory: `/sdcard/Android/data/{packagename}/{appkey}/core_log/easemob.log` which contains the SDK logs.

### iOS
#### Simulator 
1. Copy the path printed by NSHomeDirectory()
2. In the Finder on your Mac, select Go > Go to Folder
3. Paster the path(command + v),and press return
4. open the logs directory:`{the path}/Library/Application Support/HyphenateSDK/easemobLog/easemob.log` which contains the SDK logs.
