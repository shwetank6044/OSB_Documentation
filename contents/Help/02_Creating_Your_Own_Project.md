### Is your model on ModelDB?

First of all, if the model is published, **please submit the original scripts to [ModelDB](http://senselab.med.yale.edu/ModelDB/default.asp*)**. This is the correct place for depositing models at the time of publication and should be the first port of call for anyone looking for scripts related to a publication in computational neuroscience.

Placing a model on OSB after submission to ModelDB is an indication that you wish to develop your (or other modellers’ publicly shared) models in an open source collaborative environment, to get help debugging/improving them, to convert them to simulator independent formats, and generally encourage wider reuse.

### Sign up to OSB

Register as a user of OSB [here](/account/register). Add your GitHub username and [INCF user profile](http://incf.org/community/people) if you have one.

You should also add the URL of your project, software or lab. In the latter case, if the PI is in agreement, we can add the group to the list of [labs taking part in the OSB initiative](/about#who_about). Please send a mail to info@opensourcebrain.org if you are interested in that.

### Share your code

Create a new repository for your code on GitHub (see [here](/docs/Help/Some_Extra_Information) if want to know more about Source Code technologies and Git/GitHub). See the introduction to creating a new repository on [GitHub help](https://help.github.com/articles/create-a-repo). 

The repository can be hosted on the [OpenSourceBrain GitHub organisation](https://github.com/OpenSourceBrain), but there is no problem having it under your personal account. If you would like us to host the repository, <a href="mailto:info@opensourcebrain.org">let us know</a> and we’ll add the repository and give your GitHub user full access to it.

### Create a new OSB project

Go to http://www.opensourcebrain.org when you’re logged in. There should be a green button on the top right for adding a new project.

![](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/NewProject.png)

Enter the long name of the project (this can be edited later), the short ID (this can't be changed), a description of the project and the path to the GitHub repository. If the code is not on GitHub yet, or if you host it elsewhere leave this blank. The repository URL can be added manually at a later point.

### Write your documentation/wiki

OSB documentation is written in [Markdown format syntax](https://daringfireball.net/projects/markdown/basics), together with some further Redmine and OSB specific additions (See below for further information). Note Markdown allows you to include most HTML syntax (i.e. videos...). In order to be as compatible as possible with GitHub wikis, OSB uses [GitHub Flavored Markdown](https://help.github.com/articles/markdown-basics). You can find a cheatsheet [here](/help/en/wiki_markdown_syntax.html).  

We describe briefly below some OSB/Redmine features to enhance wiki pages on OSB.

#### Reference to a Repository file. 

You can point to any file (markdown or plain text) in your GitHub or Bitbucket repository (the repository used in your project).

<code>github:[path]</code>
<code>bitbucket:[path]</code> 

This will retrieve the file content and display it in the OSB wiki page. This allows a single file in your repo (e.g. the main README) to be the master copy of the documentation for your project, and to make that accessible to someone browsing the project on OSB.

###### Example: 
<code>github:help/readme.md</code>
<code>bitbucket:help.txt</code>


#### Reference to pubmed publication: 

<code>pubmed:[publicationID]</code>

###### Example: 

<code>pubmed:17442244</code> 

This syntax will generate a reference link like this:
pubmed:17442244

and a bibliography section will be automatically generated at the bottom of the page. This section will summarize all the references using the following format:

Gleeson P,			Steuber V and 			Silver RA,
<i><a href="http://www.ncbi.nlm.nih.gov/pubmed/17442244">neuroConstruct: a tool for modeling networks of neurons in 3D space.</a></i> Neuron, 2007, 54(2): 219-35 

#### Create a formula

You can wrte formulas in your documentation using the LaTeX syntax. You only need to enclose you formula like this:

<code>{{latex(formula)}}</code>

###### Example:

<code>{{latex(x=\frac{-b\pm\sqrt{b^2-4ac}}{2a})}}
</code>

This will automatically generate the following image using the [google chart API](https://developers.google.com/chart/infographics/docs/formulas): 
![](https://raw.githubusercontent.com/OpenSourceBrain/OSB_Documentation/master/resources/images/formula.png)

#### Link to Wiki page

If you want to link to other wiki page:

<code>[[Wiki page]]</code>

<a href="#">Wiki page</a>

#### Link to an Issue

If you want to link to an issue in your project:

<code>Issue #12</code>

Issue <a href="#">#12</a>

#### Link to a Commit

If you want to link to a commit in your repository:

<code>commit:f30e13e43</code>

<a href="#">f30e13e4</a>


### Say hello…

Now is a good time to drop us a line on info@opensourcebrain.org, and let us know your plans for what you’d like to get out of OSB. We’re always happy to hear from new users.
