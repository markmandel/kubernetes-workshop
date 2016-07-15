# Upgrade Kubectl in Cloud Shell

Run the following commands in your **Cloud Shell** terminal to upgrade Kubectl to the latest version

```
cd /google/google-cloud-sdk/bin/
sudo mv kubectl kubectl.orig
sudo wget https://storage.googleapis.com/kubernetes-release/release/v1.3.0/bin/linux/amd64/kubectl
sudo chmod +x kubectl
cd ~
```

Now run `kubectl version`, and you should get an output that looks like this, wherein the Client version and the Server Version should match:

```
Client Version: version.Info{Major:"1", Minor:"3", GitVersion:"v1.3.0", GitCommit:"283137936a498aed572ee22af6774b6fb6e9f
d94", GitTreeState:"clean", BuildDate:"2016-07-01T19:26:38Z", GoVersion:"go1.6.2", Compiler:"gc", Platform:"linux/amd64"
}
Server Version: version.Info{Major:"1", Minor:"3", GitVersion:"v1.3.0", GitCommit:"283137936a498aed572ee22af6774b6fb6e9f
d94", GitTreeState:"clean", BuildDate:"2016-07-01T19:19:19Z", GoVersion:"go1.6.2", Compiler:"gc", Platform:"linux/amd64"
}
```