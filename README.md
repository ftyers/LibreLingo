<h1 align="center">
<img src="logo_for_readme.svg" alt="LibreLingo" /></h1>
<p align="center"><em>an experiment to create a community-driven language-learning platform</em></p>


[Click here for live demo](https://librelingo.app/)

## Project goal

My goal is to start a community-driven language-learning platform that gives it's users and contributors a way to influence it's future and adapt it to special requirements.

To achieve that, I release all source code under the GPLv3 free software license, which guarantees end users the freedom to run, study, share, and modify the software.

In addition to licensing the software under a free software license, the course content will be decoupled from the software itself, and the development of GPLv3 or public domain course content will be encouraged. This should allow course developers to retain the freedom to choose how they use their work.

Once course content is properly decoupled from the software, it should be possible to experiment with alternative ways of using course content: for example, the creation of audiobooks or print material.

## Screenshots

<div align="center">
    <img src="/screenshots/screenshot1.png" width="400px"></img> 
    <img src="/screenshots/screenshot2.png" width="400px"></img> 
    <img src="/screenshots/screenshot3.png" width="400px"></img> 
    <img src="/screenshots/screenshot4.png" width="400px"></img> 
</div>


## Milestones

Here's a rough sketch of how  I imagine the milestones of this project:

### First demo

* ☑️ Demo course content in Spanish for English speakers
* ☑️ Some basic building blocks of course content implemented
* ☑️ Developers can use course editor
* ☑️ Basic theme/branding

### Alpha release

* ☐ Course progress can be properly syncronised across devices
* ☐ Course editor can be accessed by all course contributors
* ☐ Statistics about course controbutors are collected and published
* ☐ At least the basics of the Spanish course are ready
* ☐ Most of the course building blocks are implemented


### Beta release

* ☐ All of the basic building blocks of courses are implemented
* ☐ More advanced learning features (reading exercises)
* ☐ Spaced repetition implemented
* ☐ Spanish course is stable and useful

### Stable release(s)

* ☐ Any user can build their own course
* ☐ Users can suggest changes to course content
* ☐ There's a marketplace for "unofficial" courses
* ☐ Multiple stable courses available
* ☐ Mobile apps available
* ☐ Wiki features
* ☐ Dictionary
* ☐ Speaking exercises

## Become a contributor

### Contribute to course material
If you are interested in contributing to course development, please fill the following form: https://danielkantor196881.typeform.com/to/V00Paz. The project is in a very early stage right now, so you might not be able to contribute right away. Your work will be released in this GitHub repository and you will show up as a contributor here.

### Contribute to software development
If you are interested in writing code for LibreLingo, you can simply start submitting pull requests. You can also use this form to get in touch: https://danielkantor196881.typeform.com/to/jTe9jX. **You don't _need_ to fill this form. You can just start submitting issues and pull requests if your wish!**

### Other forms of contribution
You can help LibreLingo by testing it and submitting feature requests or bug reports: https://github.com/kantord/LibreLingo/issues/new. If you want to get in touch, you can simply the contacts on [my GitHub profile](https://github.com/kantord).

## Tech stack

​       | Web app/PWA   | Course editor |
--------| ------------- | ------------- |
Frontend| Svelte        | Django Admin* |
Backend | CouchDB       |               |

\* Djando Admin might be replaced in the future

Testing is done using Jest and Cypress. Other technology in use include: bulma, webpack, etc.

## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fkantord%2FLibreLingo.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fkantord%2FLibreLingo?ref=badge_large)

## Development

### Running the project in development mode

If you have cloned the repo and have `yarn` installed on your computer, you can install dependencies and run the development server using:

```
yarn
yarn dev
```

### Deploying to production

LibreLingo's frontend is a static site, therefore you can simply deploy it using the static HTTP server of your choice!

To generate the static files (assuming that you have set up a working development mode), you just have to export them using:

```
yarn export
```

This will create a `__sapper__/export` folder with a production-ready build of your site.

See Sapper's documentation for more detail: https://sapper.svelte.dev/docs#Exporting


### Using the course editor

The course editor is in a very early stage, and is only usable by developers. Since it's not publicly hosted yet, you can only use it for testing purposes.

The course editor is implemented as a django project in the `course_editor` folder.

If you want to set up your course editor with real data, you can find a database dump here: `src/courses/spanish-from-english/courseData.json`

Check out Django's documentation about database dumps: https://docs.djangoproject.com/en/3.0/ref/django-admin/#loaddata

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://www.daniel-kantor.com/cv/"><img src="https://avatars2.githubusercontent.com/u/3704904?v=4" width="100px;" alt=""/><br /><sub><b>Daniel Kantor</b></sub></a><br /><a href="https://github.com/kantord/LibreLingo/commits?author=kantord" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/aha999"><img src="https://avatars3.githubusercontent.com/u/50620416?v=4" width="100px;" alt=""/><br /><sub><b>Klemen Skerbiš</b></sub></a><br /><a href="#ideas-aha999" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/12people"><img src="https://avatars0.githubusercontent.com/u/7361228?v=4" width="100px;" alt=""/><br /><sub><b>Mirek Mazel</b></sub></a><br /><a href="#ideas-12people" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="http://tbg.asciiking.com/about.html"><img src="https://avatars0.githubusercontent.com/u/12728?v=4" width="100px;" alt=""/><br /><sub><b>Chris Babcock</b></sub></a><br /><a href="#ideas-swift2plunder" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="http://wake.st"><img src="https://avatars2.githubusercontent.com/u/7890201?v=4" width="100px;" alt=""/><br /><sub><b>Liaizon Wakest</b></sub></a><br /><a href="#ideas-wakest" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/schmittlauch"><img src="https://avatars3.githubusercontent.com/u/1479555?v=4" width="100px;" alt=""/><br /><sub><b>Trolli Schmittlauch</b></sub></a><br /><a href="#ideas-schmittlauch" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://deuchnord.fr"><img src="https://avatars3.githubusercontent.com/u/7600265?v=4" width="100px;" alt=""/><br /><sub><b>Jérôme Deuchnord</b></sub></a><br /><a href="#ideas-Deuchnord" title="Ideas, Planning, & Feedback">🤔</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://gitea.nutomic.com/nutomic"><img src="https://avatars1.githubusercontent.com/u/1044450?v=4" width="100px;" alt=""/><br /><sub><b>Felix Ableitner</b></sub></a><br /><a href="https://github.com/kantord/LibreLingo/issues?q=author%3ANutomic" title="Bug reports">🐛</a></td>
    <td align="center"><a href="http://navanchauhan.me"><img src="https://avatars1.githubusercontent.com/u/29234112?v=4" width="100px;" alt=""/><br /><sub><b>Navan Chauhan</b></sub></a><br /><a href="#infra-navanchauhan" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
    <td align="center"><a href="http://roshanjossey.github.io"><img src="https://avatars0.githubusercontent.com/u/8488446?v=4" width="100px;" alt=""/><br /><sub><b>Roshan Jossy</b></sub></a><br /><a href="#ideas-Roshanjossey" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/ledgelight"><img src="https://avatars0.githubusercontent.com/u/57244557?v=4" width="100px;" alt=""/><br /><sub><b>ledgelight</b></sub></a><br /><a href="#ideas-ledgelight" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="http://xixona.dlsi.ua.es/~fran/"><img src="https://avatars3.githubusercontent.com/u/449545?v=4" width="100px;" alt=""/><br /><sub><b>Francis Tyers</b></sub></a><br /><a href="#ideas-ftyers" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://netspring.wordpress.com"><img src="https://avatars0.githubusercontent.com/u/7551116?v=4" width="100px;" alt=""/><br /><sub><b>titanix</b></sub></a><br /><a href="#ideas-titanix" title="Ideas, Planning, & Feedback">🤔</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

