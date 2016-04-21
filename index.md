---
layout: workshop
root: .
venue: "Scripting Carpentry"
address: Puget Sound Regional Council, 1011 Western Ave, Suite 500, Seattle WA
country: us
language: en
latlng: 47.6054148,-122.337372
humandate: "Spring 2016"
humantime: "12:30 pm - 4:30 pm daily"
startdate: "2016-03-28"  # use YYYY-MM-DD format like "2015-01-01"
enddate: "2016-03-28"    # use YYYY-MM-DD format like" 2015-01-02"
instructor: ["Billy Charlton", "Suzanne&nbsp;Childress", "Brice&nbsp;Nichols", "Hana&nbsp;Ševčíková"]
helper: ['Peter Caballero, Stefan Coe']
contact: "bcharlton@psrc.org"
# etherpad: "https://public.etherpad-mozilla.org/p/psrc-scripting-workshop-2016"
eventbrite:       # optional (insert the alphanumeric key for Eventbrite registration, e.g., "1234567890AB")
---

<!--
  HEADER

  Edit the values in the block above to be appropriate for your workshop.
  If the value is not 'true', 'false', 'null', or a number, please use
  double quotation marks around the value, unless specified otherwise.
  And run 'tools/check' *before* committing to make sure that changes are good.
-->

<!--
  EVENTBRITE

  This block includes the Eventbrite registration widget if
  'eventbrite' has been set in the header.  You can delete it if you
  are not using Eventbrite, or leave it in, since it will not be
  displayed if the 'eventbrite' field in the header is not set.
-->
{% if page.eventbrite %}
<iframe
  src="https://www.eventbrite.com/tickets-external?eid={{page.eventbrite}}&ref=etckt"
  frameborder="0"
  width="100%"
  height="248px"
  scrolling="auto">
</iframe>
{% endif %}

<h2 id="general">General Information</h2>

<!--
  INTRODUCTION

  Edit the general explanatory paragraph below if you want to change
  the pitch.
-->

Hi there! Scripting Carpentry is a set of introductory workshops that can help get you up to speed on tools that will make your work day easier. This course is based on materials produced by [Software Carpentry]({{site.swc_site}}). Software Carpentry's mission is to help scientists and engineers get more research done in less
time and with less pain by teaching them basic lab skills for
scientific computing.

This hands-on workshop will cover basic
  concepts and tools, including program design, version control, data
  management, and task automation. Participants will be encouraged to
  help one another and to apply what they have learned to their own
  research problems.

<!--
  AUDIENCE

  Explain who your audience is.  (In particular, tell readers if the
  workshop is only open to people from a particular institution.
-->

<table><tr>
<td><b>Who:</b></td>

<td>The course is aimed at practitioners, researchers and data scientists in any technical field. <i>You don't need to have any previous knowledge of the tools that will be presented at the workshop.</i><br/><br/>This course is aimed at <i>novices</i>. If you are already comfortable with the command line, SQL, and python scripts, you probably do not need to take this class.</td></tr>

<td><b>Where:</b></td>

<td>{{page.address}}.<br/>Get directions with <a href="http://www.openstreetmap.org/?mlat={{page.latlng | replace:',','&mlon='}}&zoom=16">OpenStreetMap</a> or <a href="http://maps.google.com/maps?q={{page.latlng}}).">Google Maps</a></td>

<tr><td valign="top"><b>Requirements:</b></td>

<td>All participants will need to set up a few specific software packages on their computer <a href="#setup">(listed below)</a>.
<ul><li>If you are PSRC staff, set up the software on your <b>primary work desktop/laptop</b> in advance of the workshop day.</li>
<li>If you are not currently working at PSRC, <b>you must bring your own laptop</b>, set up with the software below.</li>
<li>All participants are also required to abide by the Software Carpentry <a href="{{site.swc_site}}/conduct.html">Code of Conduct</a>.</li>
</ul>
</td></tr>

</table>

Email Billy Charlton for more information.

------

## Syllabus

<div class="row">
  <div class="col-md-6">
    <h3 id="syllabus-shell"><span style="color:green;"><a href="http://psrc.github.io/novice-shell">Command-Line Ninja:<br/>The Bash Shell</a></span></h3>
    <i><span style="color:green;">March 21, 8:30am - 12:30pm</span></i>
    <ul>
      <li>Why learn the bash shell?</li>
      <li>Files and directories</li>
      <li>History and tab completion</li>
      <li>Linking programs with pipes and redirection</li>
      <li>Looping over files</li>
      <li>Creating and running shell scripts</li>
      <li>Finding things</li>
    </ul>
  </div>

  <div class="col-md-6">
    <h3 id="syllabus-git"><span style="color:green;"><a href="http://swcarpentry.github.io/sql-novice-survey">Version Control with Git</a></span></h3>
    <i><span style="color:green;">March 28, 12:30pm - 4:30pm</span></i>
    <ul>
      <li>Creating a repository</li>
      <li>Recording changes to files: <code>add</code>, <code>commit</code>, ...</li>
      <li>Viewing changes: <code>status</code>, <code>diff</code>, ...</li>
      <li>Ignoring files</li>
      <li>Working on the web: <code>clone</code>, <code>pull</code>, <code>push</code>, ...</li>
      <li>Collaborating with others</li>
      <li>Resolving conflicts</li>
      <li>Hosting files online using GitHub</li>
    </ul>
  </div>

</div>

<div class="row">
  <div class="col-md-6">
    <h3 id="syllabus-sql"><span style="color:green;"><a href="http://swcarpentry.github.io/sql-novice-survey/">Managing Data with SQL</a></span></h3>
    <i><span style="color:green;">March 29, 12:30pm - 4:30pm</span></i>
    <ul>
      <li>Reading and sorting data</li>
      <li>Filtering with <code>where</code></li>
      <li>Calculating new values on the fly</li>
      <li>Handling missing values</li>
      <li>Combining values using aggregation</li>
      <li>Combining information from multiple tables using <code>join</code></li>
      <li>Creating, modifying, and deleting data</li>
    </ul>
  </div>

  <div class="col-md-6">
    <h3 id="syllabus-r"><span style="color:green;"><a href="http://psrc.github.io/novice-r">Programming in R</a></span></h3>
    <i><span style="color:green;">April 5, 12:30pm - 4:30pm</span></i>
    <ul>
      <li>Learning the basics in R</li>
      <li>Working with vectors and data frames</li>
      <li>Reading and plotting data</li>
      <li>Creating and using functions</li>
      <li>Loops and conditionals</li>
      <li>Using R from the command line</li>
    </ul>
  </div>
</div>

<div class="row">
  <div class="col-md-6">
    <h3 id="syllabus-python"><span style="color:green;"><a href="http://psrc.github.io/novice-python-data-analysis">Programming in Python</a></span></h3>
    <i><span style="color:green;">April 18, 12:30pm - 4:30pm</span></i>
    <ul>
      <li>Introducing Python</li>
      <li>Working with arrays</li>
      <li>Reading and plotting data</li>
      <li>Creating and using functions</li>
      <li>Loops and conditionals</li>
      <li>Defensive programming</li>
      <li>Using Python from the command line</li>
    </ul>
  </div>

  <div class="col-md-6">
    <h3 id="syllabus-make"><span style="color:green;"><a href="http://psrc.github.io/novice-make">Automation with Make</a></span></h3>
    <i><span style="color:green;">April 19, 12:30pm - 4:30pm</span></i>
    <ul>
      <li>Introduction: why use a build tool?</li>
      <li>Makefiles: rules for building things</li>
      <li>Don't repeat yourself: automatic variables</li>
      <li>Dependencies on data and code</li>
      <li>Patterns, wildcards, and substitution rules</li>
      <li>Variables and Functions</li>
    </ul>
  </div>

</div>

<!--
  ETHERPAD

  At `_misc/etherpad.txt` you will find a template for the etherpad.

  Display the Etherpad for the workshop.  You can set this up in
  advance or on the first day; either way, make sure you push changes
  to GitHub after you have its URL.  To create an Etherpad, go to

      http://pad.software-carpentry.org/YYYY-MM-DD-site

  where 'YYYY-MM-DD-site' is the identifier for your workshop,
  e.g., '2015-06-10-esu'.
-->

------

## Setup

You MUST set up the following software before the class begins.

At the workshop, you will be using a laptop to remote control your primary work computer: that way, all the software setup can happen ahead of time, and all the software will be waiting for you when you get back to your desk after the workshop.

A reference list of common issues that occur during installation: [Configuration Problems and Solutions wiki page](https://github.com/swcarpentry/workshop-template/wiki/Configuration-Problems-and-Solutions).

---

### Windows Instructions

**Be sure to set up all six software items below on your primary desktop computer ahead of time -- before the day of the course.**

#### 1. Git and the 'Bash' Shell

Git lets you track and share changes made to files, and Bash is a command-line "shell" (command interpreter) that gives you the power to do simple tasks more quickly.

On Windows, the easiest way to get both Git and Bash is to use the Git for Windows installer.

* You need the **latest version of 64-bit Git**. Even if you already have Git installed on your PC, replace it with this new version.
* Be sure to select the correct installer options listed below!

Installation instructions for both Git and Bash:

1. Download the [Git for Windows Installer](https://git-for-windows.github.io).
2. Run the installer
3. Click on "Next" a few times to get to the "Adjusting your PATH environment" page.
4. Select **"Use Git from the Windows Command Prompt"** and click on "Next". If you forget to do this, programs that you need for the workshop *will not work properly.* If this happens, rerun the installer and select the appropriate option.
5. Keep **"Checkout Windows-style, commit Unix-style line endings"** selected. Click "Next".
6. Select **"Use Windows' default console window"** and click on "Next" and "Finish".

#### 2. ConsoleZ Command Terminal

[ConsoleZ](https://github.com/cbucher/console/wiki) is a much nicer terminal program that has a legible font, resizable window, and more. You'll use ConsoleZ to use the Bash program instead of using the "Git Bash" icon. Git Bash still works, but its window is janky.

* Download the [ConsoleZ Installer](/scripting-workshop-2016/setup/ConsoleZ-Installer.exe) and follow the default installer prompts.
* If Chrome or Firefox warns you that the installer file is untrusted, just go along with it. I created the installer here at PSRC and it is safe to install.
* ConsoleZ installer is also saved on the network, at *X:\DSA\Software*


#### 3. Text Editor

When you're writing scripts, it's nice to have a text editor that is optimized for code, with features like automatic indentation and color-coding of key words. MS Word and WordPad are bad choices because they are not designed for writing code. Do not use MS Word or WordPad for this class.

**Nano** is a basic text editor and is the default that instructors use in the workshop. If you do not already have a text editor that you prefer, use nano.

* To install nano, download the [Software Carpentry Windows installer](https://github.com/swcarpentry/windows-installer/releases/latest) and double click on the file to run it.
* **Other editors** in use at PSRC that you may want to try include [Notepad++](http://notepad-plus-plus.org) and [Sublime Text](http://www.sublimetext.com). Be aware that you must add the editor's installation directory to your system path. Please ask a coworker or your instructor for assistance if you don't know how to edit your system path.


#### 4. Python

[Python](http://python.org) is a great general-purpose programming language, and is one of the most popular tools for scientific computing as well. It has many optional packages called "libraries", and we use a lot of them at PSRC. Installing all of Python's scientific libraries individually can be a bit difficult, so we recommend [Anaconda](https://www.continuum.io/anaconda), an all-in-one installer.

**Make sure you install Python version 2.7**. If you have an older version of Python such as 2.6, you will probably need to uninstall it. Also we are not ready to move to Python 3 just yet. Don't install Python 3.

To install Anaconda Python 2.7:

* Open the Continuum Anaconda [download page](http://continuum.io/downloads) with your web browser.
* Download the Python 2.7 installer for Windows.
* Install Python 2.7 using all of the defaults -- and make sure to check **Make Anaconda the default Python**.

We will teach Python using the IPython notebook, a programming environment that runs in a web browser. For this to work, you will need an up-to-date browser. The current versions of the Chrome, Safari and Firefox browsers are all supported. Some older browsers, including Internet Explorer version 9 and below, are not.


#### 5. SQLite and Make

SQL is a programming language used with databases. Here at PSRC, we have existing enterprise databases in MS-SQL and MySQL, but those are a bit complex to set up for desktop use. For this workshop, we use a very simple database manager called [SQLite](http://www.sqlite.org). The SQL language is essentially identical, so the skills will all transfer -- and having a simple desktop version of SQL has its own benefits!

Make is a build tool that helps automate repetitive tasks.

* The [Software Carpentry Windows Installer](https://github.com/swcarpentry/windows-installer/releases/latest) installs SQLite and Make for Windows. If you already used the installer to install the nano text editor above, you don't need to run it again. Otherwise, run it now.

#### 6. R Statistics

[R](http://www.r-project.org) is a programming language that is especially powerful for data exploration, visualization, and statistical analysis. To interact with R, we use [RStudio](http://www.rstudio.com).

* Install R by downloading and running [this .exe file](http://cran.r-project.org/bin/windows/base/release.htm) from [CRAN](http://cran.r-project.org/index.html).
* Then install the [RStudio IDE](http://www.rstudio.com/ide/download/desktop).

#### 7. Check your setup

Important! Run these commands now, to ensure that all the previous steps worked correctly.

1. Download [swc-installation-test-1.py](/scripting-workshop-2016/setup/swc-installation-test-1.py)
2. Download [swc-installation-test-2.py](/scripting-workshop-2016/setup/swc-installation-test-2.py)
3. Open up a Bash shell by starting "ConsoleZ" or "Git Bash" on Windows, or "Terminal" on Mac
4. Change into the directory where you put the script by typing in the bash window:
   * <code>cd ~/Downloads</code>
5. To check you have the correct version of Python, run the script:
   * <code>python swc-installation-test-1.py</code>
   * If there are any errors, correct them now!
6. After verifying Python works, check that you have set up the other software requirements correctly. Run the script:
   * <code>python swc-installation-test-2.py</code>

If anything is missing, the script output will specify what needs to be corrected.

---

<!--
### Mac OS X

**Bash:** the default shell in all versions of Mac OS X is Bash, so no need to install anything.

* You access Bash from the Terminal
        (found in <code>/Applications/Utilities</code>). You may want to keep Terminal in your dock for this workshop.

**Git:** For OS X 10.9 and higher, install Git for Mac by downloading and running the most recent "mavericks" installer from
        [this list](http://sourceforge.net/projects/git-osx-installer/files/). After installing Git, there will not be anything in your <code>/Applications</code> folder, as Git is a command line program.

* For older versions of OS X (10.5-10.8), use the most recent available installer labelled "snow-leopard" [available here](http://sourceforge.net/projects/git-osx-installer/files).

**Python:** We recommend the Continuum Ananconda Python all-in-one python installer, which installs a basic Python system as well as the scientific computing modules required for this course.

* Open [http://continuum.io/downloads](http://continuum.io/downloads) with your web browser.
* Download the Python 2.7 installer for OS X.  We are not using Python 3 yet.
* Install Python 2.7 using all of the defaults for installation.

**SQLite**. SQLite comes pre-installed on Mac OS X.

**R** Statistics software.

* Install R by downloading and running [this .pkg file](http://cran.r-project.org/bin/macosx/R-latest.pkg) from [CRAN](http://cran.r-project.org/index.html).
* Also install the [RStudio IDE](http://www.rstudio.com/ide/download/desktop).

### Linux

Use your system's package manager to install python, sqlite, git, r, make, and nano.

-->
