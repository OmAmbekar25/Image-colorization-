<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Colorization - README</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 40px;
            line-height: 1.6;
        }
        h1, h2, h3 {
            color: #333;
        }
        a {
            color: blue;
        }
        img {
            max-width: 100%;
            height: auto;
            display: block;
            margin: 20px 0;
        }
    </style>
</head>
<body>
    <h1>Image Colorization - README</h1>
    
    <h2>Introduction</h2>
    <p>Image colorization is a compelling field in computer vision that focuses on converting grayscale or monochrome images into color images. This process is valuable for restoring historical photographs, enhancing media visuals, and improving usability in various applications.Historically, image colorization has been performed manually, a labor-intensive process requiring considerable artistic skill. However, advancements in machine learning and deep learning have revolutionized this field, making automated colorization more efficient and accessible.

The latest neural network technique involves the use of Resnet for feature extraction and combines or fusing it with a layer that comes after pooling/downsampling of the input or encoded layer and then decoding it with convolution layers through upsampling to predict the colored image. Also, there are various types of GAN such as pix2pix GAN, Cycle gan which are much more advanced techniques for image colorization.
The auto-encoder network which I have explained in this model also servers the purpose of a generator in the GAN network. There understanding this notebook would help you further in understanding complex networks and methodologies involved in image colorization.
Today, colorization is usually done by hand in Photoshop. To appreciate all the hard work behind this process, take a peek at this gorgeous colorization memory lane video:
In short, a picture can take up to one month to colorize. It requires extensive research. A face alone needs up to 20 layers of pink, green and blue shades to get it just right.
This article is for beginners. Yet, if you’re new to deep learning terminology, you can read my previous two posts here and here, and watch Andrej Karpathy’s lecture for more background.
The first section breaks down the core logic. We’ll build a bare-bones 40-line neural network as an
―alpha‖ colorization bot. There’s not a lot of magic in this code snippet. This well help us become familiar with the syntax.
The next step is to create a neural network that can generalize — our ―beta‖ version. We’ll be able to color images the bot has not seen before.
For our ―final‖ version, we’ll combine our neural network with a classifier. We’ll use an Inception Resnet V2 that has been trained on 1.2 million images. To make the coloring pop, we’ll train our neural network on portraits from Unsplash
</p>
    <img src="images/introduction.jpg" alt="Image Colorization Example">
    
    <h2>Abstract</h2>
    <p>Image colorization is the process of converting grayscale images into colored ones, leveraging deep learning techniques. Modern approaches use CNNs to predict color information by training on large datasets of paired grayscale and colored images.</p>
    
    <h2>Scope of the Study</h2>
    <ul>
        <li>Traditional vs. modern colorization techniques.</li>
        <li>Deep learning models like CNNs, GANs, and autoencoders.</li>
        <li>Applications in media, medical imaging, and historical restoration.</li>
    </ul>
    <img src="images/scope.jpg" alt="Scope of Image Colorization">
    
    <h2>Methodology</h2>
    <p>The methodology includes data collection, preprocessing, model training, and evaluation. Techniques include:</p>
    <ul>
        <li><strong>RGB Space-based Method:</strong> Uses three color channels (R, G, B).</li>
        <li><strong>Separable Space-based Method:</strong> Uses CIELAB, YUV, and HSV color spaces.</li>
    </ul>
    <img src="images/methodology.jpg" alt="Colorization Process">
    
    <h2>Challenges</h2>
    <ul>
        <li>Loss of color information in grayscale images.</li>
        <li>Ambiguity in grayscale representations.</li>
        <li>High computational complexity for training models.</li>
        <li>Perceptual color constancy and color bleeding.</li>
    </ul>
    <img src="images/challenges.jpg" alt="Challenges in Colorization">
    
    <h2>Traditional Approaches</h2>
    <ul>
        <li>Manual colorization techniques.</li>
        <li>Rule-based methods.</li>
        <li>Color propagation techniques.</li>
    </ul>
    
    <h2>Conclusion</h2>
    <p>Deep learning has revolutionized image colorization, making it more efficient and widely applicable. Ongoing research aims to enhance accuracy and generalization.</p>
    
    <h2>Flowchart</h2>
    <img src="images/flowchart.jpg" alt="Image Colorization Flowchart">
    
    <h2>References</h2>
    <ul>
        <li><a href="https://www.freecodecamp.org/news/colorize-b-w-photos-with-a-100-line-neural-network-53d9b4449f8d" target="_blank">FreeCodeCamp: Neural Network for Colorization</a></li>
        <li><a href="https://www.learnopencv.com/convolutional-neural-network-based-image-colorization-using-opencv/" target="_blank">OpenCV: CNN-Based Colorization</a></li>
        <li><a href="https://www.kaggle.com/code/basu369victor/image-colorization-basic-implementation-with-cnn" target="_blank">Kaggle: Image Colorization Implementation</a></li>
        <li><a href="https://www.researchgate.net/publication/301817406_Image_Colorization_Using_a_Deep_Convolutional_Neural_Network" target="_blank">ResearchGate: Deep CNN for Colorization</a></li>
    </ul>
</body>
</html>
