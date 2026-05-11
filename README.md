# Create Your Presentation with Reveal.js and markdown

In this project, you will create a presentation using [Reveal.js](https://revealjs.com/) and markdown. 

The goal is to experience a simplified version of a real developer workflow:

1. Fork a project
2. Edit files
3. Preview changes live
4. Save and publish your work

--- 

# Tutorial

## Option 0 (Local copy)

### Step 1 — Fork the Repository

Login or create your [GitHub](https://github.com) account.

Click the **Fork** button in the top right corner of this page.

This creates your own copy of the project.

### Step 2 — Open the project in your editor
If you don't have an editor, you can download Cursor, Claude Code or Visual Studio Code. 

Make your connect your Github account to it and link your [SSH key][https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account]. In order to interact with GitHub directly from your editor.

Open the project using your editor.

### Step 3 - Install dependencies

First you need to install Node.js (which contains the package manager [NPM](https://www.npmjs.com/))

#### Windows
1. **Download the installer** from the [official Node.js website](https://nodejs.org/).
2. **Run the installer** (`.msi` or `.exe`).
3. Follow the installation prompts.
4. Open **Command Prompt** or **PowerShell** and verify the installation:
   ```powershell
   node --version
   npm --version
   ```


#### macOS
**Option 1: Using the official installer**
1. **Download the installer** from the [official Node.js website](https://nodejs.org/).
2. **Run the `.pkg` installer**.
3. Follow the installation prompts.
4. Open **Terminal** and verify:
   ```bash
   node --version
   npm --version
   ```

**Option 2: Using Homebrew (recommended if you are feeling a bit technical)**
1. Install Homebrew (if not already installed):
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
2. Install Node.js:
   ```bash
   brew install node
   ```
3. Verify:
   ```bash
   node --version
   npm --version
   ```

#### **Linux (Debian/Ubuntu and derivatives)**
Using your terminal
1. Update your package list:
   ```bash
   sudo apt update
   ```
2. Install Node.js and npm:
   ```bash
   sudo apt install nodejs npm
   ```
3. Verify:
   ```bash
   node --version
   npm --version
   ```

Then install the library reveal-md. 
Type this in your terminal and hit enter.

```
npm install -g reveal-md
```

### Step 3 - Edit the slides

Create the file `slides.md` in your directory and start writing some markdown. 

Here is an example of simple presentation. Basically you just need to use `---` as a delimiter to add a new slide.

```
# My First Presentation
---
## Introduction
- Welcome to my talk!
- I made this using Markdown.
---
## Why Markdown?
- Easy to learn
- Works everywhere
- No fancy software needed
---
## Table example
| Cheese Name      | Region          | Milk Type | Texture         | Best Paired With         |
|------------------|-----------------|-----------|-----------------|--------------------------|
| Brie de Meaux    | Île-de-France   | Cow       | Soft, creamy    | Fresh baguette, fruit    |
| Roquefort        | Midi-Pyrénées   | Sheep     | Blue, crumbly   | Walnuts, sweet wine      |
| Camembert       | Normandy        | Cow       | Soft, runny     | Apples, red wine         |
| Comté            | Franche-Comté   | Cow       | Hard, nutty     | Cured meats, white wine  |
| Chèvre          | Loire Valley    | Goat      | Soft, tangy     | Salad, honey             |
| Reblochon        | Savoie          | Cow       | Semi-soft       | Potatoes, white wine     |
| Munster          | Alsace          | Cow       | Soft, pungent   | Rye bread, beer          |
| Cantal           | Auvergne        | Cow       | Semi-hard       | Bread, red wine          |
---
## Image example
![Docs Hero](/medias/LaSuite_Docs_Hero.png)
```

If you want to learn more about using reveal.js and markdown for presentation you can read this [documentation](https://docs.hedgedoc.org/references/slide-options/) or ask your favourite AI chatbot, reveal.js is  well known.

### Step 4 — Preview Your Slides
In your Terminal type this and hit enter, it will reflect your local changes instantly

```
reveal-md slides.md --watch
```
Click on the link on your terminal to see your slides. It should say 
```
The slides are at http://localhost:1948/slides.md
```

Navigate your slides using
* arrow keys
* space bar
* on-screen arrows

If you hit `esc` you'll see a preview of all your slides.

To kill the reveal-md server on your computer just do `ctrl + c` in the terminal and hit enter.


### Step 5 — Publish your presentation

Push your work to GitHub following the Git and GitHub tutorial from class provided in the syllabus.

--- 

## Option 2 - Using IETF HedgeDoc instance
If what's above felt too complicated, you're one of the first groups presentating, or you just can't manage to install Node.js on your computer. Here is a simpler way to go about it. 

### Step 1 - Create an account on IETF DataTracker

It's simple go here : https://datatracker.ietf.org/accounts/create/

Login with the account you just created.

Your id is your email address.

### Step 2 - Login on notes.ietf.org

Go to this address: https://notes.ietf.org/
Click on sign in and on the orange button that says `Sign in with IETF DataTracker`

### Step 3 - Create a you note and add your presentation content

The nice thing about this approach is you can collaborate in real time.

### Step 4 - View your slides

Click on Slide Mode in the  dropdown menu in the top right corner.
![Slide Mode](/medias/heddoc_slides.png)

A new tab opens and you can see your navigate your slides.