# Upgrade Kubectl in Cloud Shell

Run the following commands in your **Cloud Shell** terminal to upgrade Kubectl to the latest version

```
cd /google/google-cloud-sdk/bin/
sudo mv kubectl kubectl.orig
sudo wget https://storage.googleapis.com/kubernetes-release/release/v1.3.2/bin/linux/amd64/kubectl
sudo chmod +x kubectl
cd ~
```

Now run `kubectl version`, and you should get an output that looks like this, wherein the Client version and the Server Version should match:

```
Client Version: version.Info{Major:"1", Minor:"2", GitVersion:"v1.2.4", GitCommit:"3eed1e3be6848b877ff80a93da3785d9034d0a4f",
 GitTreeState:"clean"}
Server Version: version.Info{Major:"1", Minor:"3", GitVersion:"v1.3.2", GitCommit:"9bafa3400a77c14ee50782bb05f9efc5c91b3185",
 GitTreeState:"clean"}
```
