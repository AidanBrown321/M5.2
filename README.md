# web-dev-starter

This is a starter project for web development with no frameworks and minimal
dependencies. It is intended to be a starting point for web development projects
that are written in plain HTML, CSS, and JavaScript.

## Getting Started

To get started, clone this repository and run the following commands:

```bash
npm install
```

This will install the necessary dependencies for the project.

## Development

It is recommended to use the VSCode Live Server extension to run the project
locally. This will allow you to see changes in real-time as you make them. There
is no need to run a build process or refresh the page manually. Additionally,
you do not need to setup a local server to run the project.

## Testing

To run the tests for the project, run the following command:

```bash
npm test
```

## Running The Site

To run the site, you will need to run Live Preview: Start Server. To do this on VS Code, you
can press ctrl + shift + p, then you should see the command listed. Once you click it, you
can see the page either in the IDE or you can show it in the browser.

## Accessibility Lab Answers

Color: The pink is fine for the background color when there is black text but it isn't optimal. It passes
all of the css tests but a lighter color would be even easier to read. The dark green does not pass most of the
contrast tests so it will need to be changed out for white or a lighter color. The light blue color on the comments is
fine and contrasts well with the black text.

Semantic HTML: When you try to navigate it using a keyboard, there are no header tags or paragraph elements implemented, so it is hard to tell
where you are on the site if you were using a screen reader. Also, not all of buttons are accessible like the show comments button that it is at the bottom. I replaced the div class="nav" with an actual nav elements and added paragraph tags throughout the article.

Images: I added alt text to all of the images.

Audio Player: I added a transcript that users can access if they are hearing impaired and be able to read it. I also added a download option for
those that may have older browsers that don't support the audio.

The Forms: I added a label that is set to display: none in the css to the top search form. I also added labels to both the name and comment
inputs for the comments section at the bottom.

Show/Hide Comment Control: I made the button an actual button so it can be focused with the tab key and activated with return.

The Table: I added scope to the data cells and also added a caption so a user could determine what information was in the table
before reading it.

Other considerations: I changed the headers in the table to be th elements instead of td since they were headers instead of data points.
For my second consideration, I changed the row headers for bear types which are wild and urban to have a black border to the right of them
so that it is clear what they are. I also made the trancript only show when you click the button so that it isn't always there if someone isn't
hearing impaired.
