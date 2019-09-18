# CodingNomads Platform Updates

## Synchronizing Styling

We want a **unified style** across all courses on the whole site.
It is helpful to **centralize** the design as much as possible and allow
it to **remain adaptable** without having to dig into every course's code separately.

With this in mind I did some research and have a few updates to report:

### Colors

<div style="display: flex; justify-content: space-between;">

<div>
    <p>My aim was to use the colors from our logo:</p>
    <img src="https://pbs.twimg.com/profile_images/960981641689677824/ddu4i3as_400x400.jpg" width="250">
</div>

<div>
Specifically, I would suggest the two outer colors:

<h4>sunset yellow (outermost)</h4>
<div style="display: flex">
    <div style="background-color: #FBB03B; width: 80px; height: 80px; color: white;">#FBB03B</div>
    <div>
        <ul>
            <li>HTML code:  #FBB03B</li>
            <li>RGB code:   R: 251 G: 176 B: 59</li>
            <li>HSV:    36.56° 76.49% 98.43%</li>
        </ul>
    </div>
</div>

<h4>sea blue</h4>
<div style="display: flex">
    <div style="background-color: #0071BD; width: 80px; height: 80px; color: white;">#0071BD</div>
    <div>
        <ul>
            <li>HTML code:  #0071BD</li>
            <li>RGB code:   R: 0 G: 113 B: 189</li>
            <li>HSV:    204.13° 100% 74.12%</li>
        </ul>
    </div>
</div>

</div>

</div>

### General Theme

The general theme settings for the platform now reflect these two colors as **primary** (sea-blue) and **secondary** (sunset-yellow) **Brand colors**.

They can be changed in `Administration / Appearance / Themes / Theme Settings`

### Section Dividers

Secondly, the section dividers can now accept custom CSS classes that also reflect the Brand colors, and most importantly, make them easier to create and maintain.

The HTML code for the section dividers can now be reduced to this:

```html
<h5 class="section-divider">Variables</h5>
```

instead of that:

```html
<p><br></p><h5 style="background-color: #049fcd; color: #ffffff;"><b>&nbsp;<nolink>Variables</nolink></b></h5><p></p>
```

which means getting rid of all the in-line CSS and just **assigning one of two classes** in the usual HTML edit box:

* `section-divider` for the general dividing elements (using CN sea-blue)
* `section-assignment` for the "Assignments" dividing elements (using CN sunset-yellow)

They are appropriately styled with spacing etc. from within our theme's SCSS file.
Design changes for the dividers can now be made centrally in the [**Maker** Theme settings](https://platform.codingnomads.co/learn/admin/settings.php?section=themesettingmaker) in the "Advanced" tab inside the second SCSS box.

Currently:

```css
.section-divider,
.section-assignment {
    color: #fff;
    font-weight: bold;
    margin: 30px 0 5px 0;
    padding: 2px 0 2px 25px;
}
.section-divider {background-color: #0071BD;} // codingnomads seablue
.section-assignment {background-color: #FBB03B;} // codingnomads sunsetyellow
```

With this color/style changes, spacing (padding, margin) etc. can be easily applied site-wide.

**So, if we apply those classes on all dividers once, we can keep playing and improving the style site-wide
without needing to go into every course separately, which makes keeping up-to-date and improving easier.**

This is highly editable, so any color, spacing, ... changes can afterwards be done in one swoop [here](https://platform.codingnomads.co/learn/admin/settings.php?section=themesettingmaker) (Advanced tab / second SCSS box).

### Stop Automatic Linking

Since the `<nolink>` tags are [somewhat messy](https://docs.moodle.org/36/en/Nolink_tags), I decided to [**disable Autolinking**](https://docs.moodle.org/24/en/Autolinking) for the Python Online course.

I think it's more a pain-in-the-ass than helpful.

Autolinking can be **disabled site-wide**, which I would suggest to do, but I kept it for the Python course for now to not mess something up that might be used by someone else already.
