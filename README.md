# it-info
Information for the current IT Executive.

## About

This file is for the current IT Executive. This is a list of the how-to's to do your role in relation to the website. The website is hosted on Github pages because it's free and it's simpler. The websites are built in pure HTML, CSS, and JS. In this document, I'm assuming you have zero knowledge of Github or Github pages. If you have any questions, fire me a message on Facebook or chat to the previous years IT person.

## Using Github

### Why?

Pretty simply: it's free, keeps a copy of all files and copies of previous years so it's easy to get past speaker and sponsor information.


### Creating a new website repository

We have a QCOP organization. If you are not apart of this organization then you need to contact the co-chairs or the previous years co-chairs. They have `owner` permissions. All QCOP related code can be found [here](https://github.com/QCOP). Each year creates a new repository (In short: repo) for their website so following the naming convention `QCOP-20XX`. There is no copy of the [2016](https://github.com/qcop/qcop-2015) year however it was a fork of the 2015 in terms of looks, and the speaker and sponsor assets exists in [2017](https://github.com/qcop/qcop-2017).

![logo](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/step1_1.png "Logo Title Text 2")


As an owner, you can create the new repository: click the `+` in the top right corner, then `New Repository`. From the new repository page you can change the owner (using the dropdown) to be `QCOP`. Insert the name (`QCOP-20__`) and the description (`The Queen's Conference on Philanthropy website for 20__-20__`). Keep the repository public because website assets are public anyway (plus private costs money). Check `Initialize this repository with a README`, and add an `Apache License`. Then click `Create repository`.

![logo2](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/step1_2.png "Logo Title Text 2")


### Cloning your repository

Now open your new repository, so the URL would be something like: `https://github.com/qcop/qcop-20XX`. It will look like:

![logo3](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/step1_3.png "Logo Title Text 2")


Keep this open. Now you need `git`. Git and Github are two different things. Git is a versioning software for developers. And Github at a high level is a UI for public Git servers. I'm not going to explain it too much more but if you do some Googling, someone explains it.


#### Installing Git

Go to [https://git-scm.com/](https://git-scm.com/) and hit the download on the right side.

![logo4](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/step1_4.png "Logo Title Text 2")


Now install that.


#### Cloning

Open your repo Github page again. Under the green button, you'll see a URL. This should be `https`, if not click `Use HTTPS`. Copy it. It will be something like `https://github.com/qcop/qcop-20__.git`.


Open a terminal (this is a program) on your computer. Navigate to the desired folder using:
```
# Lists the current folders and files in your current directory
ls

# Navigates into a folder
cd ______

# Navigates back a folder
cd ..

# Takes you to your desktop
cd ~/Desktop
```

I'd probably do something like:
```
cd ~/Desktop
```

Then clone the repository using that `git` link:

```
git clone https://github.com/qcop/qcop-20__.git
```

And you should see a new folder in that directory (folder). Then navigate into that directory using:

```
cd qcop-20__
```

You can also press `tab` to auto complete the folder if you are at a unique part.

*Image with commands below*

### Making your commits

Just as a test/example copy and paste a file into that folder (A file you don't mind being public). After doing that, in your terminal with the repo being your current directory (hence follow the `cd` into the correct folder).

You should be able to type:

```
git status
```

and see the one file.

*Instructions from above in my terminal*

![logo5](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/step2_1.png "Logo Title Text 2")


Then type:
```
git add --all
```

or to add each individual file:
```
git add FILE_NAME_LIKE_CHANGE_THIS
# Example: git add ./example_file.txt
# ./ <-- means current directory
```

Then type (description cannot be blank):

```
git commit -m "DESCRIBE WHAT YOU DID HERE"
```

Then push it to the cloud/Github:
```
git push
```

And you should see it on Github.

![logo6](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/step2_3.png "Logo Title Text 2")


So every time you want to update the website. Change the file, then follow the `add`, `commit`, `push` commands. If you ever have an issue, do `git status` and read the recommended commands.



### Updating the GH-Pages Branch

On the repo, there is a settings tab. You'll have to open it.

![logo7](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/step3_1.png "Logo Title Text 2")


Scroll down to the `Github Pages` section. Use the `source` dropdown and select the `master branch`. This means all files on `master` will go to the website.

![logo28](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/step3_2.png "Logo Title Text 2")


Now you should be able to go to `https://qcop.github.io/qcop-20__` and see the website. It may take a few minutes. If you can't after 2 hours, you did something wrong.


### Pointing the domain

To get the QCOP domain to work on the Github pages so you go to `qcop.ca` instead of `https://qcop.github.io...`. You'll need to add a `CNAME` file to your repo (put one in the folder and push it to the server). This file is `CNAME` only, no extensions or anything. Look at the previous years to see an example. In this file add `qcop.ca`. You can open a file like this using [Atom](https://atom.io/), Sublime Text 3, Notepad++, Notepad, etc.


Next, QCOP's domain is registered with CanHost. The co-chairs should have the email and password.


![logo9](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/stepa.png "Logo Title Text 2")

![logo10](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/stepb.png "Logo Title Text 2")

![logo11](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/stepc.png "Logo Title Text 2")

![logo12](https://raw.githubusercontent.com/QCOP/it-info/master/imgs/stepd.png "Logo Title Text 2")
