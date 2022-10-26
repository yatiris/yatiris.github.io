# Yatiris lab website

This is repository for [Yatiris website](http://yatiris.github.com/). Most of the code comes from [http://kordinglab.com/], which uses Jekyll to run a Github page. We are welcome for other people to contribute to our site not just lab members. Feel free to fork and pull-request!


## Run the page locally

To run locally, follow instruction [here](https://jekyllrb.com/) to install Jekyll then run `bundle exec jekyll serve` to see in `localhost:4000`.


## Add posts

It's very easy to add post. All the posts are located in `_posts` folder. It arrangement is based on
date. Each post can be written in markdown format. You just have to state headers before writing: `title`, `description` and `categories`. `description` will be shown when you share on social media like Facebook or twitter. See the following headers:

```
---
title: SIPAIM
description: all links to the conference SIPAIM
categories: scientists
---
```

We have 4 categories: `scientists`, `students`, `discussion`, `news` you can choose and this will be rendered to different location.


## How to add posts


- **Directly edit on Github**, you can simply go to `_posts` and click `New file` then put some markdown file e.g. `2016-02-03-post-name.md` and start writing news post. Github also allows you to preview it so it's nice for people who don't want to clone the repo. 

- **Clone the repository**, kind of the same as directly add post on Github. You just have to clone the repository. Then add new post file, commit and push to the repo.

The changes will take approximately half a minute to render. You can see the new posts or changes on [yatiris.github.io](http://yatiris.github.io/)!


## Add yourself

You can add yourself to the page in `_people` folder just create file name `<firstname>_<lastname>.md` in the folder. We require few line of header before you start writing your own page. See the following for the header

```
---
name: Eva Dyer
position: postdoc
avatar: eva.jpg
twitter:
joined: 2014
---
```

If you don't have information, just leave it blank. The avatar will bring photo from `images/people` folder and display it on people page. 
For lab position, you can choose position from 4 classes including `postdoc`, `gradstudent`, `visiting`, `others` (so called Honorary members). Position will put you into section that you choose.

## Add new publications

All publications from the lab are located in `publications.md`. Please upload new publication on your own!


## Add a new Thesis to our archive

You can add your proposals to the web just by creating a file `<YYYY>-<MM>-<DD>-thesis-spa.md` inside the `_thesis` folder. We require the file to have a few lines of information:

```
---
title: My thesis
description: PhD Thesis 
header-img: images/tesis-grado/<filename>.png
categories: [tesis-grado/tesis-doctorado]
---
```

Below this header, you may add the abstract or description of your work.

## Add Project proposals

You can add your proposals to the web just by creating a file `<YYYY>-<MM>-<DD>-tfi-<yourname>.md` inside the `_tfi` or `_phd` folder. We require the file to have a few lines of information:

```
---
title: Title of your proposal
categories: [propuestas-tfi | propuestas-phd]
header-img: <filename>.png
referent: "<your name>"
contact: <your e-mail>
state: [open | closed]
description: <Description of project proposal>
---
```

The image should illustrate the topic of the project and the file should be added to `images/tfi/` or `images/phd/`. Set state to `closed` when the project has been assigned to a student. Please bear in mind that these proposals should be in Spanish.
