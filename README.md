# Fusion CAC Web Product Documentation

This is the Fusion CAC Web Product Documentation site!

## Recommended Workflow for working with this repository

### Install Visual Studio Code with Markdown Plugins

Install Visual Studio Code, and add the following extensions through the extensions tab:

- Hugo Language and Syntax Support
- Markdown All in One
- Markdown PDF
- markdownlint
- Markdown Preview Mermaid Support

### Install Hugo

Download the hugo 134.2 release from this link:

https://github.com/gohugoio/hugo/releases/download/v0.134.2/hugo_extended_0.134.2_windows-amd64.zip

In this zip file, there is a single exe that you need (hugo.exe.)  Copy this to either the root of your drive
or (if you're familiar with the PATH environment variable) somewhere on your PATH.

### Local Development/Preview

Open the folder in Visual Studio Code and work on markdown files in the content subdirectory.  To start a local server,
open the terminal (View -> Terminal) and type:

- `/hugo server` if you installed hugo on the root of your C drive
- `hugo server` if you installed hugo somewhere on your PATH

Once you run this, navigate in your browser to http://localhost:1313/fusion-cac-web-docs to view a live
preview in your browser.  This view will auto-refresh and update as you make changes to files and save them in Visual 
Studio Code.

### Sharing your changes and deploying to the live site

The live site is locaed at: https://dolbeysystems.github.io/fusion-cac-web-docs/  

To deploy your local changes to production, commit and sync (push) your changes using the `Source Control` tab in Visual
Studio Code.

> [!note]
> If you get a warning saying that you need to pull changes before pushing, do as it says and
> pull changes using the `...` menu on the `Source Control` tab and choosing `Pull`.  This will
> integrate changes that you were not up to date with on the server before pushing your changes.
> Once this is completed, you should push/sync again.

### Authoring

Details on how to author content in the content folder can be found at the documentation for the hugo relearn theme 
here:

https://mcshelby.github.io/hugo-theme-relearn/index.html



