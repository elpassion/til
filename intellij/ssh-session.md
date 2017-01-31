## Configuring SSH Session in IntelliJ IDEA

#### 1. Add server
- Launch IDE preferences with <kbd>command</kbd> + <kbd>;</kbd>
- Go to *Build, Execution, Deployment > Deployment*
- Click *Add server* action
- Type name and select type: **SFTP**
- Enter server host/port and your credentials with preferred auth type
- Click *OK* to apply changes

#### 2. Select host to connect
- Close all dialogs and launch enter action dialog with <kbd>command</kbd> + <kbd>shift</kbd> + <kbd>A</kbd>
- Start writing down: *Start SSH Session...*
- Select host by name entered in previous step
- You're connected, next time omit step 1