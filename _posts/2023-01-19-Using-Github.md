## using Github
<br>
I started today practicing data analysis techniques using python, and I thought I should figure out how to publish these things onto github. With this I can share my examples for code such as monte carlo and machine learning. 
<br>
<br>
<b>Getting Started<b>
<br>
Once you have your github account setup you need to install git if you are using linux. Git allows you to commit and push your code directly into your repository. Once installed these are the steps I used to push my code. 
<br>
<b>Setup Config<b>: Setup config by git config user.name “<github username>”. You can find this in your profile. Then git config user.email “<github email>”
<br>
<b>Generate your SSH key<b>: This is basically your password for github. Check for any ssh keys you may have

 ~~~
 ls -al ~/.ssh
  
~~~
If no keys exist create one. 
 ~~~
$ ssh-keygen -t ed25519 -C "your_email@example.com"
$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/id_ed25519
~~~
The number at the end might be different if you renamed it. 
<br>
<br>
<b>Git going<b>
<br>
After you have your ssh key setup you can type git init to setup github initial files. Now you can use this example by github to push files to your repo.
~~~
$ echo "# Testing" >> README.md
$ git init
$ git add README.md
$ git commit -m "first commit"
$ git branch -M main
$ git remote add origin git@github.com:<your repo here>
$ git push -u origin main
~~~
Success!
I will be uploading code base off of montecarlo, geant4, root, and tensor flow. Stay tune!
