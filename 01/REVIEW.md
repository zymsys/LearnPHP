Chapter 1: Getting Started with PHP
===================================

Review
------

1. What is HTML? What is XHTML? Name two differences between HTML and XHTML.

    HTML is used to specify the contents of a web page, and the meaning or context of the contents.  For example,
    a heading would be wrapped in heading tags (H1, H2, etc) and a paragraph would be wrapped in paragraph (P) tags.

    XHTML is a special type of XML which is used for the same purpose, and which is easier for machines to parse than
    HTML.  It looks a lot like HTML, but can be difficult to get right.

    One of the differences between HTML and XHTML is that the w3c stands behind HTML but has halted work on XHTML
    instead supporting an XML version of HTML 5.  Another difference is that I can remember the doctype for HTML 5
    but I could never remember the doctype for XHTML.

2. What encoding is your text editor or IDE set to use? Does that match the encoding specified in your generated HTML
pages?

    I normally use IntelliJ IDEA for my IDE, and it is configured to use UTF-8.  I prefer to code my HTML from scratch,
    and when I specify the character type I specify UTF-8.

3. What is CSS and what is it used for?

    CSS stands for Cascading Style Sheets and is used to specify the appearance of HTML documents.

4. What file extension should PHP scripts have for your particular server?

    All of the PHP servers I'm using look for a .php extension for PHP files.

5. What is meant by Web root directory? What is the Web root directory for your server?

    The Web root directory is the main folder which contains web contents.  Any documents which need to be accessed
    through a URL need to live under this directory unless special web server configurations are used.  Any PHP script
    which should be loaded by a URL should live here too, although these scripts can include scripts from folders
    outside of the web root.

6. How do you test PHP scripts? What happens when PHP scripts are not run through a URL?

    I test PHP scripts either through PHPUnit or by loading them in a browser and testing manually.  When PHP scripts
    are not run through a URL they don't generally have their contents returned over HTTP.  PHP scripts can be run
    from the command line, or executed through the php executable in a number of ways.  Generally this is for some
    kind of utility function which doesn't result in a web page.  For example a site might run a script every night
    to send out birthday greetings to members by email.

7. Name two ways comments can be added to PHP code. Identify some ways you would use comments.

    Comments are normally added either as blocks which begin /* and end */, or as single lines which start with //.
    I like to use comments to document functions, methods and variables, including PHPDOC style notation to indicate
    the expected data types, and the purpose of functions.  I try to avoid other comments and instead try to write
    straight forward code that is easy to read with long descriptive variable names.