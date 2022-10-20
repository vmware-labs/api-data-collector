# API Data Captor for Mock Servers

API Data Captor for Mock Servers is a Chrome DevTools Extension powered by React and Ant Design that can capture HTTP Requests and save/edit its Response Payloads in JSON for updating local mock server database. It also can allow users to record the selected Requests/Responses details and save them as JSON or ZIP files. According to different input "project" and "session" field, the JSON object will be stored locally and can be retrieved. Also, it will generate custom routes.json file automatically.
## Installation

API Data Captor uses npm to manage and install packages. It is strongly recommended to install Node.js >16 and npm.

1. Clone the repo in your local system
```
git clone git@gitlab.eng.vmware.com:cpsbu/cloud-path/mock-server-generator.git
```

2. Enter the /extension folder in the repo, install the dependencies and build the application
```
npm install
 
npm run move
```

3. Open Chrome with the extensions management address chrome://extensions

4. Click the "Load Unpacked" button and selected the Repo folder

## Usage
- Project/Session management: You can select/input the "Project" and "Session" field to save/load your JSON file according to the selected two fields locally.

- Start/Stop recording: You can click on the "Capture" switch to enable/disable the recording functionalities.

- Max Record Limitation: You can click on the "Record Limit" switch to enable/disable the max number limitation for the records. The default value is 50. You can input and select the number you want in the selector near the switch.

- Clear: You can click the "Clear" button to clear all the captured information data in the current session.

- Setting: You can select the request type you want to capture.

- Save/Load locally: When you entered the "Project" and "Session" fields, you can click "Save To Local" or "Load From Local" button to store and retrieve the data stored in JSON object.

- Download: You can choose to download the captured data in JSON or ZIP format by clicking "Download JSON" or "Download ZIP" button. Also, you can download the selected data by clicking the "Download selected".

- Data Selection, Searching and Filtering: The captured data will be listed in the table below. You can click the "Response" button to preview the response payload. You can search the data according to the keywords in URL and select the data you want.

- Automated capture process for CPN mock server: As for OAuth Apps, the "oath-apps", "max-oath-apps" and "roles" fields are be automatically captured.

- Regular Expression for routes: Users can edit the regex lists by opening the regex modal. Specifically, each visited URL will be splitted by "/" and if one part matches regex list, it will be replaced by the corresponding identifier.

- Automated capture process for CPN mock server: As for OAuth Apps, the "oath-apps", "max-oath-apps" and "roles" fields are be automatically captured.

- Response editing: You can edit the response by clicking the response editing icon in the response preview page.

## License
- BSD-2
