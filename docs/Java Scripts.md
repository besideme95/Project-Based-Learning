# Java Scripts

## JAVASCRIPTS30

### 1. Javascripts Drum Kit

To quickly generate a basic HTML structure, you can type ! and then press Tab. This will create the following template:
```Javascripts 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>JS Drum Kit</title>
  <link rel="stylesheet" href="style.css">
  <link rel="icon" href="https://fav.farm/✅" />
</head>
<body>

<body>
<html>
```

**Basic HTML Structure for JS Drum Kit**

The following table outlines the basic components of an HTML document, specifically tailored for your JS Drum Kit project.

| **Element**                   | **Code**                                                | **Description**                                                                                                                                          |
|-------------------------------|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Document Type Declaration** | `<!DOCTYPE html>`                                      | This declaration defines the document type and version of HTML being used. It helps the browser to render the page correctly.                          |
| **HTML Tag**                  | `<html lang="en">`                                     | This tag is the root element of the HTML document. The `lang` attribute specifies the language of the document (in this case, English).                |
| **Head Section**              | `<head>`                                               | The `<head>` section contains meta-information about the HTML document, such as its character encoding and linked resources.                           |
| **Character Set**             | `<meta charset="UTF-8">`                               | This meta tag specifies the character encoding for the document, allowing the browser to render text correctly.                                        |
| **Title**                     | `<title>JS Drum Kit</title>`                           | The content inside the `<title>` tag sets the title of the webpage, which appears in the browser tab. You can change the name here to reflect your project's title. |
| **Link to Stylesheet**        | `<link rel="stylesheet" href="style.css">`            | This line links to an external CSS file for styling the HTML document.<br>**`rel`**: Stands for relationship, indicating the relationship between the current document and the linked resource.<br>**`href`**: Stands for Hypertext Reference, providing the URL of the linked resource (in this case, `style.css`). |
| **Link to Favicon**           | `<link rel="icon" href="https://fav.farm/✅" />`      | This tag links to a favicon (a small icon displayed in the browser tab). Ensure that the URL points to a valid icon image.                             |
| **Body Section**              | `<body>`                                               | The `<body>` section contains the content of the webpage that will be displayed to users. You will add your JavaScript and HTML elements for the drum kit within this section. |


This HTML snippet creates a simple drum kit interface where each drum sound is linked to a specific keyboard key. Each `<div class="key">` contains a data-key attribute that matches a sound to its key code. Inside each key div, a `<kbd>` shows the keyboard key, and a `<span class="sound">` labels the sound.

The `<audio>` elements connect to sound files (like clap.wav and hihat.wav), allowing users to play sounds by pressing the corresponding keys on their keyboard. This setup lets users create music interactively by tapping their keyboard.


```HTML
<div class="keys">
<div data-key="65" class="key">
    <kbd>A</kbd>
    <span class="sound">clap</span>
</div>
<div data-key="83" class="key">
    <kbd>S</kbd>
    <span class="sound">hihat</span>
</div>
<div data-key="68" class="key">
    <kbd>D</kbd>
    <span class="sound">kick</span>
</div>
<div data-key="70" class="key">
    <kbd>F</kbd>
    <span class="sound">openhat</span>
</div>
<div data-key="71" class="key">
    <kbd>G</kbd>
    <span class="sound">boom</span>
</div>
<div data-key="72" class="key">
    <kbd>H</kbd>
    <span class="sound">ride</span>
</div>
<div data-key="74" class="key">
    <kbd>J</kbd>
    <span class="sound">snare</span>
</div>
<div data-key="75" class="key">
    <kbd>K</kbd>
    <span class="sound">tom</span>
</div>
<div data-key="76" class="key">
    <kbd>L</kbd>
    <span class="sound">tink</span>
</div>
</div>

<audio data-key="65" src="sounds/clap.wav"></audio>
<audio data-key="83" src="sounds/hihat.wav"></audio>
<audio data-key="68" src="sounds/kick.wav"></audio>
<audio data-key="70" src="sounds/openhat.wav"></audio>
<audio data-key="71" src="sounds/boom.wav"></audio>
<audio data-key="72" src="sounds/ride.wav"></audio>
<audio data-key="74" src="sounds/snare.wav"></audio>
<audio data-key="75" src="sounds/tom.wav"></audio>
<audio data-key="76" src="sounds/tink.wav"></audio>
```

| **Element/Attribute** | **Code**                    | **Description**                                                                                                                                         |
|-----------------------|-----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Div Element**       | `<div>`                     | The `<div>` tag is a block-level container used to group content. It can be styled with CSS and manipulated with JavaScript.                           |
| **Class Attribute**   | `class="keys"`              | The `class` attribute is used to assign a class name to an element, allowing it to be styled or selected by CSS or JavaScript.                          |
| **Data Key Attribute**| `data-key="65"`            | The `data-*` attribute is used to store custom data directly on an HTML element. The `data-key` attribute here associates a specific keyboard key with the sound it triggers. |
| **Kbd Element**       | `<kbd>A</kbd>`             | The `<kbd>` tag represents user input (usually keyboard input) in a document. It's used to display the key that should be pressed (in this case, the letter 'A'). |
| **Span Element**      | `<span class="sound">clap</span>` | The `<span>` tag is an inline container for text or other elements. It can be styled with CSS. Here, it displays the name of the sound associated with the key. |
| **Audio Element**     | `<audio data-key="65" src="sounds/clap.wav"></audio>` | The `<audio>` tag is used to embed sound content in a web page. The `src` attribute specifies the URL of the audio file to play, while `data-key` helps link the audio to the corresponding key. |
| **Src Attribute**     | `src="sounds/clap.wav"`    | The `src` attribute in the `<audio>` tag indicates the path to the audio file that will be played when the associated key is pressed.                       |


