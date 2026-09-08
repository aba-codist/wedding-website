<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title> Samira & Jahid | Wedding Invitation</title>

<!-- NORMAL MODERN FONT -->

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">


<style>

/* =========================================
   GLOBAL SETTINGS
========================================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    background:#090807;
    color:#ffffff;
    font-family:'Poppins',sans-serif;
    overflow-x:hidden;
}


/* =========================================
   CUSTOM SCROLLBAR
========================================= */

::-webkit-scrollbar{
    width:8px;
}

::-webkit-scrollbar-track{
    background:#090807;
}

::-webkit-scrollbar-thumb{
    background:#d4af37;
    border-radius:10px;
}


/* =========================================
   LOADING SCREEN
========================================= */

.loader{
    position:fixed;
    inset:0;

    background:#080706;

    display:flex;
    align-items:center;
    justify-content:center;

    z-index:9999;

    transition:1s ease;
}

.loader-content{
    text-align:center;
}

.loader-ring{
    width:80px;
    height:80px;

    border:3px solid #282015;
    border-top:3px solid #d4af37;

    border-radius:50%;

    margin:auto;

    animation:spin 1.2s linear infinite;
}

.loader h2{
    margin-top:25px;

    font-size:22px;
    font-weight:500;

    color:#d4af37;

    letter-spacing:2px;
}

@keyframes spin{

    100%{
        transform:rotate(360deg);
    }

}


/* =========================================
   HERO SECTION
========================================= */

.hero{

    min-height:100vh;

    display:flex;
    align-items:center;
    justify-content:center;

    text-align:center;

    position:relative;

    background:

    linear-gradient(
        rgba(0,0,0,.55),
        rgba(0,0,0,.88)
    ),

    url("https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=1800&q=90");

    background-size:cover;
    background-position:center;

}

.hero::before{

    content:"";

    position:absolute;

    inset:0;

    background:

    radial-gradient(
        circle,
        transparent 20%,
        rgba(0,0,0,.7)
    );

}

.hero-content{

    position:relative;
    z-index:2;

    max-width:1000px;

    padding:50px 25px;

    animation:heroAnimation 1.5s ease;
}


@keyframes heroAnimation{

    from{
        opacity:0;
        transform:translateY(40px);
    }

    to{
        opacity:1;
        transform:translateY(0);
    }

}


.hero-top{

    font-size:13px;

    letter-spacing:6px;

    color:#d4af37;

    margin-bottom:25px;

}


.hero h1{

    font-size:clamp(60px,10vw,130px);

    font-weight:700;

    line-height:1;

    margin-bottom:25px;

    background:

    linear-gradient(
        90deg,
        #b8860b,
        #fff1a8,
        #d4af37,
        #fff1a8,
        #b8860b
    );

    -webkit-background-clip:text;

    color:transparent;

}


.hero-description{

    font-size:16px;

    color:#dddddd;

    letter-spacing:2px;

}


.hero-date{

    display:inline-block;

    margin-top:35px;

    padding:16px 35px;

    border-top:1px solid #d4af37;

    border-bottom:1px solid #d4af37;

    color:#f7e7a1;

    font-size:14px;

    letter-spacing:2px;

}


/* =========================================
   FLOATING GOLD PARTICLES
========================================= */

.particle{

    position:fixed;

    width:5px;
    height:5px;

    background:#d4af37;

    border-radius:50%;

    pointer-events:none;

    z-index:5;

    animation:floatUp linear infinite;

}


@keyframes floatUp{

    0%{

        transform:translateY(110vh);

        opacity:0;

    }

    20%{
        opacity:.8;
    }

    100%{

        transform:translateY(-10vh);

        opacity:0;

    }

}


/* =========================================
   COMMON SECTION
========================================= */

section{

    padding:110px 8%;

}

.section-small{

    text-align:center;

    color:#d4af37;

    font-size:12px;

    font-weight:600;

    letter-spacing:5px;

    margin-bottom:15px;

}


.section-title{

    text-align:center;

    font-size:clamp(35px,5vw,65px);

    font-weight:700;

    margin-bottom:60px;

    color:#ffffff;

}


.gold-line{

    width:80px;
    height:3px;

    background:#d4af37;

    margin:20px auto 0;

}


/* =========================================
   INVITATION SECTION
========================================= */

.invitation-box{

    max-width:950px;

    margin:auto;

    padding:70px 50px;

    text-align:center;

    background:

    linear-gradient(
        135deg,
        #18140d,
        #090807
    );

    border:1px solid rgba(212,175,55,.35);

    box-shadow:

    0 25px 70px rgba(0,0,0,.5);

    position:relative;

}


.invitation-box::before{

    content:"✦";

    position:absolute;

    top:-25px;

    left:50%;

    transform:translateX(-50%);

    font-size:45px;

    color:#d4af37;

    background:#090807;

    padding:0 20px;

}


.invitation-box p{

    color:#cccccc;

    font-size:17px;

    line-height:2;

}


/* =========================================
   COUPLE SECTION
========================================= */

.couple-container{

    display:grid;

    grid-template-columns:repeat(2,1fr);

    gap:40px;

    max-width:1200px;

    margin:auto;

}


.person-card{

    text-align:center;

    padding:50px 30px;

    background:

    linear-gradient(
        145deg,
        #19140e,
        #090807
    );

    border:1px solid rgba(212,175,55,.25);

    transition:.5s ease;

}


.person-card:hover{

    transform:translateY(-12px);

    border-color:#d4af37;

    box-shadow:

    0 25px 60px rgba(212,175,55,.12);

}


.person-image{

    width:220px;
    height:220px;

    margin:auto;

    padding:7px;

    border-radius:50%;

    background:

    linear-gradient(
        135deg,
        #8a6500,
        #f7e7a1,
        #d4af37
    );

}


.person-image img{

    width:100%;
    height:100%;

    object-fit:cover;

    border-radius:50%;

}


.person-role{

    margin-top:25px;

    font-size:12px;

    font-weight:600;

    letter-spacing:5px;

    color:#d4af37;

}


.person-card h2{

    font-size:42px;

    font-weight:700;

    margin:15px 0 25px;

    color:#ffffff;

}


.family-details{

    border-top:

    1px solid rgba(212,175,55,.2);

    padding-top:20px;

}


.family-details p{

    margin:13px 0;

    font-size:15px;

    color:#bbbbbb;

}


.family-details strong{

    color:#f7e7a1;

    font-weight:600;

}


/* =========================================
   COUNTDOWN
========================================= */

.countdown-section{

    background:

    linear-gradient(
        rgba(0,0,0,.82),
        rgba(0,0,0,.9)
    ),

    url("https://images.unsplash.com/photo-1519225421980-715cb0215aed?auto=format&fit=crop&w=1800&q=90");

    background-size:cover;

    background-position:center;

    background-attachment:fixed;

}


.countdown{

    display:flex;

    justify-content:center;

    gap:20px;

    flex-wrap:wrap;

}


.time-box{

    width:150px;

    padding:30px 10px;

    text-align:center;

    background:rgba(0,0,0,.55);

    border:1px solid rgba(212,175,55,.45);

    backdrop-filter:blur(10px);

}


.time-box h2{

    font-size:45px;

    color:#f7e7a1;

}


.time-box span{

    font-size:11px;

    letter-spacing:3px;

    color:#aaaaaa;

}


/* =========================================
   EVENTS SECTION
========================================= */

.events{

    display:grid;

    grid-template-columns:repeat(3,1fr);

    gap:25px;

    max-width:1200px;

    margin:auto;

}


.event-card{

    padding:45px 25px;

    text-align:center;

    background:#100e0a;

    border:1px solid rgba(212,175,55,.25);

    transition:.4s;

}


.event-card:hover{

    transform:translateY(-10px);

    border-color:#d4af37;

}


.event-icon{

    font-size:40px;

    margin-bottom:20px;

}


.event-card h3{

    font-size:20px;

    font-weight:600;

    color:#f7e7a1;

    margin-bottom:18px;

}


.event-card p{

    color:#aaaaaa;

    line-height:1.8;

    font-size:14px;

}


/* =========================================
   VENUE SECTION
========================================= */

.venue-container{

    max-width:1200px;

    margin:auto;

    background:#0e0c09;

    border:1px solid rgba(212,175,55,.3);

    overflow:hidden;

}


.venue-image{

    height:500px;

    position:relative;

}


.venue-image img{

    width:100%;
    height:100%;

    object-fit:cover;

}


.venue-image::after{

    content:"";

    position:absolute;

    inset:0;

    background:

    linear-gradient(
        transparent,
        rgba(0,0,0,.8)
    );

}


.venue-details{

    padding:60px 30px;

    text-align:center;

}


.venue-details h2{

    font-size:35px;

    font-weight:700;

    color:#f7e7a1;

    margin-bottom:25px;

}


.venue-details p{

    color:#bbbbbb;

    font-size:15px;

    line-height:2;

}


.location-btn{

    display:inline-block;

    margin-top:30px;

    padding:17px 40px;

    background:

    linear-gradient(
        90deg,
        #b8860b,
        #f7e7a1,
        #d4af37
    );

    color:#111111;

    text-decoration:none;

    font-size:14px;

    font-weight:600;

    transition:.4s;

}


.location-btn:hover{

    transform:scale(1.06);

}


/* =========================================
   RSVP SECTION
========================================= */

.rsvp{

    text-align:center;

    background:

    radial-gradient(
        circle,
        #2a210d,
        #080706
    );

}


.rsvp-box{

    max-width:750px;

    margin:auto;

}


.rsvp-box h2{

    font-size:clamp(45px,7vw,85px);

    font-weight:700;

    color:#f7e7a1;

}


.rsvp-box p{

    color:#bbbbbb;

    line-height:2;

    margin:25px 0;

}


.rsvp-btn{

    display:inline-block;

    padding:18px 45px;

    background:#d4af37;

    color:#111;

    text-decoration:none;

    font-weight:600;

    transition:.3s;

}


.rsvp-btn:hover{

    background:#fff0a5;

    transform:translateY(-5px);

}


/* =========================================
   FOOTER
========================================= */

footer{

    text-align:center;

    padding:35px;

    background:#050504;

    color:#777777;

    font-size:13px;

}


/* =========================================
   RESPONSIVE DESIGN
========================================= */

@media(max-width:850px){

    section{
        padding:80px 6%;
    }

    .couple-container{
        grid-template-columns:1fr;
    }

    .events{
        grid-template-columns:1fr;
    }

    .hero-top{
        letter-spacing:3px;
    }

    .hero-description{
        font-size:13px;
    }

    .venue-image{
        height:300px;
    }

}


@media(max-width:500px){

    .invitation-box{
        padding:55px 25px;
    }

    .person-image{
        width:180px;
        height:180px;
    }

    .time-box{
        width:130px;
    }

    .hero-date{
        padding:15px 20px;
        font-size:12px;
    }

}

</style>

</head>


<body>


<!-- =====================================
     LOADER
===================================== -->

<div class="loader" id="loader">

    <div class="loader-content">

        <div class="loader-ring"></div>

        <h2>OUR FOREVER BEGINS</h2>

    </div>

</div>



<!-- =====================================
     HERO
===================================== -->

<section class="hero">

    <div class="hero-content">

        <p class="hero-top">
            TOGETHER WITH THEIR FAMILIES
        </p>


        <h1>
            SAMIRA <br> & <br> JAHID
        </h1>


        <p class="hero-description">
            REQUEST THE HONOUR OF YOUR PRESENCE
        </p>


        <div class="hero-date">

            SATURDAY • 20 DECEMBER 2026 • 06:30 PM

        </div>

    </div>

</section>



<!-- =====================================
     INVITATION MESSAGE
===================================== -->

<section>

    <p class="section-small">
        A BEAUTIFUL BEGINNING
    </p>


    <h1 class="section-title">

        A Celebration Of Love

        <div class="gold-line"></div>

    </h1>


    <div class="invitation-box">

        <p>

            With immense joy and happiness,
            together with our beloved families,
            we invite you to celebrate the beginning
            of our beautiful journey together.

            <br><br>

            Your presence, love and blessings
            will make our special day even more
            memorable and meaningful.

        </p>

    </div>

</section>



<!-- =====================================
     COUPLE SECTION
===================================== -->

<section>

    <p class="section-small">
        THE BEAUTIFUL COUPLE
    </p>


    <h1 class="section-title">

        Meet The Couple

        <div class="gold-line"></div>

    </h1>



    <div class="couple-container">


        <!-- GROOM -->

        <div class="person-card">

            <div class="person-image">

                <img
                src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?auto=format&fit=crop&w=700&q=90"
                alt="Groom">

            </div>


            <p class="person-role">
                THE GROOM
            </p>


            <h2>
                Jahid
            </h2>


            <div class="family-details">

                <p>

                    <strong>Father:</strong>

                    Mr. Rahman Ahmed

                </p>


                <p>

                    <strong>Mother:</strong>

                    Mrs. Fatema Rahman

                </p>


                <p>
                    📍 Chattogram, Bangladesh
                </p>

            </div>

        </div>



        <!-- BRIDE -->

        <div class="person-card">

            <div class="person-image">

                <img
                src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?auto=format&fit=crop&w=700&q=90"
                alt="Bride">

            </div>


            <p class="person-role">
                THE BRIDE
            </p>


            <h2>
                Samira
            </h2>


            <div class="family-details">

                <p>

                    <strong>Father:</strong>

                    Mr. Karim Islam

                </p>


                <p>

                    <strong>Mother:</strong>

                    Mrs. Salma Karim

                </p>


                <p>
                    📍 Dhaka, Bangladesh
                </p>

            </div>

        </div>


    </div>

</section>



<!-- =====================================
     COUNTDOWN
===================================== -->

<section class="countdown-section">

    <p class="section-small">
        THE BIG DAY IS COMING
    </p>


    <h1 class="section-title">

        Counting Every Moment

        <div class="gold-line"></div>

    </h1>


    <div class="countdown">


        <div class="time-box">

            <h2 id="days">00</h2>

            <span>DAYS</span>

        </div>



        <div class="time-box">

            <h2 id="hours">00</h2>

            <span>HOURS</span>

        </div>



        <div class="time-box">

            <h2 id="minutes">00</h2>

            <span>MINUTES</span>

        </div>



        <div class="time-box">

            <h2 id="seconds">00</h2>

            <span>SECONDS</span>

        </div>


    </div>

</section>



<!-- =====================================
     EVENTS
===================================== -->

<section>

    <p class="section-small">
        CELEBRATE WITH US
    </p>


    <h1 class="section-title">

        Wedding Events

        <div class="gold-line"></div>

    </h1>


    <div class="events">


        <div class="event-card">

            <div class="event-icon">
                💍
            </div>

            <h3>
                Wedding Ceremony
            </h3>

            <p>
                20 December 2026
            </p>

            <p>
                06:30 PM
            </p>

        </div>



        <div class="event-card">

            <div class="event-icon">
                🥂
            </div>

            <h3>
                Grand Reception
            </h3>

            <p>
                21 December 2026
            </p>

            <p>
                07:00 PM
            </p>

        </div>



        <div class="event-card">

            <div class="event-icon">
                ❤️
            </div>

            <h3>
                Dinner & Celebration
            </h3>

            <p>
                An Evening Of Love
            </p>

            <p>
                With Family & Friends
            </p>

        </div>


    </div>

</section>



<!-- =====================================
     VENUE
===================================== -->

<section>

    <p class="section-small">
        THE PLACE WHERE MAGIC HAPPENS
    </p>


    <h1 class="section-title">

        Wedding Venue

        <div class="gold-line"></div>

    </h1>



    <div class="venue-container">


        <div class="venue-image">

            <img
            src="https://images.unsplash.com/photo-1464366400600-7168b8af9bc3?auto=format&fit=crop&w=1800&q=90"
            alt="Wedding Venue">

        </div>



        <div class="venue-details">


            <h2>
                Royal Grand Convention Hall
            </h2>


            <p>
                📍 123 Wedding Avenue
            </p>


            <p>
                Chattogram, Bangladesh
            </p>


            <p>

                ✨ Join us for an unforgettable evening
                filled with love, happiness,
                laughter and beautiful memories.

            </p>



            <a
            href="https://maps.google.com"
            target="_blank"
            class="location-btn">

                VIEW LOCATION 📍

            </a>


        </div>


    </div>

</section>



<!-- =====================================
     RSVP
===================================== -->

<section class="rsvp">

    <div class="rsvp-box">


        <h2>
            Save The Date
        </h2>


        <p>

            Your presence will make our special day
            even more beautiful.

            <br>

            We look forward to celebrating
            this unforgettable moment with you.

        </p>


        <a href="#" class="rsvp-btn">

            Click For Home 💌

        </a>


    </div>

</section>



<!-- =====================================
     FOOTER
===================================== -->

<footer>

    Made With ❤️ For Samira & Jahid

    <br><br>

    © 2026 • A Celebration Of Love & Forever

</footer>



<!-- =====================================
     JAVASCRIPT
===================================== -->

<script>


/* =========================================
   LOADER
========================================= */

window.addEventListener("load",function(){

    setTimeout(function(){

        const loader =
        document.getElementById("loader");

        loader.style.opacity="0";

        loader.style.visibility="hidden";

    },1500);

});



/* =========================================
   COUNTDOWN
========================================= */

const weddingDate =
new Date("December 20, 2026 18:30:00").getTime();


const countdownInterval =
setInterval(function(){


    const now =
    new Date().getTime();


    const distance =
    weddingDate-now;



    if(distance < 0){

        clearInterval(countdownInterval);

        document.getElementById("days").innerHTML="00";

        document.getElementById("hours").innerHTML="00";

        document.getElementById("minutes").innerHTML="00";

        document.getElementById("seconds").innerHTML="00";

        return;

    }



    const days =
    Math.floor(
        distance/(1000*60*60*24)
    );



    const hours =
    Math.floor(

        (distance%
        (1000*60*60*24))

        /(1000*60*60)

    );



    const minutes =
    Math.floor(

        (distance%
        (1000*60*60))

        /(1000*60)

    );



    const seconds =
    Math.floor(

        (distance%
        (1000*60))

        /1000

    );



    document.getElementById("days").innerHTML=days;

    document.getElementById("hours").innerHTML=hours;

    document.getElementById("minutes").innerHTML=minutes;

    document.getElementById("seconds").innerHTML=seconds;


},1000);



/* =========================================
   FLOATING GOLD PARTICLES
========================================= */

function createParticle(){


    const particle =
    document.createElement("div");


    particle.classList.add("particle");


    particle.style.left =
    Math.random()*100+"vw";


    particle.style.animationDuration =
    Math.random()*8+7+"s";


    const size =
    Math.random()*5+2;


    particle.style.width =
    size+"px";


    particle.style.height =
    size+"px";


    document.body.appendChild(particle);



    setTimeout(function(){

        particle.remove();

    },15000);


}


/* CREATE PARTICLES */

setInterval(createParticle,600);


</script>


</body>

</html>
