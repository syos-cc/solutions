Configure :
* Install KeePassXC
* Create new KeePassXC database with YubiKey Challenge-Response Credential
  * ( youtube : How To: Programming the YubiKey with a Challenge-Resonse Credential )
* Create in KeePassXC new SSH-Agent entry ( maybe with upload the file, not as external key )
* Configure this entry to add/remove key automatically to ssh-agent
* Under settings -> SSH-Agent configure the Agent
  * ( tested linux and macos with SSH-Agent-Integration and windows with putty-agent )
* Setup ssh-agent and KeePassXC as apps who start when system boot

Usage :
* When system boot, open with your Yubi-key the database.
  * That's it :-)
The ssh-keys will automatically loaded to the running ssh-agent and removed if KeePass will be closed.
