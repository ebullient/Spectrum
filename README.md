# Welcome to Spectrum Obsidian Theme 👋
![Last Commit](https://img.shields.io/github/last-commit/braweria/Spectrum?style=for-the-badge)  

![Version](https://img.shields.io/badge/version-0.16.6-blue?style=for-the-badge)
[![Documentation](https://img.shields.io/badge/documentation-yes-brightgreen?style=for-the-badge)](https://github.com/Braweria/Spectrum#readme)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green?style=for-the-badge)](https://github.com/Braweria/Spectrum/graphs/commit-activity)
[![License: MIT](https://img.shields.io/github/license/Braweria/Spectrum?style=for-the-badge)](https://github.com/Braweria/Spectrum/blob/master/LICENSE)
[![Twitter: braweria](https://img.shields.io/twitter/follow/braweria.svg?style=social)](https://twitter.com/braweria)

> Spectrum is a dark and light theme for Obsidian.md, a note taking app. Spectrum is meant to be easy on the eyes and boost productivity, but also to not bore your mind by using colours here and there.

- 🏠 [My Homepage](https://braweria.de)

- ✨ [Forum Thread with Changelogs](https://forum.obsidian.md/t/12688)

## Content

- [Contributing](#-Contributing)
  - [Get Started](#Get-Started)
  - [How to compile](#How-to-compile)
- [Author](#Author)
- [Show your support](#Show-your-support)
- [License](#-License)
- [Features of this Theme](#Features-of-this-Theme)
  - [Font](#Font)
  - [Kanban](#Kanban)
  - [Floating Images](#Floating-Images)
  - [Eisenhower Matrix](#Eisenhower-Matrix)
  - [Mermaid Overflow](#Mermaid-Overflow)
- [Places where Spectrum was mentioned](#Places-where-Spectrum-was-mentioned)

## 🤝 Contributing

Contributions, issues and feature requests are welcome!

Feel free to check [issues page](https://github.com/Braweria/Spectrum/issues). You can also take a look at the [forum thread](https://forum.obsidian.md/t/12688).

### Get started 

```sh
git clone https://github.com/Braweria/Spectrum.git
cd Spectrum
npm install
```

### How to compile

```sh
npm run scss
```

## Author

👩‍💻 **Wiktoria Mielcarek**

* Website: https://braweria.de/
* Twitter: [@braweria](https://twitter.com/braweria)
* Github: [@Braweria](https://github.com/Braweria)
* LinkedIn: [Wiktoria Mielcarek](https://linkedin.com/in/wiktoria-mielcarek)


## Show your support

Give a ⭐️ when you like this theme!


## 📝 License

Copyright © 2021 [Wiktoria Mielcarek](https://github.com/Braweria).

This project is [MIT](https://github.com/Braweria/Spectrum/blob/master/LICENSE) licensed.

## Features of this Theme

Some features for this theme are not self-explanatory. Seeing a different colour for the heading is one thing, but what about the hidden features you wouldn't know unless someone told you about it? That's what this section is for.

### Font

This Theme is build with the [JetBrains Mono](https://www.jetbrains.com/lp/mono/) font in mind. I recommend installing it. If you do not want to install the font, the next best monospace font will be used.


### Kanban

With this theme you can create your very own wannabe kanban board! To create one, all you have to do is to set the `cssclass` to `kanban` inside your YAML frontmatter.

```yaml
___
cssclass: [kanban]
---
```

Then you can start creating an unordered list, which will represent your kanban board. The vers first level of list items, are the boards. Every item a level deeper, represent the task or the subtask.

```md
- Ideas
  - checklists
  - external links
- To-Do
  - git push
  - preview image for spectrum
- Doing
  - write the README
- Done
  - features of spectrum
    - Kanban
    - Floating Images
```

![Kanban](./images/kanban.jpg)

### Floating Images

When writing a lot of text, some images have to be inserted to break up the paragraphs. Sometimes those images should be on the left or right of the text, with the text wrapping around it. Now it is possible! All you have to do is to give it the alternative text.

```md
![float-right](./images/kanban.jpg)
```
```md
![float-left](./images/kanban.jpg)
```

This is also possible with wikilinks of images that are already inside your vault!

```md
![[kanban.jpg|float-right]]
![[kanban.jpg|float-left]]
```

*Note: If your image is wider than the note itself, you will have to give it a smaller width for the floating to work. You might also have to either refresh Obsidian or just switch notes real quick, to see the changes. Sometimes Obsidian doesn't live-reload the alternative text.*

### Eisenhower Matrix

You can create your very own Eisenhower Matrix, all you have to do is have either notes or headings within the same note of your four sections. That is important, because you're going to embed them into a table!

First you have to include the new CSS Class `matrix` into your frontmatter.

```yaml
---
cssclass: [matrix]
---
```

Then you'll create a table with two rows and two columns, excluding the table heading. Inside each of the cells you can now embed your sections.

```md
|                   |             |
| ----------------- | ----------- |
| ![[#To-Do]]       | ![[#Doing]] |
| ![[#Considering]] | ![[#Maybe]] |
```

![Eisenhower Matrix](./images/eisenhower.png)

### Mermaid Overflow

You work on two notes and have a mermaid graph open? It has a ton of information, but too small to read? Now with this class you will no longer have this problem! The fixed min-width of a mermaid graph is 750px, which is the width of a note. So now you can scroll left and right to view your graph.

```yaml
___
cssclass: [mermaid-scroll]
---
```

If you want to have the min-width be bigger, you can use this snippet:

```css
.mermaid-scroll .mermaid {
  min-width: 750px; /* Your custom size */ 
}
```

## Places where Spectrum was mentioned

Spectrum is slowly starting to become a theme liked by many users of Obsidian. Here are some online places, where Spectrum was being mentioned:

- [Top 8 Beautiful Obsidian Themes](https://www.youtube.com/watch?v=JgtyQeWkXxE) by Filipe Donadio