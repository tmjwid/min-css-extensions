# min-extensions
Small, useful extensions to min.css (https://github.com/owenversteeg/min) keeping with the small nature of the framework. To see them in action, [click here]()

## Providing the following additions:

### Screen size constraints (e.g do not show on mobile) for mobile, tablet and desktop

### Navigation
- Light theme navigation menu
- Additonal text line for navigation (e.g tagline)
- Right hand side links in nav
  
### User messages
- Error
- Success
- Info
- Warning

### Standard sizes headings

### Smaller button for btn-sm

### Basic "card" style element

### Responsive images by default (might not be worth it to some people)

### Small fixes including
- divs can now be use in the nav without adding additional hamburger menu icons

# Docs

## Usage

Download minext.css, modify (if need be) and minify. Reference in your html under your min.css reference 

```
<link rel="stylesheet" href="./assets/min.css">
<link rel="stylesheet" href="./assets/minext.css">
```

## Screen size contraints
To not show an element based on the size of device, you can use the following classes to any node.
    
    hidden-d (for desktop)
    hidden-t (for tablet)
    hidden-m (for mobile)

## Navigation
### Light menu
The light menu is very simple to activate, simplely add the class `light` to the nav element like so.

```<nav class="nav light" tabindex="-1" onclick="this.focus()">```

### Twoline
Adding additonal space for a tagline is easy too, just add the class `twoline` to the nav element like so 

```<nav class="nav twoline" tabindex="-1" onclick="this.focus()">```

Then add your additional text in a row (for padding) or just text (without padding), above your links if you are using left hand links 

```
<nav class="nav twoline" tabindex="-1" onclick="this.focus()">
    <div class="container">
        <a class="pagename" href="#">Min Ext</a>
        <div> //add a class row here for padding
            <span>Lorem Ipsum is simply dummy text of the printing and typesetting</span>
        </div>
        <div>
            <a href="#">One</a>
            <a href="#">Two</a>
        </div>
    </div>
</nav>
```
If you are using righthand side links, put the text under the links. 

```
<nav class="nav twoline" tabindex="-1" onclick="this.focus()">
    <div class="container">
        <a class="pagename" href="#">Min Ext</a>
        <div class="links-right">
            <a href="#">One</a>
            <a href="#">Two</a>
        </div>
        <div> //add a class row here for padding
            <span>Lorem Ipsum is simply dummy text of the printing and typesetting</span>
        </div>
    </div>
</nav>
```

### Righthand side links
Simply wrap your links in a div and add the class `links-right`

```
<nav class="nav" tabindex="-1" onclick="this.focus()">
    <div class="container">
        <a class="pagename" href="#">Min Ext</a>
        <div class="links-right">
            <a href="#">One</a>
            <a href="#">Two</a>
        </div>
    </div>
</nav>
```

## Messages
All messages use basic syntax for the message and an overload for the type. Here are each message type. 
```
<div class="col c3 msg error">
    oh no
</div>
<div class="col c3 msg warning">
    be careful
</div>
<div class="col c3 msg success">
    well done!
</div>
<div class="col c3 msg info">
    today is a good day to live!
</div>
```

## Cards

Cards are a way to showcase something important, or for user sections. The following html produces a card. The classes `title` and `date` provide additional styling. 
```
<div class="col c3 card">
    <div class="col c12">
        <img src="https://placeimg.com/480/410/tech/sepia" />
    </div>
    <h2 class="title">TITLE</h2>
    <span class="date">20-02-2019</span>
    <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>                    
</div>
```


I hope you like these additons, please let me know of any issues in the issue tracker and you can contact me [here](mailto:hello@mandark.org). Very welcome to pr's with additional fixes and features! 
