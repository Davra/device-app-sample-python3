## How to create a Python Device Application running as a Systemd Service


### Copy this sample code, edit and assemble artifact.
- Clone this directory of files to a local directory of your own.
- Edit config.txt to assign a unique applicationName.
- Get the very latest SDK at https://raw.githubusercontent.com/Davra/device-agent-python3/main/davra-agent/davra_sdk.py
- Edit app.py to perform your application code as required.
- Edit requirements.txt to list the python libraries you require.
- Run ./build.sh to assemble the .tar.gz artifact.

### Deploy to devices using Jobs mechanism
- Upload the .tar.gz artifact to the file repository in the Davra Platform.
- Create a job to "Install application as a service" on selected devices.
- Choose the artifact uploaded in prior steps as the file to deploy.
- The job will place the artifact on the device, unzip it and run install.sh.

### Further versions
- Edit code as required such as app.py.
- Edit version in config.txt.
- Edit requirements.txt if new python libraries required.
- Run ./build.sh.
- Deploy to devices as above.

### SDK versions
While a copy of davra_sdk.py is included, the SDK may be amended over time. It is released
as part of the device-agent-python3 project and the latest version can be retrieved from:
https://raw.githubusercontent.com/Davra/device-agent-python3/main/davra-agent/davra_sdk.py
In order to avail of the latest SDK features, you may also need to run the latest agent version:
https://github.com/Davra/device-agent-python3
