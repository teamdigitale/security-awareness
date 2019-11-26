[![License](https://img.shields.io/github/license/teamdigitale/security-awareness.svg)](https://github.com/teamdigitale/security-awareness/blob/master/LICENSE) [![GitHub issues](https://img.shields.io/github/issues/teamdigitale/security-awareness.svg)](https://github.com/teamdigitale/security-awareness/issues) [![Join the #design channel](https://img.shields.io/badge/Slack%20channel-%23security-blue.svg)]( https://developersitalia.slack.com/archives/C7BB7SX4P/) [![Get invited](https://slack.developers.italia.it/badge.svg)](https://slack.developers.italia.it/) [![sicurezza on forum.italia.it](https://img.shields.io/badge/Forum-sicurezza-blue.svg)](https://forum.italia.it/c/sicurezza)

# Security awareness
> Attention: This is not a course like many others! The digital security course (or “security awareness”) that you are about to start will allow you to find out what are the correct behaviors to keep to manage information securely.

- [How to start](#how-to-start)
- [How to contribute](#how-to-contribute)
- [Translate the course](#translate-the-course)

![Security Awareness](https://teamdigitale.github.io/security-awareness/img/picture-home.png)

# How to start
A simple compatct web site based on [Hugo CMS](https://gohugo.io) and is based on the following [bootstrap theme](https://github.com/francescozaia/hugo-theme-bootstrap-italia).

To install hugo follow the [following steps](https://gohugo.io/getting-started/quick-start/).

##### Mac
```
brew install hugo
```
##### Linux
```
apt-get install hugo
sudo dnf install hugo
```

In order to recreate the web site 
```
hugo
```
to launch the site locally 

```
hugo serve
```

Check the logs in order to see the correct URL and port (as example);
```
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/security-awareness/ (bind address 127.0.0.1)
```

# How to contribute
Contributions are always welcome! If you find some problems or glitches when using the app, we warmly encourage you to file an issue using GitHub's issue tracking feature. However, the CONTRIBUTING.md file located inside the root of the repo provides insightful details about how to collaborate in an efficient way with the community.

# Translate the course
If you want to add a language to this site, you can follow these steps:

1. Add a language in the file `config/_default/languages.yaml`, for instance for Spanish:
   ```
   es:
     urlPrefix: 'es/'
     languageName: ESP
     weight: 3
     contentDir: content/es
   ```
2. Add an image with the flag of the corresponding language in `static/img/lang` with the proper name. For instance for Spanish: `ESP.png`

3. Create a new file in the folder `i18n` (for instance `es.yaml`) by coping the English file `i18n/en.yaml` and translate all texts.

4. Copy all the content of `content/en` folder to a new folder (for instance `content/es`) and proceed to translate all relevant texts. All the vingettes and images can be found in a version without any text in the folder `images-languages`. You can use that version to add the texts in your language for transaltion.

5. Test the correct translation of all parts.

6. Create a pull request to propose the translation to the project maintainers.