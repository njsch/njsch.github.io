# njsch.github.io
My Github personal user account static Pages site.

## Overview
This site is powered by Jekyll, as are many user and organisation and project sites on github Pages. It contains mostly Markdown sources converted into target HTML but some of the HTML is manually implemented. Any Ruby backend is from Jekyll only, since Github only allows for static content or client-only code from Javascript, but nothing server-side. There is one LaTeX source for some target HTML.

to set up this site:
1. Fork the repo.
2. Clone your fork.
3. Go into Settings > Pages on the Github website for the forked repo's settings.
4. Set up the publishing source to come from Github Action via a workflow and ensure it is set to the `github-pages` environment via the `Deploy Jekyll with GitHub Pages dependencies preinstalled` workflow.
5. Not sure if you may have to remove the CNAME file for my custom domain name or remove the url from the `_config` YAML file.
6. Make, commit and push your changes.
