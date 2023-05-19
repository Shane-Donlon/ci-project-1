# Wexford Walking Group 
[Deployment Link](https://shane-donlon.github.io/ci-project-1/index.html)


| Table Of Contents |
| --- |
| [Deployment Link](#wexford-walking-group) |
| [Site Preview](#site-preview) |
| [Project Goals](#project-goals) |
| [UX](#ux) |
| [Symantec HTML](#symantec-html) |
| [Color Scheme](#color-scheme) |
| [Fonts Used](#fonts) |
| [Technology Used](#technology-used) |




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
    change your browser settings to either dark mode or to light mode. 
    The meta tag for color scheme was used so that even if the css style sheet does not load, the background 
    will be that of the theme picked, and will not "jump" from light to dark as the css files load.
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
  <ul><li>The em element was used on the success page for a similar reason, I want to set the same emphasis for accessible and sighted users.</li></ul>
</ol>


While the user of multiple H1’s per page is allowed, for accessibility purposes I prefer to err on the side of caution and used 1 H1 per page. 
As well as with my reset.css all User Agent styling was taken away, this was done intentionally as all fonts are the same, and I do not fall into the “it looks like a H1, so I’ll use a H1” mentality. 


## Color Scheme
![color scheme preview](documentation/assets/color-scheme.jpg)

The site has 3 main colours that are used in a variety of ways brown, black and white.
These colours were used to mimic that of a Bernese Mountain Dog to keep the dog theme throughout this site.

<em> The dark theme background colour is decided by the browser and is not part of the colour palette. </em>


As previously mentioned the selection colours were also changed to black background white text / white background black text, depending on the theme used.
This was to keep in-line with the branding color choices (default is blue selection which is not part of the branding)
To see this simply use your mouse to select text (hold down the click and drag the mouse over the text / ctrl + a)



## Fonts

The primary font of the site is Roboto, this was used as it has a variety of weights and styles available for the site, and it was chosen as it could be dynamic in weights and styles. 

![Font Weight Roboto 400](documentation/assets/font-weight-roboto-400.jpg)
![Font Weight Roboto 500](documentation/assets/font-weight-roboto-500.jpg)
![Font Weight Roboto 500](documentation/assets/font-weight-roboto-700.jpg)

The secondary font of the site is Bebas Neue this was chosen as it is an uppercase font, but also the weight was appealing as a secondary font.
I intentionally kept both fonts a Sans-Serif font as to complement each other.

![Font Weight Bebas Neue 400](documentation/assets/font-weight-bebas-neue-400.jpg)


A paragraph length was also used to ensure that no head turning is required to read long sentences on larger screens. 
Font weights are not heavily prevalent in the site as this is informal, but also as over-relying on weights can reduce their impact.


## Technology Used
### Languages
- [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML): the markup language used to create the website.
- [CSS](https://developer.mozilla.org/en-US/docs/Web/css): the styling language used to style the website.

JavaScript was not used on this site, as it was a HTML and CSS only challenge, if JavaScript was allowed for this I would have used an Event Listener and Arrow Function like below to toggle the active class on the hamburger menu

    hamgurgerMenu = document.querySelector(".hamburger-menu");
    navBar = document.querySelector(".nav");

    hamgurgerMenu.addEventListener("click", () => {
      navBar.classList.toggle("active");
    });

## Testing
As a note before we disucss testing. 

The hamburger menu was created using CSS :has which is curently only supported in Chrome and Safari (technical preview) see [can I use](https://caniuse.com/css-has) 

This was taken into consideration, and I have built the hamburger menu into a Feature Query in CSS, meaning that when Firefox supports :has() it will automatically become a hamburger menu without having to write any new code.

As a fall back for this, browswers that do not support :has() will have the navigation links wrap to the top beside the branding.
See images below. This was all a consious decision as browswer support for :has() is currently at 86.93% (see can I use link above) globally and it is a good time for me, to start to push the bounderies with this psuedo class to get a better understanding of it. Also this is a personal project, so I have no issues with being experimental with newer elements, but still being consious of browswer support. But also it was a good time to practice my feature query skills in css (@supports)

As the nav bar is as designed tests some tests will not apply for Firefox and will be marked as not applicable "N/A"

Firefox Menu Screenshot


![firefox nav bar](documentation/assets/firefox-has-not-supported.jpg)


Chrome Menu Screenshot


![chrome nav bar](documentation/assets/chrome-has-supported.jpg)


<table>
  <th>Testing Number</th>
  <th>Testing Description</th>
  <th>Result Chrome</th>
  <th>Result Chrome Mobile</th>
  <th>Result Firefox</th>
  <th>Result Firefox Mobile</th>
  <th>Result Safari Tablet</th>
  <tr>
    <td>1</td>
    <td>Website Loads</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>2</td>
    <td>Wagggling Animation index page does not laod on mobile</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>3</td>
    <td>Wagggling Animation index page does laod on desktop</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>4</td>
    <td>Index page hero image loads</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>5</td>
    <td>Navigation Links go to correct pages (index page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>6</td>
    <td>Footer links open in new tab (index pages)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>7</td>
    <td>Navigation Links go to correct pages (routes page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>8</td>
    <td>Footer links open in new tab (routes pages)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>9</td>
    <td>Navigation Links go to correct pages (beginners page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>10</td>
    <td>Footer links open in new tab (beginners pages)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>11</td>
    <td>Navigation links open in new tab (success pages)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>12</td>
    <td>Footer links open in new tab (success pages)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>13</td>
    <td>Skip to content appears on tab (index page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>14</td>
    <td>Skip to content appears on tab (routes page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>15</td>
    <td>Skip to content appears on tab (routes page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>16</td>
    <td>Skip to content appears on tab (sucess page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>17</td>
    <td>Skip to content click and enter goes to main (index page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>18</td>
    <td>Skip to content click and enter goes to main (routes page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>19</td>
    <td>Skip to content click and enter goes to main (beginners page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>20</td>
    <td>Skip to content click and enter goes to main (success page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>21</td>
    <td>Hamburger menu appears on mobile devices (index page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>22</td>
    <td>Hamburger menu appears on mobile devices (routes page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>23</td>
    <td>Hamburger menu appears on mobile devices (beginners page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>24</td>
    <td>Hamburger menu appears on mobile devices (success page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>25</td>
    <td>
      Nacigation Links Animate on hover and tab / focus desktop only (index
      page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>26</td>
    <td>
      Nacigation Links Animate on hover and tab / focus desktop only (routes
      page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>27</td>
    <td>
      Nacigation Links Animate on hover and tab / focus desktop only (beginners
      page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>28</td>
    <td>
      Nacigation Links Animate on hover and tab / focus desktop only (success
      page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>29</td>
    <td>
      Join Us Link Animate on hover and tab / focus desktop only (index page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>30</td>
    <td>Footer Links Animate on hover desktop only (index page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>31</td>
    <td>Footer Links Animate on hover desktop only (routes page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>32</td>
    <td>Footer Links Animate on hover desktop only (beginners page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>33</td>
    <td>Footer Links Animate on hover desktop only (sucess page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>34</td>
    <td>Footer Links Animate on active mobile only (index page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>35</td>
    <td>Footer Links Animate on active mobile only (routes page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>36</td>
    <td>Footer Links Animate on active mobile only (beginners page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>37</td>
    <td>Footer Links Animate on active mobile only (sucess page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>38</td>
    <td>Page Responsive for mobile only (index page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>39</td>
    <td>Page Responsive for mobile only (routes page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>40</td>
    <td>Page Responsive for mobile only (beginners page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>41</td>
    <td>Page Responsive for mobile only (sucess page)</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>42</td>
    <td>Dark mode (index page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>43</td>
    <td>Dark mode (routes page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>44</td>
    <td>Dark mode (beginners page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>45</td>
    <td>Dark mode (success page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>46</td>
    <td>Light mode (index page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>47</td>
    <td>Light mode (routes page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>48</td>
    <td>Light mode (beginners page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>49</td>
    <td>Light mode (success page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>50</td>
    <td>Selection colour light mode (all devices) (index page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>51</td>
    <td>Selection colour light mode (all devices) (routes page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>52</td>
    <td>Selection colour light mode (all devices) (beginners page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>53</td>
    <td>Selection colour light mode (all devices) (success page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>54</td>
    <td>
      Walking Group Wexford branding links to index page (all devices) (index
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>55</td>
    <td>
      Walking Group Wexford branding links to index page (all devices) (routes
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>56</td>
    <td>
      Walking Group Wexford branding links to index page (all devices)
      (beginners page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>57</td>
    <td>
      Walking Group Wexford branding links to index page (all devices) (success
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>58</td>
    <td>
      Walking Group Wexford branding links cursor pointer on hover (desktop
      only) (index page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>59</td>
    <td>
      Walking Group Wexford branding links cursor pointer on hover (desktop
      only) (routes page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>60</td>
    <td>
      Walking Group Wexford branding links cursor pointer on hover (desktop
      only) (beginners page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>61</td>
    <td>
      Walking Group Wexford branding links cursor pointer on hover (desktop
      only) (success page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>62</td>
    <td>
      Navigation Links cursor pointer on hover (desktop only) (index page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>63</td>
    <td>
      Navigation Links cursor pointer on hover (desktop only) (routes page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>64</td>
    <td>
      Navigation Links cursor pointer on hover (desktop only) (beginners page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>65</td>
    <td>
      Navigation Links cursor pointer on hover (desktop only) (success page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>66</td>
    <td>Footer Links cursor pointer on hover (desktop only) (index page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>67</td>
    <td>Footer Links cursor pointer on hover (desktop only) (routes page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>68</td>
    <td>
      Footer Links cursor pointer on hover (desktop only) (beginners page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>69</td>
    <td>Footer Links cursor pointer on hover (desktop only) (success page)</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>70</td>
    <td>
      Abbreviation HTML routes page only hover mouse over KM and leave for a few
      seconds (desktop only) (routes page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>71</td>
    <td>Input Form contains red border for required input (beginners page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>72</td>
    <td>Input Form contains green border for valid input (beginners page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>73</td>
    <td>
      Submit button redirects to success page upon valid input fields completed
      correctly (beginners page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>74</td>
    <td>Reset Form button clears all data from form (beginners page)</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>75</td>
    <td>
      Required Field First Name cannot submit if blank or incomplete (error
      appears) (beginners page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>76</td>
    <td>
      Required Field Surname cannot submit if blank or incomplete (error
      appears) (beginners page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>77</td>
    <td>
      Required Field email cannot submit if blank or incomplete (error appears)
      (beginners page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>78</td>
    <td>
      Submit Button cursor pointer on hover (desktop only) (beginners page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>79</td>
    <td>
      Reset Form button cursor pointer on hover (desktop only) (beginners page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>80</td>
    <td>
      Submit Button animates on hover and focus (desktop only) (beginners page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>81</td>
    <td>
      Reset Form Button animates on hover and focus (desktop only) (beginners
      page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>82</td>
    <td>
      Iframes Cursor Pointer on hover (desktop only) (beginners
      page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>


  <tr>
    <td>83</td>
    <td>
      Iframes play on click (beginners
      page)
    </td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Pass</td>
    <td>Not Applicable</td>
    <td>Not Applicable</td>
  </tr>

  <tr>
    <td>84</td>
    <td>
      Contrast Colour Checker Light Mode (index
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>
  
    <tr>
    <td>85</td>
    <td>
      Contrast Colour Checker Light Mode (routes
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

 <tr>
    <td>86</td>
    <td>
      Contrast Colour Checker Light Mode (beginners
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>
  
   <tr>
    <td>87</td>
    <td>
      Contrast Colour Checker Light Mode (success
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>
<tr>
    <td>88</td>
    <td>
      Contrast Colour Checker Dark Mode (Index
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>

  <tr>
    <td>89</td>
    <td>
      Contrast Colour Checker Dark Mode (routes
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>
  
    <tr>
    <td>90</td>
    <td>
      Contrast Colour Checker Dark Mode (beginners
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>
    <tr>
    <td>91</td>
    <td>
      Contrast Colour Checker Dark Mode (success
      page)
    </td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
    <td>Pass</td>
  </tr>
</table>


Notes on the contrast this has also been verified by a person who has partial colour blindness and all words were legible (both light and dark modes)
