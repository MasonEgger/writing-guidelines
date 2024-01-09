DigitalOcean is excited to continue building out its collection of technical articles related to server administration and software engineering. To ensure that DigitalOcean articles have consistent quality and style, we have developed the following guidelines.

There are four sections in this guide:

* **[Style](https://www.digitalocean.com/community/tutorials/digitalocean-s-writing-guidelines#style)**, our high-level approach to writing technical tutorials
* **[Structure](https://www.digitalocean.com/community/tutorials/digitalocean-s-writing-guidelines#structure)**, an explanation of our layout and content
* **[Formatting](https://www.digitalocean.com/community/tutorials/digitalocean-s-writing-guidelines#formatting)**, a Markdown reference guide
* **[Terminology](https://digitalocean.com/community/tutorials/digitalocean-s-writing-guidelines#terminology)**, a guide to common terms and word usage

To get published quickly, we recommend that you read the [Style](https://www.digitalocean.com/community/tutorials/digitalocean-s-writing-guidelines#style) and [Structure](https://www.digitalocean.com/community/tutorials/digitalocean-s-writing-guidelines#structure) sections in their entirety before you begin working on your article.

You can use the [Formatting](https://www.digitalocean.com/community/tutorials/digitalocean-s-writing-guidelines#formatting) section of this guide along with our [Markdown previewer](https://www.digitalocean.com/community/markdown) and [How To Write a Proposal and Outline for a DigitalOcean Community Tutorial](https://www.digitalocean.com/community/tutorials/how-to-write-a-proposal-and-outline-for-a-digitalocean-community-tutorial)  as references while writing your article.

We also have a [technical best practices guide](https://www.digitalocean.com/community/tutorials/technical-recommendations-and-best-practices-for-digitalocean-s-tutorials) outlining our tech-focused recommendations.

<$>[note]
We have developed [article templates in Markdown format](https://github.com/do-community/do-article-templates) you can use as a starting point for your article. We strongly recommend using one of these templates to plan and develop your article.
<$>

Read on to learn about our article style.

---

## Style

The style for DigitalOcean articles reflects our purpose in publishing them: to provide quality learning information for engineers and developers. We strive to ensure that all DigitalOcean tutorials are:

* **Comprehensive and written for all experience levels**
* **Technically detailed and correct**
* **Practical, useful, and self-contained**
* **Friendly but formal**

These principles guide authors to create articles, tutorials, and other learning materials that help people solve their problems and grow as developers.

### Comprehensive and written for all experience levels

Our articles are written to be as clear and detailed as possible without making assumptions about the reader's background knowledge.

We explicitly include every command a reader needs to go from their first SSH connection on a brand new server to the final, working setup. We also provide readers with all of the explanations and background information they need to understand the tutorial. The goal is for our readers to learn the concepts, not just copy and paste code and commands.

We avoid words like "simple,” "straightforward,” "easy," "simply," "obviously," and "just," as these words make assumptions about the reader's knowledge. While authors use these words to encourage and motivate readers to push through challenging topics, they often have the opposite effect; a reader who hears that something is "easy" may be frustrated when they encounter an issue. Instead, we encourage our readers by providing the explanations they need to be successful.

###  Technically detailed and correct

Our articles are technically accurate and follow industry best-practices. They also provide more details than just the code and commands. We don’t provide large blocks of configuration or program code and ask readers to paste it into their text editor, trusting us that it works and is safe. We provide all the details necessary for the readers to understand and trust the article.

Every command should have a detailed explanation, including options and flags as necessary. Every block of code should be followed by prose explanations that describe what it does and why it works that way. When you ask the reader to execute a command or modify a configuration file, first explain what it does and why you're asking the reader to make those changes. These details give readers the information they need to grow their skills.

Authors test their tutorials to ensure they work by following them exactly as written on fresh servers to ensure accuracy and identify missing steps. Our editors also test these articles as part of the review process to ensure a great learning experience for the reader.

### Practical, useful, and self-contained

Once a reader has finished a DigitalOcean article, they will have installed, built, or set up something from start to finish. We emphasize a practical approach: at the end of an article, the reader should have a usable environment or an example to build upon.

What this means for the writer is that the article should cover the topic thoroughly. Authors should link to existing DigitalOcean articles as prerequisites that readers will follow before beginning the tutorial and link to available DigitalOcean articles to provide additional information in the body of the tutorial. Authors should only send readers offsite to gather information if there’s no existing DigitalOcean article and the information can’t be added to the article directly in a short summary.

### Friendly but formal

Our tutorials aim for a friendly but formal tone. This means that articles do not include jargon, memes, excessive slang, emoji, or jokes. As we're writing for a global audience, we aim for a tone that works across language and cultural boundaries. 

Unlike blog posts, we do not use the first person singular (e.g., "I think ..."). Instead, we encourage the use of the second person (e.g., "You will configure ...") to keep the focus on the reader and what they'll accomplish. In some cases, we'll use the first person plural (e.g., "We will examine ...").

We encourage motivational language focused on outcomes. For example, instead of "You will learn how to install Apache," try "In this tutorial, you will install Apache." This approach motivates the reader and focuses on the goal they need to accomplish. 

Finally, the language of our tutorials honors diverse human experiences and follows our [Community Code of Conduct](https://www.digitalocean.com/community/pages/code-of-conduct). That means we avoid offensive language or other content that is in reference to (but not limited to) age, disability, ethnicity, gender identity or expression, level of experience, nationality, neurodiversity, personal appearance, race, religion, political affiliation, sexual orientation, socioeconomic status, or technology choices.


---

## Structure

DigitalOcean articles have a consistent structure, which includes an introduction, a conclusion, and any prerequisites necessary for a reader to get started. However, the specific structure depends on the type of article.

Most of the tutorials we publish are procedural, which walk the reader through accomplishing a task step-by-step. The structure for a procedural article should be:

* Title (Level 1 heading)
* Introduction (Level 3 heading)
* Prerequisites (Level 2 heading)
* Step 1 — Doing the First Thing (Level 2 heading)
* Step 2 — Doing the Next Thing (Level 2 heading)
* ...
* Step n — Doing the Last Thing (Level 2 heading)
* Conclusion (Level 2 heading)

Conceptual articles will have a title, an introduction, and a conclusion, but they might not have a prerequisites section or follow the "Step" convention:

* Title (Level 1 heading)
* Introduction (Level 3 heading)
* Prerequisites (optional) (Level 2 heading)
* Subtopic 1 (Level 2 heading)
* Subtopic 2 (Level 2 heading)
* ...
* Subtopic n (Level 2 heading)
* Conclusion (Level 2 heading)

Some articles are more focused on a very small specific task or solution, and they'll often have a title, a small introductory sentence, and a conclusion at the end. Those articles will have a structure like this:

* Title (Level 1 heading)
* Introduction paragraph
* Prerequisites (optional) (Level 2 heading)
* Article body
* Conclusion paragraph

Our [article templates](https://github.com/do-community/do-article-templates) have this structure already written for you in Markdown, and we encourage you to use these templates as a starting point for your own articles. 

### Title

When you write your title, think carefully about what the reader will accomplish by following your tutorial. Try to include the goal of the tutorial in the title, not just the tool(s) the reader will use to accomplish that goal. Ideally, titles will be under 60 characters long.

A typical title for a procedural tutorial follows this format: **How To \<Accomplish a Task> with \<Software> on \<Distro>**.

For example, if your tutorial is about installing the Caddy web server, the goal is likely to [host a website](https://www.digitalocean.com/community/tutorials/how-to-host-a-website-with-caddy-on-ubuntu-18-04). If your tutorial is about installing Fail2Ban, the goal might be to [protect an Nginx server](https://www.digitalocean.com/community/tutorials/how-to-protect-an-nginx-server-with-fail2ban-on-ubuntu-22-04). 

Titles that include the goal (like "[How To Host a Website Using Cloudflare and Nginx on Ubuntu 22.04](https://www.digitalocean.com/community/tutorials/how-to-host-a-website-using-cloudflare-and-nginx-on-ubuntu-22-04)") are generally more informative for the reader than titles that don't (like "How To Use Cloudflare and Nginx on Ubuntu 22.04").

### Introduction

The first section of every article is the **Introduction**, which is usually one to three paragraphs long. The purpose of the introduction is to motivate the reader, set expectations, and summarize what the reader will do in the article. Your introduction should answer the following questions:

* **What is the tutorial about?** What software is involved and what does each component do (briefly)?
* **Why should the reader learn this topic?** What are the benefits of using this particular software in this configuration? What are some practical reasons why the reader should follow this tutorial?
* **What will the reader do or create in this tutorial?** Are they setting up a server and then testing it? Are they building an app and deploying it? Be specific, as this provides the motivation readers need and gets them excited about the topic.
* **What will the reader have accomplished when they’re done?** What new skills will they have? What will they be able to do that they couldn't do before?

Answering these questions in your introduction will also help you design a clear and reader-focused tutorial, as you'll align the content of your tutorial to the things you mention in the introduction. A good introduction lets the learner know what the rest of the article is about.

Keep the focus on the reader and what they will accomplish. Instead of using phrases like "we will learn how to," use phrases like "you will configure" or "you will build."  This goes a long way to motivate the reader and get them excited about your topic. In addition, keep the focus on the problem the reader is solving rather than the technology. For example, if a tutorial is about building a project with React, you can focus your introduction on the project rather than explaining what React is.

### Prerequisites

The **Prerequisites** sections of DigitalOcean articles have a very specific format and purpose.

The purpose is to spell out _exactly_ what the reader should have or do before they follow the current tutorial. The format is a list that the reader can use as a checklist. Each point must link to an existing DigitalOcean tutorial that covers the necessary content or the official product documentation if there are no current DigitalOcean tutorials. This allows you to rely on existing content that is known to work instead of starting from scratch.

Our systems and DevOps tutorials take the reader from a fresh deployment of a vanilla distribution image to a working setup, so they should start with the first SSH connection to the server or include a prerequisite tutorial that does.

Common prerequisite for system administration and DevOps tutorials include:

* The number of servers necessary, including distribution, initial server setup, and any additional necessary options (like memory requirements, DO API keys, IPv6, or private networking).
* Software installation and configuration, such as Apache, a LAMP stack, or databases.
* Required DNS settings or SSL certificates.

Our software development tutorials work in a similar fashion, providing the reader with all of the prerequisites they'll need up front, including a prerequisite for the development environment. 

Common prerequisites for software development tutorials include:
* Local software needed, such as Git, Node.js, Python, Ruby, or Docker.
* Additional user accounts like GitHub, Facebook, Twitter, or other services your reader will need.
* Tutorials that will help the reader get their project started, such as or [How To Set Up an HTML Project](https://www.digitalocean.com/community/tutorials/how-to-set-up-your-html-project). 
* Conceptual articles that provide important background a reader might find helpful, such as [Understanding the DOM](https://www.digitalocean.com/community/tutorial_series/understanding-the-dom-document-object-model).

For example, a tutorial about building and deploying a Node.js application and deploying it to an Ubuntu server using Git might have the following prerequisites:

> To complete this tutorial, you will need: 
> * One Ubuntu 22.04 server set up by following [the Ubuntu 22.04 initial server setup guide](https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-22-04), including a non-root `sudo`-enabled user and a firewall.
> * A domain name configured to point to your server. You can learn how to point domains to DigitalOcean Droplets by following the [Domains and DNS guide](https://docs.digitalocean.com/products/networking/dns/).
> * Git installed on your local machine. You can follow the tutorial [Contributing to Open Source: Getting Started with Git](https://www.digitalocean.com/community/tutorials/contributing-to-open-source-getting-started-with-git) to install and set up Git on your computer.
> * A local development environment for Node.js, which you can set up with [How To Install Node.js on Ubuntu 22.04](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-22-04). For other systems, follow the appropriate tutorial on [How To Install Node.js and Create a Local Development Environment](https://www.digitalocean.com/community/tutorial_series/how-to-install-node-js-and-create-a-local-development-environment) for your system.

By reading the prerequisites, your reader knows exactly what they need to do before they start. There are no surprises. 

When you test your tutorial, follow all of the prerequisite tutorials exactly as written so that everyone uses the same starting point. If you change a variable or complete an optional step from one of the prerequisites, make sure to note that.

You can review good prerequisites examples for:

* Ubuntu 20.04 servers, software installation, and DNS records in [this Minio tutorial's prerequisites](https://www.digitalocean.com/community/tutorials/how-to-set-up-minio-object-storage-server-in-standalone-mode-on-ubuntu-20-04#prerequisites).

* Handling multiple servers with software installation in [this monitoring tutorial’s prerequisites](https://www.digitalocean.com/community/tutorials/how-to-monitor-server-health-with-checkmk-2-0-on-ubuntu-20-04) or [this Nagios and Alerta tutorial's prerequisites](https://www.digitalocean.com/community/tutorials/how-to-monitor-nagios-alerts-with-alerta-on-centos-7#prerequisites).

* React-based web development projects by reading [How To Test a React App with Jest and React Testing Library](https://www.digitalocean.com/community/tutorials/how-to-test-a-react-app-with-jest-and-react-testing-library).

Be specific with your prerequisites. A prerequisite like "Familiarity with JavaScript" without a link to something specific doesn't give your reader much context. Instead, list specific concepts the reader should know and provide them with resources that help them get up to speed so they can successfully complete your tutorial. For example, use something like “Familiarity with Javascript. To build your skills, check out the [How To Code in JavaScript](https://www.digitalocean.com/community/tutorial_series/how-to-code-in-javascript)  series.”

### Steps

The **Step** sections are the parts of your tutorial where you describe what the reader needs to do and why. A step contains commands, code listings, and files, and provides explanations that not only explain **what to do** but also **why you're doing it this way.**

Each step begins with a level 2 heading. 

Procedural tutorials start each step title with the word **Step** and a number, followed by an em-dash. The step title describes what readers will accomplish in that step and uses a gerund (**-ing** words), like so:

> Step 1 – Creating User Accounts

After the title, add an introductory sentence that describes what the reader will do in each step  and what role it plays in achieving the overall goal of the tutorial. Focus on the reader. Instead of phrases like "We will learn" or "I will explain," use phrases like "You will build" or "you will create."

### Commands in Steps

All commands a reader must run should be on their own line in their own code block, and each command should be preceded by a description that explains what the command does. After the command, provide additional details about the command, such as what the arguments do and why your reader is using them. 


> Execute the following command to display the contents of the `/home/<^>sammy<^>` directory, including all hidden files:
> ```command
> ls -al /home/<^>sammy<^>
> ```
> The `-a` switch shows all files, including hidden ones, and the `-l` switch shows a long listing including timestamps and file sizes.

You should display the output of commands and programs using a separate code block, such as the following example:

> Run the `hello.js` program:
> ```command
> node hello.js
> ```
> The program's output will print to the screen:
> ```
> [secondary_label Output]
> Hello world!
> This is my first Node.js program!
> ```

The output block has a label and is separated from the command with some text that explains the output. Separating the commands from the output makes it more clear to readers where the command ends and the output begins.

If readers will be moving between directories, be sure to provide the command(s) necessary for those movements.

### Opening, Creating, and Viewing Files

Like commands, always introduce a file or script by describing its general purpose, then explain any changes that the reader will be making in the file. Without these explanations, readers won't be able to customize, update, or troubleshoot issues.

Explicitly tell the user to create or open each file you'll have them use.

On tutorials that are targeted to command-line users, instruct the reader to create and open the file using a command on its own line:

> Open the file `/etc/hginx/config` with the following command:
> ```command
> nano /etc/nginx/sites-available/default
> ```

<$>[note]
We use the `nano` editor for Ubuntu and Debian tutorials as it's already installed. We use `vi` on tutorials for CentOS and FreeBSD. In all cases, avoid using `touch` to create new empty files, as your readers can create files with the editor directly.
<$>

For tutorials where the reader is not expected to use the command-line interface, such as front-end development tutorials, you can omit the command to open the file. However, be sure to tell the reader which file to open explicitly:

> Open the file `src/App.js` in your editor.

A reader should always know which file they're working with.

### Code blocks

We treat all code as an opportunity for learning. If you're asking the reader to write code, follow the same approach as for commands: introduce the code block with a high-level explanation of what it does. Then show the code, and then call out any important details. 

Here's an example:

> Create the file `hello.js` in your text editor:
> ```command
> nano hello.js
> ```
> Add the following code to the file, which prints a message to the screen:
> ```js
> [label hello.js]
> console.log("Hello world!");
> console.log("this is my first Node.js program!")
> ```
> The `console.log` function takes a string and prints it to the screen on its own line.

Note that the code block has a label that clearly shows the filename.

[This Docker Swarm tutorial](https://www.digitalocean.com/community/tutorials/how-to-create-a-cluster-of-docker-containers-with-docker-swarm-and-digitalocean-on-ubuntu-16-04) is a good example of how to use our custom Markdown to distinguish between commands run on several different servers, as well as locally.

Sometimes you'll open a file and ask the reader to change something specific. When you do this, show the relevant parts of the file and use highlighting to make it clear what should change:

> Open the file `/etc/nginx/sites-available/default` in your editor:
>
> ```command
> nano /etc/nginx/sites-available/default
> ```
>
> Change the `server_name` value to your domain name:
>
> ```nginx
> [label /etc/nginx/sites-available/default]
> server {
>     listen 80 default_server;
>     listen [::]:80 default_server ipv6only=on;
> 
>     root /usr/share/nginx/html;
>     index index.html index.htm;
> 
>     server_name <^>your_domain<^>;
> ...
> 
> }
>```

Be sure to explain what the change does and why it’s necessary.

DigitalOcean's [custom Markdown and formatting guidelines](http://do.co/style#formatting) are designed to help make our tutorials' instructions as easy to read as possible. 

### Transitions

Each step should be framed with a brief introductory sentence and a closing transition sentence that describes what the reader accomplished and where they are going next. Transitions guide the reader and provide important context for instructions, commands, and output. To avoid repetition, vary the language used for these sentences so that it does not reiterate the step titles.

Here is an example of a transition at the end of Step 1 in this tutorial on [How To Secure Nginx with Let's Encrypt on Rocky Linux 8](https://www.digitalocean.com/community/tutorials/how-to-secure-nginx-with-let-s-encrypt-on-rocky-linux-8#step-2-updating-the-firewall-rules):

> You have now installed the Let’s Encrypt client, but before obtaining certificates, you need to make sure that all required ports are open. To do this, you will update your firewall settings in the next step.

In the example above, the author summarized what the reader achieved, introduced the next task, and explained how the two steps are connected.

Framing each step in this way helps readers learn and motivates them to keep going. 

### Conclusion

The **Conclusion** of your tutorial should summarize what the reader has accomplished by following your tutorial. Instead of using phrases like "we learned how to," use phrases like "you configured" or "you built."  

The conclusion should also describe what the reader can do next, which can include a description of use cases or features the reader can explore, links to other DigitalOcean tutorials with additional setup or configuration, and links to external documentation.

Some good examples include [this Kubernetes tutorial’s conclusion](https://www.digitalocean.com/community/tutorials/how-to-access-vault-secrets-inside-of-kubernetes-using-external-secrets-operator-eso#conclusion) and [this `node-csv` tutorial's conclusion](https://www.digitalocean.com/community/tutorials/how-to-read-and-write-csv-files-in-node-js-using-node-csv#conclusion).

---

## Formatting

DigitalOcean tutorials are formatted in the Markdown markup language. [Daring Fireball](http://daringfireball.net/projects/markdown/syntax) publishes a comprehensive Markdown guide if you're unfamiliar with it. DigitalOcean also uses some [custom Markdown](https://www.digitalocean.com/community/markdown). Examples of our custom Markdown are in the appropriate sections below.

### Headers

Each section of our tutorials has a corresponding header: the title should be an H1 header; the introduction should be an H3 header; prerequisites, steps, and conclusion should have H2 headers. You can review this format in our [Markdown article templates](https://github.com/do-community/do-article-templates).

For procedural tutorials, step headers should include step numbers (numerical) followed by an em dash (**—**). 

Step headers should also use the gerund, which are **-ing** words. An example step header is **Step 1 — Installing Nginx**.

Use H3 headers sparingly, and avoid H4 headers. If you need to use subheaders, make sure there are two or more headers of that level within that section of the tutorial. Alternatively, consider making multiple steps.

### Line-level Formatting

**Bold text** should be used for:

* Visible GUI text
* Hostnames and usernames, like **wordpress-1** or **sammy**
* Term lists
* Emphasis when changing context for a command, like switching to a new server or user

*Italics* should only be used when introducing technical terms. For example, the Nginx server will be our *load balancer*.

In-line code formatting should be used for:

* Command names, like `unzip`
* Package names, like `mysql-server`
* Optional commands
* File names and paths, like `~/.ssh/authorized_keys`
* Example URLs, like `http://<^>your_domain<^>`
* Ports, like `:3000`
* Key presses, which should be in ALL CAPS, like `ENTER`. If keys need to be pressed simultaneously, use a plus symbol (**+**), such as `CTRL+C`.

### Code Blocks

Code blocks should be used for:

* Commands the reader needs to execute to complete the tutorial
* Files and scripts
* Terminal output
* Interactive dialogues that are in text

Indicate excerpts and omissions in files with ellipses (**. . .**). If the reader needs to make any changes, use highlighting:

> ```nginx
> [label /etc/nginx/sites-available/default]
> server {
>     listen 80 default_server;
>     listen [::]:80 default_server ipv6only=on;
> 
>     root /usr/share/nginx/html;
>     index index.html index.htm;
> 
>     server_name <^>your_domain<^>;
> ...
> 
> }
>```

If most of a file can be left with the default settings, we typically show just the section that needs to be changed.

If readers are adding lines to pre-existing code, use highlighting to indicate the new lines or other changes. Here’s an example from the tutorial, [How To Use Go Modules](https://www.digitalocean.com/community/tutorials/how-to-use-go-modules).

> Open your `main.go` file from the `mymodule` directory and add a call to `PrintHello` by adding the highlighted lines below:
> 
> ```go
> [label projects/mymodule/main.go]
> 
> package main
> 
> import <^>(<^>
> 	"fmt"
> 
> 	<^>"mymodule/mypackage"<^>
> <^>)<^>
> 
> func main() {
> 	fmt.Println("Hello, Modules!")
> 
> 	<^>mypackage.PrintHello()<^>
> }
> ```

In the example above, the items that a reader will add are all highlighted.

#### Code Block Prefixes

Do not include the command prompt (`$` or `#`) in the code block. Instead, use DigitalOcean's custom Markdown for non-root user commands, root user commands, and custom prefixes, respectively:

	```command
	sudo apt update
	```
	
	```super_user
	adduser <^>sammy<^>
	```
	
	```custom_prefix(mysql>)
	FLUSH PRIVILEGES;
	```

This is how the preceding examples will render:

> ```command
> sudo apt update
> ```
>
> ```super_user
> adduser <^>sammy<^>
> ```
>
> ```custom_prefix(mysql>)
> FLUSH PRIVILEGES;
> ```

When you present the commands this way, readers won't be able to accidentally select the prompt characters.

#### Code Block Labels

DigitalOcean's Markdown also includes labels and secondary labels. You can add labels to code blocks by adding a line with `[label Label text]` or `[secondary_label Secondary label text]` anywhere in the block.

Use labels to mark code blocks containing the contents of a file with a filename. For example, if you have a file called `app.js`, use `[label app.js]` to label the code block:

    ```js
    [<^>label app.js<^>]
    console.log("Hello World!");
    ```

The label is displayed above the code listing:

```js
[label app.js]
console.log("Hello World!");
```

Use secondary labels to mark terminal or program output printed to the screen, like this:

    ```
    [<^>secondary_label Output<^>]
    Hello World!
    ```

Secondary labels look like this:

```
[secondary_label Output]
Hello World!
```

Labels help readers understand what they're reading and how it fits in to the larger picture.

#### Code Block Environment Colors

Sometimes you'll have the reader work on multiple computers, such as their local machine and multiple servers. Using different colors for the environment display can make this easier for readers to follow. DigitalOcean's Markdown allows you to color the background of a code block by adding a line with `[environment <^>name<^>]` anywhere in the block. The options for `<^>name<^>` are `local`, `second`, `third`, `fourth`, and `fifth`.

For example, if you're writing a tutorial and you want to show a command that should be run locally instead of on a server, you can use `[environment local]`:

>```command
>[environment local]
>ssh root@<^>your_server_ip<^>
>```

These are non-primary server command examples, useful for multi-server setups:

Using `[environment second]` will render like this:

```command
[environment second]
echo "Secondary server"
```

Using `[environment third]` will render like this:

```command
[environment third]
echo "Third server"
```

Using `[environment fourth]` will render like this:

```command
[environment fourth]
echo "Fourth server"
```

And `[environment fifth`] will render like this:

```command
[environment fifth]
echo "Fifth server
```

Use these colors in multi-server or multi-environment tutorials. Where necessary, you can stack an environment label and an output label to indicate a file within a different environment, like this sample Output block in a local environment:

> ```
> [environment local]
> [secondary_label Output]
> Hello World!
> ```

Nested labels ensure that the reader has all the requisite information to run commands in the appropriate terminal session.


### Notes and Warnings

The DigitalOcean Markdown parser allows for custom **note** and **warning** code blocks to be used to display very important text.

Here's a Markdown example of a note and a warning (this is an image):

![Notes and Warnings](https://assets.digitalocean.com/articles/do_formatting/note_warning.png)

Here's the rendered result:

<$>[note]
**Note:** This is a note.
<$>

<$>[warning]
**Warning:** This is a warning.
<$>


### DigitalOcean-specific Info

The `[info]` callout is helpful when discussing DigitalOcean specific features.

<$>[info]
This feature is specific to DigitalOcean's Droplets.
<$>


### Variables

Highlight any items that the reader needs to change, like example URLs, version numbers, or modified lines in configuration files. You can do this by surrounding the word or line with our custom **<^>** Markdown. 

Here’s an example from the [Initial Server Setup with Ubuntu 22.04](https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-22-04):

>This example creates a new user called **sammy**, but you should replace that with a username that you like:
>
>```super_user
>adduser <^>sammy<^>
>```


<$>[note]
**Note**: You cannot highlight multiple lines with one pair of symbols, so you need to highlight each line individually. Occasionally a symbol like a shebang (`#`) or a backtick might break the highlighting feature in the line, and you may need to have two highlighted sections on the same line.
<$>

If you reference a variable in a context where you would normally also use `in-line code` formatting, you should use `<^>both styles<^>`. Make sure your tutorial is as accessible as possible by using language like "highlighted in the preceding code block" instead of "highlighted in red above."

Avoid language like "highlighted in yellow," as highlighting colors might change. 

### Images and Other Assets

Images can quickly illustrate a point or provide additional clarification in a step. Use images for screenshots of GUIs, interactive dialogue, and diagrams of server setups. Don't use images for screenshots of code, configuration files, output, or anything that can be copied and pasted into the article.

When including images in your tutorial, please follow these guidelines:

* Include descriptive alt text so readers using a screen reader can rely on the alt text rather than the image.
* Include a brief caption to contextualize the image within the context of the article (the caption will typically be shorter than alt text).
* Use the `.png` file format.
* Host images on [imgur](http://imgur.com/).
* Make the image with as short a height as possible.

If you make a mockup of a diagram for your tutorial, we will create a diagram in the DigitalOcean style. We'll also upload all images to DigitalOcean servers at publication time.

Here's a Markdown example for including images in your tutorial:

```
![Descriptive alt text for screen readers](http://imgur.com/your_image_url “Brief caption here”)
```

You can review examples of strong descriptive alt text in the images in [this Matomo tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-matomo-web-analytics-on-ubuntu-20-04).

Occasionally, you will want the reader to have access to a configuration file that is too long to display in the main body of the tutorial. DigitalOcean will host this file on our assets server. You can use standard link formatting to link to the file.

## Terminology

Technical articles and tutorials will use a lot of terminology, and we've standardized some of the terminology and word usage.

### Users, Hostnames, and Domains

Our default example username is `sammy`. You can also choose something descriptive where helpful, like `webdav-kai` or `nsd`.

The default hostname is `your_server`, though you may want to choose something more descriptive in multi-server setups, such as `django\_replica\_1`.

The default domain is `your_domain`. For multi-server setups, you can choose something like `primary-1.your_domain` or `replica-1.your_domain`. While `example.com` is a valid domain for documentation, using `your_domain` in tutorials makes clear that the reader should change the domain in examples.

Use highlighting when using these in configuration files, code, and output blocks, like this:

```
[label example configuration file]
ip: <^>your_server_ip<^>
domain: primary-1.<^>your_domain<^>
```

This makes it clear to readers that there is something they should change.

### IP Addresses and URLs

`<^>your_server_ip<^>`, with in-line code formatting and variable highlighting, is the default way to show an IP address. You can show multiple IP addresses with names like `<^>primary_private_ip<^>` and `<^>replica_private_ip<^>`. If you need to illustrate more realistic IP addresses, use an address in the [one of the two blocks reserved for documentation as per RFC-5737](https://tools.ietf.org/html/rfc5737). Specifically, we recommend `203.0.113.0/24` for example public addresses and `198.51.100.0/24` for example private addresses.

Example URLs that contain a variable the reader needs to customize should use code formatting with the variable highlighted. We default to using `<^>your_domain<^>`, like `https://<^>your_domain<^>:3000/simple/` or `http://<^>your_server_ip<^>/`. However, live links should use the standard Markdown link style with no extra formatting.

### Software

Use the official website's capitalization of the name of their software. If the product web site is not consistent with their capitalization, be consistent within a single article.

Link to the software's home page when you first mention the software.

### Multi-server Setups

For technical clarity, use the project's terminology for multi-server setups. Please be clear that the terms are coming from the project. For example: "The Django project refers to the original server as the **primary** and the secondary server as the **replica**. The MySQL project refers to the original server as the **master** and the secondary server as the **slave**."

When discussing multi-server architectures more abstractly, use the terms **primary** and **replica** or **manager** and **worker**.

### Technical Best Practices

Our [technical best practices guide](https://www.digitalocean.com/community/tutorials/technical-recommendations-and-best-practices-for-digitalocean-s-tutorials) guide contains more guidance that will help you create consistent, quality tutorials that help our readers.

Follow this link to [become a DigitalOcean author](https://www.digitalocean.com/community/pages/write-for-digitalocean).