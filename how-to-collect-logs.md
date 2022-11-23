If you’re troubleshooting an issue with the Agora Chat SDK,Agora support team might ask you to send the SDK logs:

`SDK logs` : Record information about events that have occurred in SDK. They can include errors and warnings as well as informational events.

* By default, the SDK outputs three log files, easemob.log, two easemob_Y-m-d_H-M-S.log files each with a default size of 2048 KB(2M).  
* These log files are encoded in UTF-8.  
* The SDK writes the latest logs in easemob.log.  
* When easemob.log is full, the SDK deletes the log file with the earliest modification time among the other two, renames easemob.log to the name of the current time-dependent file log file, and creates a new easemob.log to record latest logs.

## How to Collect SDK logs
SDK logs can be found in the following directories, depending on your operating system.

### Android
1. Enable debug Mode : 
```
 ChatClient.getInstance().setDebugMode(true);
```
2. open the logs directory: `/sdcard/Android/data/{package name}/{appkey}/core_log/` which contains the SDK logs.

### iOS
#### Simulator 
1. Copy the `app sandbox path` printed by NSHomeDirectory()
2. In the Finder on your Mac, select Go > Go to Folder
3. Paster the path(command + v),and press return
4. open the logs directory:`{app sandbox path}/Library/Application Support/HyphenateSDK/easemobLog/` which contains the SDK logs.
