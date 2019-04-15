# Responsive Images

Designed to use a grunt file and image magic to make three sets of responsive images.
Any image files that are not to be resized should be put in the images_src/fixed directory
All other image files will be put in images_src

Update npm and node
Run npm install to update any dependecies.

New images will be found in the images directory

HTML for images:

<figure>
 <picture>
    <source media="(min-width: 650px)" srcset="images/austin-medium.jpg">
    <source media="(min-width: 465px)" srcset="images/austin-small.jpg">
    <img src="images/austin-large.jpg" alt="Floss and Brach" style="width:auto;">
 </picture>
 <figcaption>
 </figcaption>
</figure>

CSS:

figure {
  margin: .25em;
  padding: 0;
  float: left;
  text-align: center;
  position: relative;
}

figure img {
  display: block;
  max-width:100%;
  margin: auto;
  height: auto;
}

figcaption {
  position: absolute;
  left:0;
  bottom:0;
  width: 100%;
  text-align: center;
  color: #C3C3E5;
}



