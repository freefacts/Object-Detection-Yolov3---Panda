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
<!-- wp:quote -->
<blockquote class="wp-block-quote"><p>The first step is to upload your <strong>images</strong> in to your Google Drive in the folder <strong><em>yolov3</em></strong>, and then just run the <strong>Colab Notebook</strong> from the repository - <a rel="noreferrer noopener" href="https://github.com/freefacts/Object-Detection-Yolov3---Panda.git" data-type="URL" data-id="https://github.com/freefacts/Object-Detection-Yolov3---Panda.git" target="_blank">https://github.com/freefacts/Object-Detection-Yolov3---Panda.git</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:heading -->
<h2>3. Train the Image dataset online</h2>
<!-- /wp:heading -->

<!-- wp:image {"id":150,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://freefactsin.files.wordpress.com/2021/02/image-7.png?w=1024" alt="" class="wp-image-150"/><figcaption><strong>Train_Yolov3.ipynb is the train file</strong> - Setup like above</figcaption></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Then run the model, you need not to worry about training, each and every instruction to train the model is given in the Colab Notebook</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":152,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://freefactsin.files.wordpress.com/2021/02/image-8.png?w=1024" alt="" class="wp-image-152"/><figcaption><strong>Extracting the images</strong></figcaption></figure>
<!-- /wp:image -->

<!-- wp:image {"id":154,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://freefactsin.files.wordpress.com/2021/02/image-9.png?w=1024" alt="" class="wp-image-154"/><figcaption><strong>If you see an output similar to the one below, then well done, your model is training</strong></figcaption></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Usually it takes a minimum of 3 hours to the entire 12 hours you have the access to the gpu.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>4. Test the model that we created</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Each 100 iterations, our custom object detector is going to be updated and saved on our Google drive, inside the folder “yolov3”.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The <strong>file that we need is “yolov3_training_last.weights”.</strong><br>You might find that other files are also saved on your drive, “yolov3_training__1000.weights”, “yolov3_training_2000.weights” and so on because the darknet makes a backup of the model each 1000 iterations.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2><strong>Test run 1</strong></h2>
<!-- /wp:heading -->

<!-- wp:image {"id":160,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://freefactsin.files.wordpress.com/2021/02/image-12.png?w=1024" alt="" class="wp-image-160"/><figcaption><strong>Yes, I was wondered - there were no inference😔</strong></figcaption></figure>
<!-- /wp:image -->

<!-- wp:heading -->
<h2><strong>Test run 2 -</strong> After leaving the model to train for like 6 hours</h2>
<!-- /wp:heading -->

<!-- wp:image {"id":158,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://freefactsin.files.wordpress.com/2021/02/image-11.png?w=1024" alt="" class="wp-image-158"/></figure>
<!-- /wp:image -->

<!-- wp:heading {"textAlign":"center","backgroundColor":"foreground","textColor":"background-high-contrast"} -->
<h2 class="has-text-align-center has-background-high-contrast-color has-foreground-background-color has-text-color has-background">Voila! - We got the Panda</h2>
<!-- /wp:heading -->

<!-- wp:gallery {"ids":[162,163,164,165,166],"linkTo":"none"} -->
<figure class="wp-block-gallery columns-3 is-cropped"><ul class="blocks-gallery-grid"><li class="blocks-gallery-item"><figure><img src="https://freefactsin.files.wordpress.com/2021/02/capture1.jpg?w=802" alt="" data-id="162" data-full-url="https://freefactsin.files.wordpress.com/2021/02/capture1.jpg" data-link="https://freefactsin.wordpress.com/capture1/" class="wp-image-162"/></figure></li><li class="blocks-gallery-item"><figure><img src="https://freefactsin.files.wordpress.com/2021/02/capture2.jpg?w=751" alt="" data-id="163" data-full-url="https://freefactsin.files.wordpress.com/2021/02/capture2.jpg" data-link="https://freefactsin.wordpress.com/capture2/" class="wp-image-163"/></figure></li><li class="blocks-gallery-item"><figure><img src="https://freefactsin.files.wordpress.com/2021/02/capture3.jpg?w=960" alt="" data-id="164" data-full-url="https://freefactsin.files.wordpress.com/2021/02/capture3.jpg" data-link="https://freefactsin.wordpress.com/capture3/" class="wp-image-164"/></figure></li><li class="blocks-gallery-item"><figure><img src="https://freefactsin.files.wordpress.com/2021/02/capture4.jpg?w=687" alt="" data-id="165" data-full-url="https://freefactsin.files.wordpress.com/2021/02/capture4.jpg" data-link="https://freefactsin.wordpress.com/capture4/" class="wp-image-165"/></figure></li><li class="blocks-gallery-item"><figure><img src="https://freefactsin.files.wordpress.com/2021/02/capture5.jpg?w=1024" alt="" data-id="166" data-full-url="https://freefactsin.files.wordpress.com/2021/02/capture5.jpg" data-link="https://freefactsin.wordpress.com/capture5/" class="wp-image-166"/></figure></li></ul><figcaption class="blocks-gallery-caption"><em>Then, I collected various images from Google and found this amazing results </em></figcaption></figure>
<!-- /wp:gallery -->

<!-- wp:paragraph -->
<p>But, if you see the 5th tile, result was scaring, it's because of the disadvantage of Yolov3 and it's limited to one class</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>That's it, This is Object Detection</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Real-time Applications of Object Detection</p>
<!-- /wp:paragraph -->

<!-- wp:list {"ordered":true} -->
<ol><li>Crowd counting</li><li>Self-driving cars</li><li>Video surveillance</li><li>Face detection</li><li>Anomaly detection</li><li>You could try whatever you want </li></ol>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p><strong>Everything is given in this link -> <a href="https://drive.google.com/file/d/151_Qtv-qaoUQQRcZF9XjdAJZBOIu2brJ/view?usp=sharing" data-type="URL" data-id="https://drive.google.com/file/d/151_Qtv-qaoUQQRcZF9XjdAJZBOIu2brJ/view?usp=sharing">https://drive.google.com/file/d/151_Qtv-qaoUQQRcZF9XjdAJZBOIu2brJ/view?usp=sharing</a></strong></p>
<!-- /wp:paragraph -->
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
