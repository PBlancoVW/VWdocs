# Quick start


## How to start collaborating?

For now the files are in GitHub and are public to anyone. I will try to have the files in Perforce, with a link to the website in the Intranet. That way the website would be easy to modify and easy to access.

If you want to start collaborating, there are two ways to modify the files. 
 
<br/>

**Option 1: to modify a single file**

Click the "EDIT DOCUMENT" link that can be found in any of the pages of this website. This will redirect you to GibHub, so you need a GibHub account and be signed in. There, click on the pen symbol to edit the file. This will fork the file to a repository in your account. You can make changes and then make a pull request to merge it with the original repository.

<br/>

**Option 2: to modify many files and create new ones**

Go to [https://github.com/PBlancoVW/vectordocu](https://github.com/PBlancoVW/vectordocu) and fork the repository. For this you need a GibHub account and be signed in. A copy of the original repository will be created in your account. You can modify it and then make a pull request to merge it with the original repository.

You can clone the repository to your computer and then commit the changes (for this you can use [GitHub Desktop](https://desktop.github.com/) or the [command line](https://github.com/GarageGames/Torque2D/wiki/Cloning-the-repo-and-working-with-Git)).

To easily modify Markdown files and see the format immediately, you can use a [Markdown editor](https://speckyboy.com/markdown-tools-editors/) (e.g. [MarkdownPad 2](http://markdownpad.com/news/2013/introducing-markdownpad-2/) for Windows).

If you create a file, remember to add a link inside _sidebar.md or in other file so that it can be accessed.

__To run the website locally and test the changes__

Install docsify:

```
npm i docsify-cli -g
```

Run the following command:

```
docsify serve docs
```

And open [http://localhost:3000](http://localhost:3000) in your web browser. You don't need to run the command again, as long as this is running you will see the changes immediately.

<br/>

If you need further help you can send an email to pblanco@vectorworks.net or slack me (Pablo).