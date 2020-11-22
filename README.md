![the shiny app tutorials project](shinytutorials.png)

# shinyTutorials

This repo contains the code for the examples and demonstrations presented on my shiny tutorials site: [davidruvolo51.github.io/shinytutorials/](https://davidruvolo51.github.io/shinytutorials/).

<!-- TOC depthFrom:2 -->

- [Motivation](#motivation)
- [Tutorials](#tutorials)
    - [Cloning Tutorials](#cloning-tutorials)
    - [Available Tutorials](#available-tutorials)
    - [Archived Tutorials](#archived-tutorials)
- [Resources](#resources)
    - [Communities](#communities)
    - [Courses](#courses)
    - [Web Accessibility](#web-accessibility)
    - [Web Development](#web-development)
- [Contributing to this project](#contributing-to-this-project)

<!-- /TOC -->

## Motivation

In my early days of learning shiny, I kept a document of all my tips and tricks. It worked nicely, but it quickly became too cluttered and scattered. I decided to create this project to organize the material in to a series of practical examples and to make it available for the wider R community.

My interests are in web accessibility, data visualization and communication of results, and good design practices. Many of these tutorials focus heavily on HTML, CSS, and JavaScript, but I will try to keep things simple and provide links for further reading. Suggestions, comments, ideas for improvement are always welcome!

## Tutorials

I plan on developing a new Shiny app every now and then. Checkout the issues label `Tutorial Ideas` for examples that I'm currently developing. If you have an idea, feel free to open a new issue.

All *live* examples can be found in the [Available Tutorials](#available-tutorials) table. The *archived* example apps listed in the [Archived Tutorials](#archived-tutorials) section. These examples still work, but the methods are outdated or the example was replaced by a newer one.

### Cloning Tutorials

You can clone the entire repository, but be aware that you will also clone the entire git history. You can either download the files or folders that you want or use `git sparse-checkout`. In the terminal, run the following commands.

```bash
git clone --filter=blob:none --sparse https://github.com/davidruvolo51/shinyAppTutorials
cd shinyAppTutorials
git sparse-checkout init --cone
git sparse-checkout set drag-and-drop
```

Switch `drag-and-drop` for the subdirectory(ies) that you wish to checkoout. For more information, checkout the GitHub blog post: [Bring your monorepo down to size with sparse-checkout](https://github.blog/2020-01-17-bring-your-monorepo-down-to-size-with-sparse-checkout/). Be aware that this is slightly experimental and these instructions may change.

### Available Tutorials

<!-- begin:activeTutorials -->

|name                        |description                                      |version |link                                                                                          |
|:---------------------------|:------------------------------------------------|:-------|:---------------------------------------------------------------------------------------------|
|Data editor                 |A shiny app for editing dataset in shiny         |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/data-editor/)             |
|Drag and drop               |create a drag and drop component                 |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/drag-and-drop/)           |
|Get window dimensions       |sending data from javascript                     |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/get-window-dims/)         |
|JS handlers                 |getting started with custom handlers             |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/js-handlers/)             |
|Loading screens for leaflet |creating a loading screen for leaflet            |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/leaflet-loading-screens/) |
|login screen                |Adding *basic* user authentication to shiny apps |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/login-screen/)            |
|R6 progress bars            |Create a progress bar component using R6 classes |1.0.0   |TBD                                                                                           |
|Responsive Datatables       |Optimize datatables for all screens              |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/responsive-tables/)       |
|Rmarkdown in Shiny          |Using Rmd files as Shiny UI                      |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/rmarkdown-shiny/)         |
|SASS in Shiny               |Getting started with SASS                        |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/sass-in-shiny/)           |
|Setting HTML Attributes     |Modifying `<html>` attributes                    |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/setting-html-attributes/) |
|Landing Pages               |Create cool landing pages in Shiny apps          |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/landing-page/)            |
|Shiny Links                 |Creating links to other pages in a shiny app     |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/shiny-link/)              |
|Shiny Listbox               |Create a customizeable dropdown menu for shiny   |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/listbox-widget/)          |
|Time Inputs                 |Getting started with shiny input bindings        |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/time-input/)              |

<!-- end:activeTutorials -->

### Archived Tutorials

The examples listed in the following table are achived. They still work, but they are either outdated or were replaced by a newer example. (I'm a bit hesitant to remove these examples in case some follows a link to a page that doesn't exist.)

<!-- begin:archivedTutorials -->

|name                    |description                                        |version |link                                                                                       |
|:-----------------------|:--------------------------------------------------|:-------|:------------------------------------------------------------------------------------------|
|Internal Links (Part 1) |Create links from one shiny page to another        |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/internal-links-a/)     |
|Internal Links (Part 2) |Create a link from a leaflet popup to a shiny page |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/internal-links-b/)     |
|Internal Links (Part 3) |Navigate to a specific tab on another page         |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/internal-links-c/)     |
|Select input styling    |Style a select input element using CSS             |1.0.0   |[tutorial](https://davidruvolo51.github.io/shinytutorials/tutorials/select-input-styling/) |

<!-- end:archivedTutorials -->

The internal links examples are outdated. Instead, use the `shinyLink` component described in the [Shiny Link](https://github.com/davidruvolo51/shinyAppTutorials/tree/prod/shiny-links) subdirectory (02 August 2020).

## Resources

Many of the tutorials rely heavily on HTML, CSS and JavaScript to create specific layouts and interactivity. These are good skills to have, and they will come in handy when building custom applications. Throughout the examples, I've tried to keep things simple and provide links to outside sources where applicable. If something isn't clear or you have suggestions for improvement, feel free to open a new issue.

If you would like to learn more, here are some links that you may find useful.

### Communities

- [Data Visualization Society](https://www.datavisualizationsociety.com)
- [dev.to](https://dev.to)
- [RStudio Community](https://community.rstudio.com)
- [r/rstats](https://www.reddit.com/r/rstats/)
- [r/rshiny](https://www.reddit.com/r/rshiny/)
- [Twitter #rstats](https://twitter.com/hashtag/rstats)

### Courses

- [W3C Online Courses](https://www.edx.org/school/w3cx) (free on [edx.org](https://www.edx.org))

### Web Accessibility

- [a11y project](https://a11yproject.com)
- [Accessibility Developer Guide](https://www.accessibility-developer-guide.com)
- [Mozilla's Learn Accessibility](https://developer.mozilla.org/en-US/docs/Web/Accessibility)
- [macOS Voice Over Commands](https://help.apple.com/voiceover/command-charts/)
- [WAI's Web Accessibility Tutorials](https://www.w3.org/WAI/tutorials/)
- [Web Accessibility Initiative](https://www.w3.org/WAI/)

### Web Development

- [CSS Tricks](https://css-tricks.com)
- [Mozilla's CSS documentation](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [Mozilla's Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)
- [Mozilla's Learn HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML)
- [Mozilla's Learn JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
- [Resources for Front-End Beginners](https://github.com/thedaviddias/Resources-Front-End-Beginner)

## Contributing to this project

I plan on writing an example once in a while. Check open issues for the label `tutorial ideas`. Comments and suggestions are always welcome. If you would like to add your own tutorial, that would be wonderful! Get in touch with me by opening a new issue and checkout the [Contributing Guidelines](https://github.com/davidruvolo51/shinyAppTutorials/blob/master/CONTRIBUTING.md) for more information.
