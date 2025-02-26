MathCask
========

MathCask is a quick starter kit for hosting your mathematical notes
and snippets as self-rendering, distributable HTML documents.  It
supports Markdown and MathJax-flavored LaTeX, making it easy to write
and distribute mathematical content.

You can use MathCask in multiple ways, depending on your technical
background.  If you're familiar with Git, GitHub, or Codeberg, you can
set up a convenient workflow for yourself where you commit your notes
into a Git repo and make them available online via GitHub pages or
Codeberg pages.  Alternatively, you can also host this kit on your
personal web server or web hosting space.

If you're not familiar with these tools, don't worry.  The first few
sections below provide a gentle guide to help you get started.


Contents
--------

* [Set Up MathCask Using GitHub Pages](#set-up-mathcask-using-github-pages)
  * [Fork MathCask](#fork-mathcask)
  * [Add Snippets](#add-snippets)
* [Set Up MathCask Using Codeberg Pages](#set-up-mathcask-using-codeberg-pages)
  * [Fork MathCask](#fork-mathcask)
  * [Add Snippets](#add-snippets)
* [Host On Your Own Web Server](#host-on-your-own-web-server)
* [How Does This Work?](#how-does-this-work)
* [Why?](#why)
* [License](#license)


Set Up MathCask Using GitHub Pages
----------------------------------

The subsections below describe how you can fork this project on
GitHub, and then write and maintain mathematical notes with it.
Naturally, this means that you need a GitHub account to perform these
steps.  If you do not want to create an account on GitHub, skip ahead
to the other sections and see if one of them suits your needs better.
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

  6. Visit `https://USERNAME.github.io/mathcask/demo.html`.  Remember
     to replace `USERNAME` in this URL with your actual username.
     Confirm the page loads fine on your web browser and all
     mathematical content is rendered properly.  The output should
     look like this: [demo.html][demo-gh]

  6. You are now setup to use MathCask.

[demo-gh]: https://susam.github.io/mathcask/demo.html


### Add Snippets

The following steps offer beginner-friendly instructions for creating
a new page to host your mathematics notes or snippets written in
Markdown and LaTeX.  If you're an experienced Git user, you may prefer
using the Git CLI tool to create and publish your pages instead of
following these steps.  However, if you're new to Git, you might the
instructions below helpful.

  1. Go to your fork of MathCask, which is likely at
     `https://github.com/USERNAME/mathcask`.

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
     `https://USERNAME.github.io/mathcask/foo.html` and confirm the
     rendered page loads on your web browser.  The output should look
     like this: [example.html][example-gh].

[example-gh]: https://susam.github.io/mathcask/example.html


Set Up MathCask Using Codeberg Pages
------------------------------------

Codeberg.org is a project repository hosting platform provided by
Codeberg e.V., a non-profit organisation.  Codeberg also offers a
service called Codeberg Pages that may be used to make your
mathematical notes available as web pages.  The subsections below
describe how you can fork this project on Codeberg, and then write and
maintain mathematical notes with it.

In this section the word `USERNAME` is used as a placeholder for your
GitHub username.  Wherever you see this word, you must replace it with
your actual username.


### Fork MathCask

The following steps describe how you can fork this project on GitHub,
and then write and maintain mathematical notes with it:

  1. Fork this project on CodeBerg by going to
     <https://codeberg.org/susam/mathcask> and clicking the **Fork**
     button at the top.

  2. Visit `https://USERNAME.codeberg.page/mathcask/demo.html`.  Remember
     to replace `USERNAME` in this URL with your actual username.
     Confirm the page loads fine on your web browser and all
     mathematical content is rendered properly.  The output should
     look like this: [demo.html][demo-cb]

  6. You are now setup to use MathCask.

[demo-cb]: https://susam.codeberg.page/mathcask/demo.html


### Add Snippets

The following steps offer beginner-friendly instructions for creating
a new page to host your mathematics notes or snippets written in
Markdown and LaTeX.  If you're an experienced Git user, you may prefer
using the Git CLI tool to create and publish your pages instead of
following these steps.  However, if you're new to Git, you might the
instructions below helpful.

  1. Go to your fork of MathCask, which is likely at
     `https://codeberg.org/USERNAME/mathcask`.

  2. Click on **Add file** and then click **New file**.

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

  5. Click **Commit changes**.

  6. Wait for a few minutes for GitHub to publish your new HTML page.
     Assuming you had named it `foo.html`, now visit
     `https://USERNAME.codeberg.page/mathcask/foo.html` and confirm the
     rendered page loads on your web browser.  The output should look
     like this: [example.html][example-cb].

[example-cb]: https://susam.codeberg.page/mathcask/example.html


Host On Your Own Web Server
---------------------------

You can also host self-rendering Markdown + LaTeX pages on your own
web server.  In fact, you do not even need this project to do so.  All
you need to do is add HTML files that contain a simple boilerplate
header to load [TeXMe][] followed by Markdown + LaTeX content.  Here
is an example such HTML:

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

The first line of this file loads TeXMe.  The TeXMe parser parses the
remainder of the file and renders the Markdown and MathJax-flavoured
LaTeX in it.  To learn more about TeXMe, see
[github.com/susam/texme][TeXMe].

[TeXMe]: https://github.com/susam/texme#texme


How Does This Work?
-------------------

If you have looked at the HTML examples from earlier sections, you may
have noticed that they all begin with this line:

```html
<!DOCTYPE html><script src="https://cdn.jsdelivr.net/npm/texme@1.2.2"></script><textarea>
```

This line loads [TeXMe][], a lightweight tool that enables seamless
rendering of both Markdown and MathJax-flavored LaTeX within the same
HTML file.  TeXMe processes the remainder of the HTML file and invokes
a Markdown parser and a LaTeX renderer separately, ensuring that each
parser only interprets the content meant for it.  This prevents
conflicts and produces clean, high-quality output.

One of the important features of TeXMe is its conformance to the
GitHub Flavoured Markdown (GFM) specification.  Since GFM is an
extension of the CommonMark specification, TeXMe also conforms to the
CommonMark specification as a bonus.  To achieve this, TeXMe invokes a
very high quality Markdown parser called Marked that is known to parse
and render GFM text very accurately.  To render MathJax-flavoured
LaTeX, TeXMe invokes MathJax of course, ensuring accurate mathematical
typesetting.  To read more about TeXMe, visit
[github.com/susam/texme][TeXMe].


Why?
----

This quick starter kit was created as a substitute for MathB.in, a
mathematics pastebin that operated from March 2012 to March 2025.
After 13 years of service, MathB.in was shut down.  See the post
[MathB.in Is Shutting Down][shutdown] for more details on why it was
shut down.

MathB.in offered a very convenient way to quickly write down a short
mathematical snippet or post using Markdown and LaTeX and then
generate a distributable link for it with the click of a button.  This
service was powered by MathB, a free and open source software available
at [github.com/susam/mathb][mathb].

Users appreciated MathB.in for its ease of use and robust support for
GitHub Flavoured Markdown (GFM), and MathJax-powered LaTeX.  Since GFM
is a strict superset of CommonMark, the parsing and rendering of user
posts conformed to the CommonMark specification as well.

With the discontinuation of MathB.in, an alternative was needed.
While this kit is nowhere near as quick and convenient as MathB.in, it
does offer a reasonably easy way to set up your own little web space
for sharing your mathematical snippets and notes.  As mentioned in the
previous section, this kit guides you through creating HTML pages for
your snippets and notes that are automatically rendered using the
[TeXMe][texme] parser, the same parser used by MathB.in.  This ensures
that the parsing accuracy, rendering quality, and Markdown
compatibility remain just as reliable.

[shutdown]: https://susam.net/mathbin-is-shutting-down.html
[mathb]: https://github.com/susam/mathb


License
-------

This quick starter kit is available under the terms of the MIT License.


<!--

Publish Checklist
-----------------

git remote add cb https://codeberg.org/susam/mathcask.git
git push cb main:pages

-->
