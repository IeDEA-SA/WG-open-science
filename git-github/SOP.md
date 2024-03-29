<img align = "right" width = "200" height = "200" src = "logo.png">


# **Standard Operating Procedures for version control using Git & GitHub within IeDEA-SA**

***Authors***: @RPanczak, @elianerohner, @rkassanjee, @aezaniewski, @LilianSmith, @pervongroote, Kathleen Kehoe, ..., on behalf
of *[IeDEA-SA Open Science Working Group](https://github.com/orgs/IeDEA-SA/teams/wg_open-science)*

<font size = "2">
 
*Reviewed by:* @jriou, ...

*Approved by:* @jriou, ...

*Version:* 0.5

*Valid from:* **TBC**

*Last revision:* 2022-02-16

*Location of SOP:*  
  - locally: ..\\OneDrive - Universitaet Bern\\IeDEA
Collaboration\\Projects & WGs\\Open Science  
  - [online](https://unibe365-my.sharepoint.com/:w:/g/personal/smith_campus_unibe_ch/EbpDaD2q8SFDs6F70jFwwMUB3d_CIdePn-Cw6CWraJZZyQ?e=0r2hPH)  

*Revision index:*

| ***Version*** | ***Summary of changes*** | ***Reason for change(s)***                               |
| ------------- | ------------------------ | -------------------------------------------------------  | 
|  0.1          |     1st draft            | NA                                                       |
|  0.2          |     2nd draft            | Including WG's comments                                  |
|  0.3          |     3rd draft            | Including team's comments                                |
|  0.4          |     4th draft            | @RPanczak moved to md; split code review and replication |
|  0.5          |     5th draft            | @RPanczak more on communication; added definitions       |


</font>

<font size = "3">

------------------------------------------------------

**Table of Contents**  

[General information](#general-information)  

[Implementation](#implementation)  

[Quality control](#quality-control)  

[Communication](#communication)  


</font>

------------------------------------------------------

## General information  

This document provides general resources on **version control** using **Git** and **GitHub** and briefly describes when and how to implement version control in International epidemiology Databases to Evaluate AIDS Southern Africa (IeDEA-SA) research projects.  

The main goal of implementing version control of the code used to produce scientific outputs of the IeDEA-SA group is to serve as an institutional memory that documents and preserves the development of analytical workflows, communication and decisions made during conducting og the analyses by team members.  

We believe that the processes of saving and sharing the code in a searchable manner will facilitate better transparency and communication and lead to:  

- increased ***collaboration*** by allowing team members to discover who works on what using which software and methods  

- improved ***quality of analyses*** by allowing team members to learn from more experienced colleagues and from previously conducted work  

- reduced ***errors*** in the code by allowing more experienced team members to review and contribute to the code,  

- increased ***efficiency*** by allowing team members to identify and avoid ***duplication*** of effort within the team  

- increased ***visibility*** of the research and the group within IeDEA-SA and, if shared publicly, with IeDEA partners and external researchers  

- project ***knowledge preservation*** versus only archiving information.  

### Definitions

Here are some excerpts from the FORRT [glossary](https://forrt.org/glossary/).  

1. Reproducibility:  

> A minimum standard on a spectrum of activities (“reproducibility spectrum”) for assessing the value or accuracy of scientific claims based on the original methods, data, and code. For instance, where the original researcher’s data and computer codes are used to regenerate the results (Barba, 2018), often referred to as computational reproducibility. Reproducibility does not guarantee the quality, correctness, or validity of the published results (Peng, 2011). In some fields, this meaning is, instead, associated with the term 'replicability' or ‘repeatability’.

2. Computational reproducibility:  

> Ability to recreate the same results as the original study (including tables, figures, and quantitative findings), using the same input data, computational methods, and conditions of analysis. The availability of code and data facilitates computational reproducibility, as does preparation of these materials (annotating data, delineating software versions used, sharing computational environments, etc). Ideally, computational reproducibility should be achievable by another second researcher (or the original researcher, at a future time), using only a set of files and written instructions. Also referred to as analytic reproducibility (LeBel et al., 2018).

3. Version control:  

> The practice of managing and recording changes to digital resources (e.g. files, websites, programmes, etc.) over time so that you can recall specific versions later. Version control systems are designed to record the history of changes (who, what and when), and help to avoid human errors (e.g. working on the wrong version). 

4. Git:  

> A software package for tracking changes in a local set of files (local version control), initially developed by Linus Torvalds. In general, it is used by programmers to track and develop computer source code within a set directory, folder or a file system. Git can access remote repository hosting services (e.g. GitHub) for remote version control that enables collaborative software development by uploading contributions from a local system. This process found its way into the scientific process to enable open data, open code and reproducible analyses.


### Version control software and online code hosting  

1. We primarily **use and recommend [git](https://git-scm.com/)** as a version control *software*.  

2. We primarily **use and recommend [GitHub](https://github.com/)** as an on-line code *hosting* and *collaboration platform* provider.  

### Teaching & learning materials  

1. Past ISPM course:  

    1. Session I: Git and GitHub: get your files under control! ([Slides](https://unibe365-my.sharepoint.com/:p:/r/personal/smith_campus_unibe_ch/Documents/IeDEA%20Collaboration/Projects%20%26%20WGs/Open%20Science/Course%20Materials/gitcourse_part1.pptx?d=wf9624a839d4c4b0780550848ee18af2d&csf=1&web=1&e=Cpxbkm); [Recording](https://unibe365-my.sharepoint.com/:v:/r/personal/smith_campus_unibe_ch/Documents/IeDEA%20Collaboration/Projects%20%26%20WGs/Open%20Science/Course%20Materials/GMT20210602-061802_Recording_1920x900.mp4?csf=1&web=1&e=MijnGx))  

    2. Session II: Git and GitHub: get your files under control! ([Slides](https://unibe365-my.sharepoint.com/:p:/r/personal/smith_campus_unibe_ch/Documents/IeDEA%20Collaboration/Projects%20%26%20WGs/Open%20Science/Course%20Materials/gitcourse_part2.pptx?d=wbfbae843947e4e69992f09f08f12c7c5&csf=1&web=1&e=kQDw6k); [Recording](https://unibe365-my.sharepoint.com/:v:/r/personal/smith_campus_unibe_ch/Documents/IeDEA%20Collaboration/Projects%20%26%20WGs/Open%20Science/Course%20Materials/GMT20210608-062040_Recording_1760x900.mp4?csf=1&web=1&e=WhQV4p))    

2. In person courses might be offered by:

    1. CH:  
        1.[SIB](https://www.sib.swiss/)  
        2. [UniBe](https://www.scits.unibe.ch/training/training_and_workshops/)  

    2. SA:
        1. ...  

3. GitHub short courses:  

    1. [Introduction to GitHub](https://lab.github.com/githubtraining/introduction-to-github)  
    2. [Uploading your project to GitHub](https://lab.github.com/githubtraining/uploading-your-project-to-github)  

4. Coursera courses:  

    1. [Introduction to Git and GitHub](https://www.courser1.org/learn/introduction-git-github)  
    2. [Version Control with Git](https://www.courser1.org/learn/version-control-with-git)  
    
5. Carpentries courses: 
    1. [Introduction to Git](https://librarycarpentry.org/lc-git/) 
    2. [Version Control with Git](https://swcarpentry.github.io/git-novice/)

6. Tutorials:  

    1. Ten Simple Rules for Taking Advantage of Git and GitHub [article](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004947)
    2. A Quick Introduction to Version Control with Git and GitHub [article](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004668)  
    3. Atlassian [tutorials](https://www.atlassian.com/git/tutorials)  
    4. Slightly longer [tutorial](https://www.toolsqa.com/git/git-tutorial/) from ToolsQA

7. Books:  

    1. [Conversational Git](http://blog.anvard.org/conversational-git/)  
    2. [Happy Git and GitHub for the useR](https://happygitwithr.com/)  
    3. [Pro Git](https://git-scm.com/book/en/v2)  

8. Cheat sheets:  

    1. GitHub's [cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)  
    2. GitLab's [cheatsheet](https://about.gitlab.com/images/press/git-cheat-sheet.pdf)  

### Institutional points of contact

1. [Radoslaw Panczak](mailto:radoslaw.panczak@ispm.unibe.ch), [Julien Riou](mailto:julien.riou@ispm.unibe.ch) and [Yann Ruffieux](mailto:yann.ruffieux@ispm.unibe.ch) \@UniBe  

2. ... \@UCT  

------------------------------------------------------

## Implementation

### Repository naming conventions

1. Projects that **carry a concept sheet number** should use it as the name prefixed with `IeDEA`. Examples of correctly named repositories are:

    1. `IeDEA_SA000` for regional projects  

    2. `IeDEA_MR000` for multiregional projects  

2. When projects **do not yet have a concept sheet number** use the `IeDEA` prefix mentioned above with one to two words added to describe the project. Please note that the repositories' names should be changed to the concept sheet number once assigned. Examples of projects without concept sheet numbers are:

    1. `IeDEA_ART` (draft [project](https://github.com/IeDEA-SA/IeDEA_ART) focused on the ATC codes of antiretroviral medications)  

    2. `IeDEA_DTG` (early stage [project](https://github.com/IeDEA-SA/IeDEA_DTG) focused on the exploration of DTG use in \@IeDEA-SA)  

3. Same logic applies to projects that will (most likely) **never be assigned a concept sheet number**. Examples are:  

    1. [`IeDEA_data-mgmt`](https://github.com/IeDEA-SA/IeDEA_data-mgmt) (project focused on documenting approaches to data preparation)  

    2. [`IeDEA_analyse`](https://github.com/IeDEA-SA/IeDEA_analyse)** (project focused on preparation of a simplified, 'analyse' ready dataset)

4. Please **adhere** to *strict naming conventions* for repositoriesand try and be consistent. Unleash your creativity on writing beautiful code and engaging prose, not reinventing naming conventions.  

### Ownership options

1. We recommend choosing **organization [\@IeDEA-SA](https://github.com/IeDEA-SA)** to own the repository containing the work. You will still be recognized as the main contributor. The URL format of projects then becomes:  

  `https://github.com/IeDEA-SA/IeDEA_SA217`  

2. Alternatively, you can choose to **personally** own the repositories containing materials of your IeDEA related projects as long as you inform the open science working group about the location of the project, update the [directory](https://github.com/IeDEA-SA/.github/blob/main/profile/README.md) and enable read access for all **[\@IeDEA-SA](https://github.com/IeDEA-SA) organisation** members. The URL format of projects then becomes:  

  `https://github.com/RPanczak/ISPM_excess-mortality`  

3. The ownership of the repositories can be **transferred** between the users. For instance, private repository can be transferred to **[\@IeDEA-SA](https://github.com/IeDEA-SA) organisation** and vice vers1.

### Depositing code

1. **At minimum,** once a project is completed, the lead author should **deposit all, final analytical code** with appropriate documentation in a repository which is owned and named following the guidelines described above. Ideally and whenever possible, this is **accompanied by datasets and metadata** deposited in an open or institutional data repository that would also allow running this code.  

2. **Ideally,** the **complete development** of the analytic code should be documented from the first to the final version. Major additions and modifications of the code should be tracked using version control features such as 'commits', 'issues' and 'releases' to document communication and decisions taken by the team members along the way.  

3. **The lead author** or a person designated by the lead author is responsible for implementing the processes defined above, **latest** upon completion of the project.  

### Accessibility

1. **At minimum,** each project should be **accessible to the [@IeDEA-SA open science working group](https://github.com/orgs/IeDEA-SA/teams/wg_open-science/members)** upon completion.  

2. **Ideally,** the project is made available to the **entire @IeDEA-SA organisation** upon completion. This is the default behaviour for projects created within organisation or transferred there.  

3. **Projects owned by other GitHub users** **should at minimum add members of the \@IeDEA-SA organization** to the repository and enable 'read' access for them.  

4. **Whenever possible,** the project's code should be **made publicly available** and **a link to the repository should appear in all related publications.**  

### Licensing & code reuse

1. We encourage the repository owners to specify **conditions under which they allow the code to be reused**.  

2. [Creative Commons](https://creativecommons.org/) licensing's philosophy and vocabulary can be used to describe how the authors wish the code to be (re)used. In particular:  

    1. **`BY`** clause can be used to indicate that the authors wish to be credited if the code is reused  

    2. **`SA`** (share alike) clause can be used to indicate that adapted code should be distributed under the same reuse rights as the original code  

3. If no license is specified, we will assume the **conservative option of a BY-SA** type of licence to promote fair attribution and openness.  

4. The lead author should **agree on these conditions with the senior author** prior to depositing any code, particularly publicly.  

5. If code with a 'BY' clause is reused, the **original author** should be **contacted** by the lead and senior authors of the current project to discuss the appropriate form of **acknowledgement**, citation, and potential authorship involvement in a new project.  

------------------------------------------------------

## Quality control

### Code review

1. At the request of the project's team, analytical code deposited prior to publication can undergo [code review](https://en.wikipedi1.org/wiki/Code_review) process.  

2. *Upon approval of resources and resolution of authorship contribution by one of the project leads* another analyst will review the analyses to assure quality and spot potential errors or inefficiencies.  

3. The lead and senior authors should inform the open science working group about the intention of the review process *at the early stage of the project* in order to facilitate resources planning  

4. The lead and senior authors should discuss the level of involvement of the reviewer and the form of attribution (in the repository `README` and in the publication) *prior to the review process*  

### Internal replication

1. At the request of the project's team, analytical code deposited prior to publication can undergo an [internal replication](https://gatesopenresearch.org/articles/4-17) process.  

2. *Upon approval of resources and resolution of authorship contribution by one of the project leads* another analyst will attempt to replicate the complete analyses to assure quality and reproducibility.  

3. The lead and senior authors should inform the open science working group about the intention of the replication *at the early stage of the project* in order to facilitate resources planning  

4. The lead and senior authors should discuss the level of involvement of the reviewer and the form of attribution (in the repository `README` and in the publication) *prior to the review process*   

------------------------------------------------------

## Communication

### GitHub issues

1. [GitHub issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues) should be used to communicate and discuss unsolved or newly discovered problems.

2. Open science working group members will collect and monitor unsolved issues and help in finding and assigning them to persons that might be able to contribute to the solution.

3. The same rules of attribution as discussed in section 5 of the *Licensing & code reuse* should be followed if collaborators make substantial contributions at the stage of the code review.

4. Boards

### GitHub wiki

### GitHub discussions
