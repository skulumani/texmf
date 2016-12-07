## Master `texmf` tree

This holds all the packages and files that I commonly use for LaTeX.

The structure is defined as follows:

`~\texmf\bibtex\bib` for bib files
`~\texmf\tex\latex\local\` for style files

* Windows:
    `C:\Users\username\texmf\`
* MacOS:
    `/Users/username/Library/texmf/`
* Unix: 
    `/home/username/texmf`

## `library.bib`

This is my master BibTeX library.
Originally, it was created and managed in [Bibdesk](http://bibdesk.sourceforge.net/) on my Mac.
However, recently I decided to switch to [Jabref](http://www.jabref.org/) to have a cross platform solution.

The important thing to keep in mind is that the library is linked to the actual pdf files. 
These files are stored in Google Drive at `docs/technical_papers/bibdesk_papers`.
This way the entire library is backed up on Google Drive and indexed via Jabref.

### User manual

1. Clone this repo to the appropriate place in your local `texmf` tree
2. Use `drive` or Google to download the `bibdesk_papers` directory, ensure you keep the same structure to make Google happy.
3. Modify the Jabref settings by going to Options > Preferences > External Programs > Main File Directory and set it to the Google drive directory from step 2
    ~~~
        /home/shankar/Drive/docs/technical_papers/bibdesk_papers
    ~~~
4. Now Jabref should be able to open any of the linked files
5. Jabref settings and plugin are located in the [`system_setup`](https://github.com/skulumani/system_setups) repo