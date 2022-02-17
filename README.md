# ServiceNow to Github
## On Your Laptop
1, run `ssh-keygen -t rsa -b 4096 -C "[YOUREMAIL]"`

2, Will generate two files, id_rsa (private key) + id_rsa.pub (public key)
## On Github.com
1, Add public key by copy/paste the content of id_rsa.pub

## In Studio of ServiceNow
1, Create a "SSH Private Key Credentials", name="MyKey", copy/paste private key from id_rsa.

![image](https://user-images.githubusercontent.com/89544426/154189101-aecf0961-7464-4380-b596-cd0ca25af1ff.png)

![image](https://user-images.githubusercontent.com/89544426/153349412-0c05f2d5-5b13-47ed-9ef8-4177c1cdc837.png)


The password will be auto pupulated when "SSH Private Key" is filled.

2, Click on "source control"

![image](https://user-images.githubusercontent.com/89544426/152921938-4956f8c7-fbbc-4e2f-8d2c-055a7fb02996.png)

3, Click "link to source control"

4, Copy/Paste URL "git@github.com:[repo]"

5, Select Credential, "MyKey"

6, Click " connect Link" Button.

refer to : `https://developer.servicenow.com/dev.do#!/guides/rome/developer-program/github-guide/troubleshooting-github-issues`

Done.

