# FEDev-practical-sample-stage-3

NOTE: A Captioned video work through of this stage has been published at:
- (coming soon)

This document summarises the steps I took when creating my solution to the sample FEDev Practial 1

The stages of development required are:
```
Stage 1. Basic HTML structure for 2 pages: “index.html” and “characters.html”
   a. No CSS
   b. No links
   c. No images

Stage 2. Add images

Stage 3. Add nav links

Stage 4. Add CSS, to make the pages look like the provided screenshots
   a. Using CSS style rules in 1 or more “.css” files

Stage 5. Refactor the website as a Svelte(kit) project
   a. Demonstrate reusable Svelte components, such as:
       i. Nav bar
       ii. page footer

Stage 6. Add a third “merchandise” page
   a. Add a link to this page in the nav bar
   b. Style this in a similar style to the other 2 pages
   c. Find images from the web for several merchandise items
   d. Add a form at the bottom of this page asking for:
       i. Name / email address / postal address
       ii. (you do NOT have to write code to process this forms submission)

Stage 7. For an ‘A’ grade illustrate some/all of the following:
   a. Replacing standard CSS rules with TailWindCSS
   b. Populating the merchandise page contents by looping through JSON data
   (rather than hard coded page content)
   c. Publish the site as static pages via GitHub Actions
```

Stage 3. Add nav links

To add nav links we need to add `<a>` elements to our pages.

1. We'll add a `<nav>` element, containing 2 links to both pages, just below the `<header>`

1. So we'll add links for the homepage (root of the website) to URL `/`, and to the characters page with URL `/characters.html` as follows

The traditional approach, which we'll use, is to declare the links inside unordered list elements as follows. I put all this inside a `<nav>` element, to allow for simpler targeting of these links in our CSS rules (to follow in next Stage):

   ```html
   <nav>
      <ul>
         <li>
            <a href="/">HOME</a>
         </li>
   
         <li>
            <a href="/characters.html">CHARACTERS</a>
         </li>
      </ul>
   </nav>
   ```

