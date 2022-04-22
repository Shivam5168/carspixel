# carspixel
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carspix</title>
    <link rel="stylesheet" href="webcars.css">
    <script src="https://kit.fontawesome.com/0e87ba70fc.js" crossorigin="anonymous"></script>
</head>
<body>
    <header>
        <nav>
            <div class="logo" title="Welcome, to Carspix.">
                <p>Cars<span>pi</span>x</p>
            </div>
        <div class="nav-bar">
            <a href="#">Home</a>
            <a href="#">About</a>
            <a href="#">Gallary</a>
            <a href="#">Contact</a>
        </div>
        <div class="icon">
            <i class="fa fa-search"></i>
            <a href="#" >Login</a>
        </div>
        </nav>
        <section class="h-text">
            <i class="fa fa-camera" id="camera"></i>
            <h1 data-aos="zoom-in-down" data-aos-delay="100" class="aos-init aos-animate">Capturing the moments that captivate your heart.</h1>
            <input type="text" name="text" class="text" placeholder="Search here...">
            <button><i class="fa fa-search"></i></button>
        </section>
    </header>
    <section class="gallary">
       <div class="gallary-feed">
        <ul>
           <li class="active" data-filter="*">All</li>
           <li data-filter=".SUV">SUV</li>
           <li data-filter=".supercar">Super Cars</li>
        </ul>
        </div>
       <div class="gallary-pics">
       <div class="pics SUV">
       <img src="./images/1.jpg" alt="image1" width="100" height="100">
       </div>
       <div class="pics supercar">
        <img src="./images/s1.jpg" alt="image5" width="100" height="100">
        </div>

      
    <div class="pics supercar">
        <img src="./images/s2.jpg" alt="image6" width="100" height="100">
        </div>
    <div class="pics SUV">
        <img src="./images/3.jpg" alt="image3" width="100" height="100">
    </div>
    <div class="pics supercar">
        <img src="./images/s4.jpg" alt="image7" width="100" height="100">
     </div>
    <div class="pics SUV">
       <img src="./images/4.jpg" alt="image4" width="100" height="100">
    </div>
    <div class="pics supercar">
        <img src="./images/s5.jpg" alt="image8" width="100" height="100">
     </div>
     <div>

     </section>
    
    <section class="member">
        
            <div class="member-text">
            <h2>Our <span>Information</span></h2>
            <p>what our member says</p>
            </div>
            <div class="member-info">
            <img src="./images/maa.jpg"  alt="maa" height="100" width="100">
            <p>From Bihar, here you can gets best pics of cars.It helps you to find the best cars.I am a B.tech Cumputer Science Engineering Student.I am learning Web Development.This is my first full front-end website.This website contain <span>HTML,CSS</span>&nbsp;and&nbsp;<span>Javascript.</span></p>
            </div>
            <div class="member-name">
                <h2>* Shivam Pradhan</h2>
            </div>
            <div class="member-social">
               <ul>
                   <li><img src="./images/m1.jpg" alt="instagram" height="100" width="100"> </li>
                   <li><img src="./images/m2.jpg" alt="youtube" height="100" width="100"> </li>
                </ul>
            </div>
                <div class="member-image">
                    <img src="./images/mi1.jpg" alt="image1">
                    <img src="./images/mi2.jpg" alt="image2">
                    <img src="./images/mi3.jpg" alt="image3">
                    <img src="./images/mi4.jpg" alt="image4">
                    <img src="./images/mi5.jpg" alt="image5">
                    <img src="./images/mi6.jpg" alt="image6">
                </div>
    </section>
    <footer>
        <div class="subscribe">
            <div>
            <h2>Subscribe our Page</h2>
            <p>we are a team,and we love your work</p>
        </div>
        
            <div class="ntext">
                <label>
            <input type="text" placeholder="Enter your email...">
            <button>Subscribe</button>
                </label>
            </div>
        </div>
            <div class="f-contact">
                <div>
                <h1>Information</h1>
                <p class="p-text">A car (or automobile) is a wheeled motor vehicle used for transportation. Most definitions of cars say that they run primarily on roads, seat one to eight people, have four wheels, and mainly transport people rather than goods.
                    <a href="https://en.wikipedia.org/wiki/Car" target="_blank">click.</a></p>
                 <i class = "fa fa-whatsapp"></i>
                 <i class = "fa fa-instagram"></i>
                 <i class = "fa fa-telegram"></i>
                 <i class = "fa fa-twitter"></i>
                </div>
            
            <div>
                <h1>Useful links</h1>
                <p>About us</p>
                <p>Gallary</p>
                <p>Blog posts</p>
                <p>Pricing Plans</p>
            </div>
            <div>
                <h1>Details</h1>
                <p>Photographers</p>
                <p>Gallary</p>
                <p>About</p>
                <p>Pricing Plans</p>
            </div>
            <div>
                <h1>Help & Support</h1>
                <p> Privacy policy</p>
                <p>Term & conditions</p>
                <p>Technical support</p>
                <p>Customer care</p>
               
            </div>
        </div>
        <div class="footer-line"></div>
        
    </footer>
    
    
    <script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4=" crossorigin="anonymous"></script>
     <script src="https://unpkg.com/isotope-layout@3/dist/isotope.pkgd.min.js"></script>
     <script type="text/javascript">
        $('.gallary-pics').isotope({
 // options
     itemSelector: '.pics',
     layoutMode: 'fitRows'
      });

      $('.gallary-feed ul li').click(function(){
      $('.gallary-feed ul li').removeClass('active');
      $(this).addClass('active');
     
      var selector = $(this).attr('data-filter');
      $('.gallary-pics').isotope({
          filter:selector
      });
      return false;
    });
   
   </script>
</body>
</html>
