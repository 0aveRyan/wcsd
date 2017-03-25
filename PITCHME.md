## Building Intuitive 
### WordPress Admin Experiences

David Ryan | daveryan.io | Web Developer @ Time Inc.
---
## CREATE EXPERIENCES
## DEFINE INTUITIVE <!-- .element: class="fragment" -->
## LETS BUILD! <!-- .element: class="fragment" -->
---
> “You can design and create, 
and build the most wonderful place in the world… 
But it takes people to make the dream a reality.”

#### - Walt Disney -
---
### Human-Centered Design
#### 1. Inspiration
*Qualitative & quantitative research.*

#### 2. Ideation <!-- .element: class="fragment" -->
*Critical evaluation* <!-- .element: class="fragment" -->

#### 3. Implementation <!-- .element: class="fragment" -->
*Conscious creation* <!-- .element: class="fragment" -->
+++

![Video](https://www.youtube.com/embed/NBu1kkSCHfs)

---
### Incomplete Intuitive Litmus Test
* People-first, woke development.
* Leverage visual toolbox. Assign hiearchy. Tidy. Tuck. <!-- .element: class="fragment" -->
* Flows that scale. <!-- .element: class="fragment" -->
* Parallel constructs & pairing language. <!-- .element: class="fragment" -->
* Respect established norms, design language. <!-- .element: class="fragment" -->
---
### Building. Oh blog yeah.
1. Techniques for success
2. Common trouble areas
3. Case Study: Featured Video / Media
4. Minutia dive
---
### Techniques For Success
Have exceptional / informed reasons for Core deviation. But don't torture Core or your product.

* Test with all plugins/themes on. <!-- .element: class="fragment" -->
* Iterate quickly, fail cheaply. <!-- .element: class="fragment" -->
* Be elastic, build growing room. <!-- .element: class="fragment" -->
* Be mindful of "cognitave enqueues." <!-- .element: class="fragment" -->
---
### Common Trouble Areas
* Confusing / conflicting color schemes.
* Misappropriating Dashicons or rolling custom. <!-- .element: class="fragment" -->
* Wordy interfaces. Thin interfaces. <!-- .element: class="fragment" -->
* Dense / unpruned interfaces. <!-- .element: class="fragment" -->
---
### Case Study: Featured Video / Media
###### FanSided approach
Add metabox mirroring Featured Image in UI and interaction.
![Screenshot of FanSided featured video metaboxes](assets/fsmetaboxes.png) <!-- .element: class="fragment" -->
---
### Case Study: Featured Video / Media
###### FanSided approach
Add metabox mirroring Featured Image in UI and interaction.
![Screenshot of FanSided custom video library in media modal](assets/setfeatvid.png)
---
### Case Study: Featured Video / Media
###### INN approach
Originally removed metabox, placed Set Featured Media next to Add Media. Now metabox.
![Screenshot of Largo metaboxes](assets/largometaboxes.png)  <!-- .element: class="fragment" -->
+++
Open Discussion About Change:
https://github.com/INN/Largo/pull/1285
---
### Case Study: Featured Video / Media
###### INN approach
Originally removed metabox, placed Set Featured Media next to Add Media. Now metabox.
![Screenshot of Largo library](assets/largolib.png)
---
### Resources in wp-admin
* Non-abstracted Components & CSS - Buttons, List Tables, Tabs, Filter Bar, Notifications, Cards, Grids, etc.
* Data APIs - Options, Meta, Transient, Heartbeat, Filesystem, REST, XML-RPC <!-- .element: class="fragment" -->
* "Component APIs" <!-- .element: class="fragment" -->
    * Customizer <!-- .element: class="fragment" -->
    * Dashboard Widgets API <!-- .element: class="fragment" -->
    * Metabox API <!-- .element: class="fragment" -->
    * The WordPress Media Modal (wp.media) / wp.template <!-- .element: class="fragment" -->
---
### Friends to invite to wp-admin party
* Yahoo's Pure CSS is rad. Written to play nice with other frameworks. Mostly plays nice in admin.
* localforage.js is great if you can assure environment. <!-- .element: class="fragment" -->
* jQuery + Underscores is a _dirt-cheap_ way to feel more 'React-y.' Just sayin'. <!-- .element: class="fragment" -->
---
### wp.template + jQuery + your JSON data from somewhere
```
// Markup
<div class="container"></div>
<script id="tmpl-welcome-to-city" type="text/html">
   <div class="welcome">Welcome to {{{ data.city }}}!</div>
</script>

// jQuery
var template = wp.template( 'welcome-to-city' );
var data = yourDataObject; // has key `city` at root
var container = $('.container');

// punch it chewie!
container.html( template( data ) ); 
```
---
# The End.
