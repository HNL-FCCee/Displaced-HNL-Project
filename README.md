# HNL Project

- [HNL Project](#hnl-project)
  * [Welcome](#welcome)
  * [Editing the repository](#editing-the-repository)

## Welcome
Welcome to the HNL Project git page.
How do you use it?
It is markdown (see the extension of this file, '.md'), you can learn a bit more on what markdown can do, you can check the [GitHub markdown guide](https://guides.github.com/features/mastering-markdown/), and also my favorite place, [CodiMD](https://codimd.web.cern.ch/). 

## Editing the repository
Since it is for documentation, no need for branches.

You can edit directly in the browser using the pencil:

![Pencil blue](pencil.png?raw=true "Pencil in blue")

Or you can copy the repository to a folder in your computer or the lxplus using the following commands.
The first time you need to clone the repository:

`git clone https://github.com/HNL-FCCee/Displaced-HNL-Project `

`cd Displaced-HNL-Project`

Then, inside the folder you can add new files or work in what is there. To add new files, you either just move them there, or create them and edit them normally inside the folder. When you are ready to upload your changes, this is what you have to do.
If you have new files:

`git add nameofthenewfile.extensionofthenewfile`

And then:

`git commit -am "Whatever message to explain your commit"`

`git push`

That is it, this is the simplest, most bare-bones use of a github repository.
