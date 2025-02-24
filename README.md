MathCask
========

MathCask is a quick starter starter kit for hosting your mathematics
notes as shareable HTML pages.  It supports Markdown and
MathJax-flavored LaTeX, making it easy to write, format, and
distribute mathematical content.

You can use MathCask in multiple ways, depending on your technical
background.  If you're familiar with Git, GitHub, or Codeberg, you can
set up a convenient workflow for yourself where you commit your notes
into a Git repo and make them available online via GitHub pages or
Codeberg pages.  Alternatively, you can also host this kit on your
personal web server or web hosting space.  If you aren't very familiar
with any of these, the sections below intend to serve as a gentle
guide to ge started.

The following sections outline the easiest ways to get started.
MathCask is a quick starter kit that lets you host your mathematics
notes as distributable HTML pages written using Markdown and LaTeX
(the MathJax flavour of LaTeX).

If you're not familiar with these tools, don't worry.  The first few
sections below provide a gentle guide to help you get started.


Set Up MathCask Using GitHub Pages
----------------------------------

In this section the word `USERNAME` is used as a placeholder for your
GitHub username.  Wherever you see this word, you must replace it with
your actual username.


### Fork MathCask

The following steps describe how you can fork this project on GitHub,
and then write and maintain mathematical notes with it:

  1. Fork this project on GitHub by going to
     <https://github.com/susam/mathcask> and clicking the **Fork**
     button at the top.

  2. Go to your forked copy of this project on GitHub and click
     **Settings**.

  3. In the left sidebar click **Pages**.

  4. Under the **Branch** section, click on the dropdown, select
     **main**, and click **Save*.

  5. Wait for a few minutes to allow GitHub to deploy the pages in
     this kit using GitHub Pages.

  6. Visit <https://USERNAME.github.io/mathcask/DEMO.html>.  Remember
     to replace `USERNAME` in this URL with your actual username.
     Confirm the page loads fine on your web browser and all
     mathematical content is rendered properly.

  6. You are now setup to use MathCask.


### Create Snippets

The following steps offer beginner-friendly instructions for creating
a new page to host your mathematics notes or snippets written in
Markdown and LaTeX.  If you're an experienced Git user, you may prefer
using the Git CLI tool to create and publish your pages instead of
following these steps.  However, if you're new to Git, you might the
instructions below helpful.

  1. Go to your fork of MathCask, possibly at,
     <https://github.com/USERNAME/mathcask>.

  2. Click on **Add file** and then click **Create new file**.

  3. Name your new file `foo.html`.  In fact, you could choose any
     name you like as long it has the extension `.html`.

  4. Now enter the following file contents:

     ```html
     <!DOCTYPE html><script src="https://cdn.jsdelivr.net/npm/texme@1.2.2"></script><textarea>

     # Euler's Identity

     In mathematics, **Euler's identity** is the equality
     $$ e^{i \pi} + 1 = 0. $$

     ## Explanation

     Euler's identity is a special case of Euler's formula from complex
     analysis, which states that for any real number $ x $,
     $$ e^{ix} = \cos x + i \sin x. $$
     ```

  5. Finally, click **Commit changes**, review/change the commit
     message, and click **Commit changes** again.

  6. Wait for a few minutes for GitHub to publish your new HTML page.
     Assuming you had named it `foo.html`, now visit
     <https://USERNAME.github.io/mathcask/foo.html> and confirm the
     rendered page loads on your web browser.


Set Up MathCask Using Codeberg
------------------------------

Coming soon!


License
-------

This quick starter kit is available under the terms of the MIT License.
