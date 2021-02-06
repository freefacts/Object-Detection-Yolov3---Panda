# Object-Detection-Yolov3---Panda
<!-- wp:heading {"textAlign":"center"} -->
<h2 class="has-text-align-center">LabelImg</h2>
<!-- /wp:heading -->

<!-- wp:heading -->
<h2>1. Prepare the Image dataset</h2>
<!-- /wp:heading -->

<!-- wp:paragraph {"align":"justify"} -->
<p class="has-text-align-justify">An image dataset is a folder containing a lot of images (I suggest to get at least 100 of them) where there is the custom object you want to detect. For example I’m training YOLO to recognize a <strong>Panda</strong>, so I have downloaded around 150 images containing Panda images.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":142,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://freefactsin.files.wordpress.com/2021/02/image-5.png?w=1024" alt="" class="wp-image-142"/><figcaption>I have collected Male images and save in a directory named <strong><em>images</em></strong></figcaption></figure>
<!-- /wp:image -->

<!-- wp:columns {"backgroundColor":"foreground"} -->
<div class="wp-block-columns has-foreground-background-color has-background"><!-- wp:column {"width":"100%"} -->
<div class="wp-block-column" style="flex-basis:100%"><!-- wp:paragraph {"align":"justify","textColor":"background"} -->
<p class="has-text-align-justify has-background-color has-text-color"><strong><a rel="noreferrer noopener" href="https://github.com/tzutalin/labelImg" target="_blank">https://github.com/tzutalin/labelImg</a> -&gt; Link to download and clone the labelImg repository, make sure that you follow the instructions to setup and install labelImg with necessary dependencies</strong></p>
<!-- /wp:paragraph --></div>
<!-- /wp:column --></div>
<!-- /wp:columns -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p>Open labelImg, load the directory</p></blockquote>
<!-- /wp:quote -->

<!-- wp:paragraph {"align":"center"} -->
<p class="has-text-align-center"><strong>Annotate the images for what object you are going to detect</strong></p>
<!-- /wp:paragraph -->

<!-- wp:list {"ordered":true} -->
<ol><li>Once we run LabelImg let’s click on “Open Dir”.</li><li>We choose the folder where the images are located</li><li>Then we click on “Select folder”</li><li>We then click on “Change save dir”.</li><li>We select the folder where the images are located (same folder we selected on step 2).</li><li>Then we click on “Select folder”.</li><li>Finally make sure that we’re using the settings for YOLO.<br>If pascalVOC is written, then let’s click and we will see YOLO.</li></ol>
<!-- /wp:list -->

<!-- wp:image -->
<figure class="wp-block-image"><img src="https://pysource.com/wp-content/uploads/2020/04/labelimg_config3.jpg" alt=""/><figcaption>Click pascalVOC, it'll change to Yolo</figcaption></figure>
<!-- /wp:image -->

<!-- wp:heading -->
<h2>&nbsp;2. <strong>Now we’re ready to label the images.</strong></h2>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li>Let’s click on “Create RectBox”</li><li>Let’s select the area where our object is located (in my case I’m going to select the Koala)</li><li>We add the label with the name of our object. In my case typed <strong>Panda </strong>and press Ok.</li><li>We click on “Save”</li></ol>
<!-- /wp:list -->

<!-- wp:image {"id":144,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://freefactsin.files.wordpress.com/2021/02/image-6.png?w=1024" alt="" class="wp-image-144"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph {"align":"center"} -->
<p class="has-text-align-center"><strong>We’re going to do this operation for all the images we have on the dataset.</strong></p>
<!-- /wp:paragraph -->
