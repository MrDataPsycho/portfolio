### Instruction

instruction on how to add blog post: in the folder click on content and then on blog,create a new markdown file under the blog folder and the name should match the blog title .
follow this template to add content,

```
---
title: "Pt Chooses Classic Blue for Its Colour of the Year 2020"
date: 2019-12-24T13:32:54+06:00
image:  images/blog/blog-cover.jpg      
feature_image: images/blog/blog-details-image.jpg
author: Alexender Schoitiz
project_images: ["images/blog/project-details-image-one.jpg", "images/blog/project-details-image-two.jpg"]
---
```

### Black Lines brand identity, by & Smith

Black Lines wants it to be as easy to serve a Negroni as it is a pint of lager. The drinks company is seeking to revolutionise the bar experience by serving cocktails by draught with a changing menu of drinks (as well as same favourite stand-bys). A pink grapefruit spritz was served through the summer while a new pear and white tea fizz joins the line-up for winter.


explnation :
the title is the name of your blog post
date can be left empy ,it should be auto populted when it is published
image will be the thumbnail
feature image :image that appear immediately before your post
author :the author of the post
project_images : an array of images that will be displayed under the content of the posts
you can equally add images within your mark down with this ![My Blog](/images/blog/blog-cover.jpg)


to add images ,go to the root of the folder and click on static and them images and then blog,you can paste your images inside the blog folder .
at all point ,to link your images to your post ,it should follow this path images/blog/nameofyourimage.jpg





to add new products ,follow this instructions 
use this templates :

```
---
title: "KIO TAPE"
date: 2019-12-23T15:44:46+06:00
type: products
sample_url: "https://www.google.com/"
download_url: "https://www.google.com/"
image: "images/projects/project-thumb-four.jpg"
category: ["PRODUCT LABEL"]
project_images: ["images/products/project-details-image-one.jpg", "images/products/project-details-image-two.jpg"]
---
```

The “Seamless Watch” watch has all the features that users expect in a digital watch, and some unusual features





title = title of your products
type = type of your product
sample url :the sample url of your product (to add pdf of your sample url ,go tot he root of the folder andthen click on static ,then pdfdownloads ,here you can paste yout pdf
downlaod files ) the url should follow this pattern "/pdfdownloads/nameofyourfile.pdf"
download url: external linkn to the sale of your product
images :should be stores at static/images/products    , and to link it ,should follow this pattern images/projects/yourimagename.jpg"
the same for project_images...

you can link images with the markdown file like this: ![My Blog](/images/products/pyspark.png)




to add event :
folow this templates:
---
venue: "California"
date: 2019-12-23T20:56:42+06:00
type: events
image: "images/events/event1.jpg"
time: "10 o'clock"

---

The “Seamless Watch” watch has all the features that users expect in a digital watch, and some unusual features.this is a description for event 1


go to content/events and create a newmardown file to add new event .
venue is the location of the evenet
images for event are stored under static/images/events




  
to change the book product at the home to a new product :

go tot he root of the folder and click on config.toml

edit the params.homePoduct parameters to change the product on homepage
  
  you can add new homepage product by adding this under the param s.homeProduct :
    [[params.homeProduct.product]]
        intro  =  "This is a unique way to learn PySpark if you already  know Pandas"
        bookdetail    = "This book covers fundamental of PySpark and good coding practices when writting PySpark code. It has many hands on coding recipes and coding challenges to quickly get you up an running with PySpark."
        imgurl = "images/products/pyspark.png"
        buyurl    = "https://leanpub.com/pandas-to-pyspark"
        sampleurl =  "https://leanpub.com/pandas-to-pyspark"
        enable = true

to disable a homepage product edit enable to false 



paste this in the front matter of any post you wish to hide : draft: true

to hide a product ,event :you can also det draft : true 


