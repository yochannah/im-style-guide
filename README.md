# im-style-guide

This is a short list of resources and to-dos; I hope I'll find time to expand on things later. 

- **InterMine data type colours:** We like to associate certain colours with certain datatypes. See [this less file](https://github.com/intermine/bluegenes/blob/dev/less/datatype-colors.less#L1-L57). 
- Generally default to flattish [material-design](https://material.io/design/)-esque style if in doubt.
    - some specific guidelines: 
        - always give buttons good click affordance. Translated into english: They should look buttony, with a border or different colour to the background, ideally some shadow, and defined `:hover` and `:active` states. We never want the user to mistake a button for the background or page decoration.    
        - call to action buttons should contrast with the rest of the page - e.g. a bright colour on white. 
        - operations that you don't want to call the user's eyes to should be lighter and less obvious - e.g. the cancel, back,  or delete button. I know you're tempted to put the delete button as red or orange for warning, but bright buttons draw the eyes and make us click them unthinkingly - the opposite of what we were trying to achieve. 
- **Avoid icon fonts.** They're easy to use, but we have [no end of problems](https://css-tricks.com/icon-fonts-vs-svg/) with them.  CORS sometimesprevents icons fonts from loading and can make the page unusable, plus they tend to abuse HTML standards and tend to be less accessible to screen readers. Instead, use inline SVG - [icomoon](https://icomoon.io/app/#/select) makes this pretty easy.  
- **colours** Use [500 colours](https://www.materialui.co/colors) forhighlights, lighter colours and greys from the chart for more subtle elements.

===================================================

## To-dos: 

- convert the colours less file so a single external less and/or sass library that can be included (possibly even a module that's on npm or yarn or something?)
- define a common svg icon library?
- auto-generate a page with visuals of the type colours, alongside their codes 
- link to intermine logos. 
