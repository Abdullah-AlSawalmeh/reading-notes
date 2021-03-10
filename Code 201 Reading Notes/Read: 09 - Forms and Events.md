# Forms
Traditionally, the term ‘form’ has referred to a printed document that contains spaces for you to fill in the information. HTML borrows the concept of a form to refer to different elements that allow you to collect information from visitors to your site.

In addition to enabling users to search, forms also allow users to perform other functions online. You will see forms when registering as a member of a website, when shopping online, and when signing up for newsletters or mailing lists.

## Form Controls
There are several types of form controls that you can use to collect information from visitors to your site:

1. ADDING TEXT:

Text input (single-line) Used for a single line of text such as email addresses and names.

Password input Like a single line text box but it masks the characters entered.

Text area (multi-line) For longer areas of text, such as messages and comments.

2. Making Choices:

Radio buttons For use when a user must select one of a number of options.

Checkboxes When a user can select and unselect one or more options.

Drop-down boxes When a user must pick one of a number of options from a list.

3. Submitting Forms:

Submit buttons To submit data from your form to another web page.

Image buttons Similar to submit buttons but they allow you to use an image.

4. Uploadi ng Files:

File upload Allows users to upload files (e.g. images) to a website.

Form Structure

The HTML < form > element is used to create an HTML form for user input:

```
<form action="http://www.example.com/subscribe.php"
method="get">
<p>This is where the form controls will appear.
 </p>
</form>
```

