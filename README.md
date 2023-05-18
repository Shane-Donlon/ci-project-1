# Wexford Walking Group 
[Deployment Link](https://shane-donlon.github.io/ci-project-1/index.html)


| Table Of Contents |
| --- |
| [Deployment Link](#wexford-walking-group) |
| [Site Preview](#site-preview) |
| [Project Goals](#project-goals) |
| [UX](#ux) |
| [Symantec HTML](#symantec-html) |

## Site Preview
![dark mode preview](documentation/assets/site-preview-dark-mode.jpg)
![light mode preview](documentation/assets/site-preview-light-mode.jpg)

## Project Goals
Wexford Walking Group is a voluntary group of dog owners, who are keen to have other likeminded people join their group. The group meets up regularly for walks, or just to chill out with some coffee and friends, the weekly coffee is always best because there is cake there.

## UX
The website was designed to be intuitive, and easy to navigate, and to be quick to get to the information needed, with a focus on user system preferences, and accessibility. As this site is for a dog walking group, I also wanted to include fun for the users through animations and interest.
The CSS :: selection pseudo element was also styled (for both dark and light modes) as part of this fun and interesting part of the site.
On the Index page, the waggling animation was included to represent that of a dog’s tail.
The  ::after pseudo elements on the navigation links and form buttons were included to add animations to the hover and focus states. 
The focuses were on these as for me, if the user has a system preference, I believe that as developers we should accommodate these as much as possible.
As well as having a high focus on accessibility. As a developer I believe that the internet is for everyone a fundamental belief for me is that if a site is not accessible a step in the development process has been missed, adding accessibility is not an extra step in the process.
Examples of where this can be found:


<ul>
  <li>
    If the user has a preference set for reduced motion, the animations are
    slowed down, and overall animation is reduced. This is to reduce animations
    that can make users nauseous (vestibular dysfunction) to test this in Chrome
  </li>
  <ol>
    <li>Go to Inspect</li>
    <li>Select the 3 dots beside the X for close</li>
    <li>Select “Run command”</li>
    <li>Search for “Reduced”</li>
    <li>Click the “Do not emulate CSS prefers-reduced-motion”</li>
    <li>
      Refresh the Index.html page and the “waggling” animation will not appear.
    </li>
    <li>To undo this open the site in a new tab.</li>
  </ol>

  <li>
    If the users have a preference set for dark mode, this is considered and the
    site will load in dark mode, if not, the site will load in light mode. Some
    styling changes were made for the “waggling” animation to improve contrast
    on dark mode, as well as the header is coloured for dark mode. To test this
    change your browser settings to either dark mode or to light mode
  </li>
<br>
  If you are on dark mode already (black background)
  <ol>
    <li>Go to Inspect</li>
    <li>Select the 3 dots beside the X for close</li>
    <li>Select “Run command”</li>
    <li>Search for "light"</li>
    <li>Click on “Emulate CSS prefers-color-scheme: light”</li>
    <li>The colour scheme should change to a white background</li>
    <li>To undo this open the site in a new tab.</li>
  </ol>
  <br>
  If you are already on light mode (white background)
  <ol>
    <li>Go to Inspect</li>
    <li>Select the 3 dots beside the X for close</li>
    <li>Select “Run command”</li>
    <li>Search for “dark”</li>
    <li>Click on “Emulate CSS prefers-color-scheme: dark”</li>
    <li>The colour scheme should change to a dark background</li>
    <li>To undo this open the site in a new tab.</li>
  </ol>

  <li>
    A “skip to content” link is added to every page, this is hidden from view
    until you tab onto this. This was placed before the branding, and navigation
    bar, as this designed to give those using screen readers an option of not
    having to tab through the navigation bar to reach the main section, if you
    click on this link the page will scroll to the main section. This was not
    styled as this is intended for screen readers only. This was styled the same
    as the navigation links as some users have a tab preference, and styling was
    added for sighted users.
  </li>

  <li>
    Focus states were included as well as hover states, so that any link /
    button animations are also “triggered” by using tab to accommodate tab
    navigation preferences (using tab key on keyboard) and that they can tell
    where on the screen that they currently are. This does not apply to the Font
    Awesome Social Media Icons, but an outline is visible when tab selected.
  </li>

  <li>
    Role = List was also used for those on older browsers and screen readers,
    this is to introduce the user that there is a list of grouped combinations
    of items.
  </li>

  <li>
    ARIA labels were used for the footer links to provide context that the pages
    open in a new tab. I did not use a “opens in same page” label for navigation
    links, as a screen reader will announce when the page has been loaded, and
    this additional context was not needed.
  </li>
</ul>

### Symantec HTML
Symantec HTML was also used on this site to provide additional context for accessibility.
Overall Symantec HTML elements used:

<ul>
  <li>Header</li>
  <li>Nav</li>
  <li>Main</li>
  <li>Section</li>
  <li>Footer</li>
  <li>H1</li>
  <li>H2</li>
  <li>H3</li>
  <li>Unordered List (UL) as the list provided did not require an order.</li>
</ul>


Below you will find a brief explaination for some of my Symantec HTML decisions made
<ol>
  <li>Index Page</li>
  <ul>
    <li>
      The section element was not used on these pages as there is only a main
      “section” on the page and did not want to cause confusion for accessible
      users. All other pages have a
      <section></section>
      element.
    </li>
  </ul>
  <li>Routes page</li>
  <ul>
    <li>
      A strong element was used for the bold text “important that everyone
      follows them” to provide additional context for screen readers, as I
      believe that these rules are important for everyone to follow.
    </li>
  </ul>
  <li>Success page</li>
  <ul><li>The em was used on the success page for a similar reason, I want to set the same emphasis for accessible and sighted users.</li></ul>
</ol>


While the user of multiple H1’s per page is allowed, for accessibility purposes I prefer to err on the side of caution and used 1 H1 per page. 
As well as with my reset.css all User Agent styling was taken away, this was done intentionally as all fonts are the same, and I do not fall into the “it looks like a H1, so I’ll use a H1” mentality. 



