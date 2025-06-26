<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />

    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" />
    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet" />
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>


</head>

<body>

    <div class="container">
        <div class="row">

            <div class="col-12 order-1 video-container ">
                <style>
                    .gradient-container {
                        background-color: linear-gradient(to top, #1e293b 15%, #16284521 78%, #0000);

                    }

                    @media (max-width: 768px) {
                        .gradient-container {
                            background-color: linear-gradient(to right, #1e293b 15%, #16284521 78%, #0000);
                        }
                    }

                    .carousel-box {
                        height: 90px;
                        overflow: hidden;
                        position: relative;
                    }

                    .carousel-wrapper {
                        position: absolute;

                        width: 100%;
                        transition: transform 0.6s ease-in-out;
                    }

                    .carousel-item-text {
                        height: 90px;
                    }

                    .vertical-slider-h5 {
                        color: #ffffff;
                        font-weight: bold;
                    }

                    .vertical-slider-img {
                        height: 30px;
                        margin: 0 6px;
                    }

                    .vertical-slider-btn1 {
                        text-transform: capitalize;
                        background-color: #a3e635;
                        width: 80%;
                        color: #ffffff;
                        font-size: 20px;
                        font-weight: 500;
                        border-style: none;
                        border-radius: 5px;
                        margin: 10px 0;
                        font-family: "Roboto", sans-serif;
                        padding: 10px;
                        max-width: 250px;
                    }

                    #vertical-slider-btn2 {
                        background-color: transparent;
                        border-color: #ffffff;
                        border-style: solid;
                        border-width: 1px;
                    }



                    .vertical-slider-span {
                        position: absolute;
                        right: 20%;
                        color: #a3e635;
                    }

                    .vertical-slider-p {
                        font-weight: bold;
                        color: #ffffff;
                        position: relative;
                        display: inline-block;
                    }

                    .vector-img {
                        position: absolute;
                        top: 5px;
                        right: 14px;
                        height: 18px;
                        z-index: 2;
                    }

                    .vertical-slider-span2 {
                        color: #a3e635;
                        font-weight: bold
                    }












                    html {

                        height: 100%;
                    }

                    .video-container {
                        position: relative;
                        width: 100%;
                        height: 100vh;
                        overflow: hidden;

                    }

                    #bg-video {
                        position: absolute;
                        top: 0;
                        left: 0;
                        width: 100%;
                        height: 100%;
                        object-fit: cover;
                        z-index: 1;
                    }

                    .container-nxt-talks {
                        position: absolute;
                        top: 0;
                        left: 0;
                        z-index: 2;
                        padding: 1rem;
                    }

                    .img-nxt-talks {
                        width: 200px;
                        height: auto;
                        display: block;
                        position: relative;
                    }

                    .h4-nxt-talks {
                        position: absolute;
                        top: 42px;
                        right: 5px;
                        font-size: 1rem;
                        color: white;
                    }

                    .container-nxt-talks-wrapper {
                        position: relative;
                        display: inline-block;
                    }

                    .vertical-slider-container {
                        position: absolute;

                        z-index: 2;
                        top: 45%;
                        padding: 1rem;

                    }



                    /* Default: small devices (bottom center) */
                    @media (max-width: 767.98px) {
                        .vertical-slider-container {
                            top: 55%;
                            left: 50%;
                            transform: translateX(-50%);


                        }
                    }

                    /* Medium devices and up: align to left vertically centered */
                    @media (min-width: 768px) {
                        .vertical-slider-container {
                            top: 60%;
                            padding-left: 40%;
                            transform: translateY(-33%);
                            width: 70vw;
                            height: 150vh;
                            /* Optional: adjust as needed */
                            max-width: 400px;
                        }
                    }


                    .horizontal-slider-bg {
                        background-color: #0d1117;

                    }


                    .horizontal-slider-h1 {
                        font-weight: bold;
                        text-transform: capitalize;
                        color: #ffffff;
                    }
                </style>

                <div>
                    <video id="bg-video" autoplay muted playsinline></video>

                    <!-- Overlay container in top-left -->
                    <div class="container-nxt-talks">
                        <div class="container-nxt-talks-wrapper">
                            <img class="img-nxt-talks" src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/64362e90abbff4d11fd25fa9_Frame%201000003044%20(2).svg" alt="Next Talks Banner" />
                            <h4 class="h4-nxt-talks">by NxtWave</h4>
                        </div>
                    </div>










                    <div class="container  gradient-container  vertical-slider-container p-4  ">

                        <!-- Vertical Slider -->
                        <div class="carousel-box mb-4">
                            <div class="carousel-wrapper" id="vertical-slider">
                                <div class="carousel-item-text d-flex justify-content-center align-items-center">
                                    <h5 class="vertical-slider-h5">A Manager at
                                        <span><img class="vertical-slider-img" src="https://uploads-ssl.webflow.com/64362e90abbff481a6d25ce8/64362e90abbff441edd25f5e_Uber.svg" alt="Uber" /></span>
                                        Teaches you about <span class="vertical-slider-span2">Programming</span>
                                    </h5>
                                </div>
                                <div class="carousel-item-text d-flex justify-content-center align-items-center ">
                                    <h5 class="vertical-slider-h5">A Sr. Recruiter at
                                        <span><img class="vertical-slider-img" src="https://uploads-ssl.webflow.com/64362e90abbff481a6d25ce8/64362e90abbff483f9d25f89_Frame%201000002924%20(1).svg" alt="Frame" /></span>
                                        Teaches about <span class="vertical-slider-span2">Acing Interviews</span>
                                    </h5>
                                </div>
                                <div class="carousel-item-text d-flex justify-content-center align-items-center ">
                                    <h5 class="vertical-slider-h5">A CEO at
                                        <span><img class="vertical-slider-img" src="https://uploads-ssl.webflow.com/64362e90abbff481a6d25ce8/64362e90abbff4e82fd25f85_Msys.svg" alt="Msys" /></span>
                                        Teaches about <span class="vertical-slider-span2">Entrepreneurship</span>
                                    </h5>
                                </div>
                                <div class="carousel-item-text d-flex justify-content-center align-items-center ">
                                    <h5 class="vertical-slider-h5">A Sr. Manager at
                                        <img class="vertical-slider-img" src="https://uploads-ssl.webflow.com/64362e90abbff481a6d25ce8/64362e90abbff44006d25f7f_Frame%201000002982.svg" alt="Frame" />
                                        Teaches you about <span class="vertical-slider-span2">Product Management</span>
                                    </h5>
                                </div>
                                <div class="carousel-item-text d-flex justify-content-center align-items-center ">
                                    <h5 class="vertical-slider-h5">A CTO at
                                        <img class="vertical-slider-img" src="https://uploads-ssl.webflow.com/64362e90abbff481a6d25ce8/64362e90abbff492bed25fa5_logo.27a7f72e%20(1)%201.svg" alt="CTO" />
                                        Teaches you about <span class="vertical-slider-span2">Leadership</span>
                                    </h5>
                                </div>
                                <div class="carousel-item-text d-flex justify-content-center align-items-center ">
                                    <h5 class="vertical-slider-h5">A Lead at
                                        <img class="vertical-slider-img" src="https://uploads-ssl.webflow.com/64362e90abbff481a6d25ce8/64362e90abbff4511cd25f81_SuperK.svg" alt="SuperK" />
                                        Teaches you about <span class="vertical-slider-span2">Career Designing</span>
                                    </h5>
                                </div>
                            </div>
                        </div>

                        <!-- Buttons -->
                        <div class="d-flex flex-column align-items-center ">
                            <a href="#claim-your-free-access-section2" class="d-md-none"> <button class="vertical-slider-btn1 ">Claim Free Access</button></a>
                            <a href="#claim-your-free-access-section1" class=" d-none d-md-block"> <button class="vertical-slider-btn1 ">Claim Free Access</button></a>
                            <button class="vertical-slider-btn1" id="vertical-slider-btn2">Watch Trailer</button>
                        </div>

                        <!-- CTA -->
                        <div class="d-flex flex-row  justify-content-center  ">
                            <p class="vertical-slider-p">Get 1 Podcast worth ₹2000


                                <img class="vector-img" src="https://uploads-ssl.webflow.com/64362e90abbff481a6d25ce8/64362e90abbff450f5d25f9f_Vector%201.png" alt="Free icon" />

                                <span class="vertical-slider-span2">Free</span>
                            </p>
                        </div>
                    </div>













                </div>

            </div>




            <div class="col-12 order-2 horizontal-slider-bg p-3">
                <div>

                    <div>
                        <style>
                            .horizontal-slider-bg {
                                background-color: #0f172a;
                                padding-top: 15%;
                                height: 110%;

                            }

                            .horizontal-slider-h2 {
                                text-transform: capitalize;
                                color: #f1f5f9;
                                font-family: Satoshi, sans-serif;
                                font-size: 48px;
                                font-weight: 700;
                                margin-bottom: 64px;


                                padding: 10px;
                                line-height: 72px;

                            }
                        </style>
                        <div class="horizontal-slider-h2 d-flex flex-row justify-content-center">
                            <h2>our speakers come from <br />your dream companies</h2>
                        </div>

                        <div>


                            <style>
                                .slider-container {
                                    overflow: hidden;
                                    width: 100%;
                                    margin-bottom: 30px;
                                    /* space between sliders */
                                }

                                .slider-track {
                                    display: flex;
                                    width: fit-content;
                                    animation-timing-function: linear;
                                    animation-iteration-count: infinite;
                                    animation-name: scrollLeft;
                                }

                                /* First slider scroll speed */
                                .slider-track.row1 {
                                    animation-duration: 50s;
                                }

                                /* Second slider scroll speed (can be same or different) */
                                .slider-track.row2 {
                                    animation-duration: 50s;
                                }

                                .slider-item img {
                                    height: 80px;
                                    width: auto;
                                    margin-right: 30px;

                                }

                                @keyframes scrollLeft {
                                    0% {
                                        transform: translateX(0%);
                                    }

                                    100% {
                                        transform: translateX(-50%);
                                    }
                                }

                                @media (max-width: 767.98px) {

                                    .horizontal-slider-bg {

                                        height: 100%;

                                    }

                                }
                            </style>

                            <div class="container-fluid slider-container  ">
                                <div class="slider-track row1">
                                    <div class="slider-item">
                                        <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/our-speaker-come-from-section/company-scroll-strip-row-1.png" alt="Row 1 Image" />
                                    </div>
                                    <div class="slider-item">
                                        <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/our-speaker-come-from-section/company-scroll-strip-row-1.png" alt="Row 1 Image" />
                                    </div>
                                </div>
                            </div>




                            <div class="container-fluid slider-container ">
                                <div class="slider-track row2">
                                    <div class="slider-item">
                                        <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/our-speaker-come-from-section/company-scroll-strip-row-2.png" alt="Row 2 Image" />
                                    </div>
                                    <div class="slider-item">
                                        <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/our-speaker-come-from-section/company-scroll-strip-row-2.png" alt="Row 2 Image" />
                                    </div>
                                </div>
                            </div>

                        </div>


                    </div>
                </div>
            </div>



            <div class="col-12  order-3 bg-row p-5">
                <div class="container ">


                    <div>

                        <div>

                            <h2 class="row3-h2">A Rare Collection of Insider<br />Knowledge, All Yours!</h2>
                            <p class="row-p3">All secrets uncovered. Exclusive insights, Timely Advice and Personal Growth Journeys straight from the tech experts.</p>


                            <style>
                                .bg-row {
                                    background-color: #1e293b;
                                    background-image: url(https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/64362e90abbff4b212d25fe3_A%20Rare%20Collection%20of%20Insider%20%20Knowledge%2C%20All%20Yours!%20\(1\).png);
                                    background-size: cover;
                                    width: 100%;

                                }

                                .row3-h2 {
                                    color: #f1f5f9;
                                    text-align: center;
                                    font-family: Satoshi, sans-serif;

                                    font-size: 48px;
                                    font-weight: 700;
                                    line-height: 72px;
                                }

                                .row-p3 {
                                    color: #cbd5e1;
                                    text-align: center;
                                    justify-content: center;
                                    align-items: center;
                                    width: 668px;
                                    margin-top: 24px;
                                    font-family: Inter, sans-serif;
                                    font-size: 18px;
                                    line-height: 28px;
                                }

                                .div-a {
                                    padding: 8px 16px;
                                    background-color: transparent;
                                    border-radius: 20px;
                                    margin: 5px;
                                    white-space: nowrap;
                                    font-weight: 500;
                                    cursor: pointer;
                                    text-align: center;
                                    transition: all 0.3s ease;
                                    flex-shrink: 0;
                                    border: 1px solid #ccc;
                                    color: #ffffff;
                                    /* default text color */
                                }

                                .div-a.selected {
                                    background-color: #ffffff;
                                    color: #0f172a;
                                    border-color: #f8fafc;
                                }

                                .scroll-container-tabs {
                                    overflow-x: auto;
                                    flex-wrap: nowrap;
                                    -webkit-overflow-scrolling: touch;
                                }

                                .scroll-container::-webkit-scrollbar {
                                    display: none;
                                }

                                @media (min-width: 768px) {
                                    .scroll-container-tabs {
                                        flex-wrap: wrap;
                                        overflow-x: visible;
                                        justify-content: center;
                                    }
                                }

                                .div-a.selected {
                                    background-color: #ffffff;
                                    color: #0f172a;
                                    border-color: #f8fafc;
                                }



                                .tab-content {
                                    display: none;
                                    /* Hide all sections by default */
                                    padding: 20px;
                                    background-color: transparent;
                                    border-radius: 10px;

                                }
                            </style>



                            <div class="d-flex scroll-container-tabs">
                                <div>
                                    <div class="div-a" id="trendingTab">🔥 Trending</div>
                                </div>
                                <div>
                                    <div class="div-a" id="allTab">All</div>
                                </div>
                                <div>
                                    <div class="div-a" id="techTab">Tech</div>
                                </div>
                                <div>
                                    <div class="div-a" id="careerTab">Career</div>
                                </div>
                                <div>
                                    <div class="div-a" id="cxoTab">CXO</div>
                                </div>
                                <div>
                                    <div class="div-a" id="productivityTab">Productivity</div>
                                </div>
                                <div>
                                    <div class="div-a" id="gsocTab">GSOC</div>
                                </div>
                                <div>
                                    <div class="div-a" id="panelTab">Panel</div>
                                </div>
                            </div>
                        </div>

                        <div class="tab-content" id="trendingContent">



                            <style>
                                body {
                                    font-family: 'Roboto', sans-serif;
                                    background-color: transparent;
                                }

                                .main-row-container {
                                    padding: 50px 15px;
                                }

                                /* Scroll container: flex row with horizontal scroll on small */
                                .scroll-container {
                                    display: flex;
                                    overflow-x: auto;
                                    gap: 80px;
                                    scroll-snap-type: x mandatory;
                                    -webkit-overflow-scrolling: touch;
                                    padding-bottom: 15px;
                                    /* to avoid cutting off cards */
                                }

                                .scroll-container::-webkit-scrollbar {
                                    display: none;
                                }

                                /* Card styling */
                                .card-wrapper-trending {
                                    border-radius: 30px;
                                    box-shadow: 0 4px 16px rgba(0, 0, 0, 0.2);
                                    overflow: hidden;
                                    background-color: transparent;
                                    flex: 0 0 90%;
                                    scroll-snap-align: start;
                                    margin-bottom: 30px;


                                    display: flex;
                                    flex-direction: column;
                                    justify-content: space-between;
                                }



                                @media (min-width: 768px) {
                                    .scroll-container {
                                        display: flex;
                                        overflow-x: visible;
                                        gap: 30px;
                                        scroll-snap-type: none;
                                        padding-bottom: 0;
                                    }

                                    .card-wrapper-trending {
                                        flex: 1;

                                        margin-bottom: 0;
                                    }

                                }

                                .bg-sandeep {
                                    position: relative;
                                    width: 100%;
                                    aspect-ratio: 16 / 9;
                                    overflow: hidden;
                                    cursor: pointer;
                                }

                                .bg-sandeep img.bg-image {
                                    position: absolute;
                                    top: 0;
                                    left: 0;
                                    height: 100%;
                                    width: 100%;
                                    object-fit: cover;
                                    z-index: 1;
                                }

                                .pulse-con {
                                    position: absolute;
                                    top: 75%;
                                    left: 7%;
                                    z-index: 2;
                                    display: flex;
                                    align-items: center;
                                    padding: 3px 10px;
                                    background-color: #60a5fa;
                                    color: white;
                                    font-size: 10px;
                                    border-radius: 45px;
                                    font-weight: bold;
                                    max-width: fit-content;
                                }

                                .pulse-wrapper {
                                    position: relative;
                                    width: 22px;
                                    height: 22px;
                                    margin-left: 12px;
                                }

                                .pulse-ring {
                                    position: absolute;
                                    top: 50%;
                                    left: 50%;
                                    width: 50%;
                                    height: 50%;
                                    border-radius: 50%;
                                    background-color: white;
                                    opacity: 0.5;
                                    transform: translate(-50%, -50%);
                                    animation: pulse-ring 2s infinite ease-out;
                                }


                                .pulse-ring:nth-child(2) {
                                    animation-delay: 0.4s;
                                }

                                .pulse-ring:nth-child(3) {
                                    animation-delay: 0.8s;
                                }

                                @keyframes pulse-ring {
                                    0% {
                                        transform: translate(-50%, -50%) scale(1);
                                        opacity: 0.5;
                                    }

                                    100% {
                                        transform: translate(-50%, -50%) scale(3.5);
                                        opacity: 0;
                                    }
                                }

                                .play-icon {
                                    position: absolute;
                                    top: 50%;
                                    left: 50%;
                                    transform: translate(-50%, -50%);
                                    width: 70%;
                                    height: 70%;
                                    background-color: white;
                                    border-radius: 50%;
                                    display: flex;
                                    justify-content: center;
                                    align-items: center;
                                    z-index: 2;
                                }

                                .play-img {
                                    width: 12px;
                                    height: 12px;
                                }

                                .modal-content {
                                    background-color: #000;
                                    border: none;
                                    border-radius: 12px;
                                    overflow: hidden;
                                }

                                .modal-header {
                                    border: none;
                                    justify-content: flex-end;
                                }

                                .modal-header .close {
                                    color: #fff;
                                    font-size: 2rem;
                                    opacity: 1;
                                }

                                .description-section {
                                    background-color: #1e293b;
                                    padding: 20px;
                                    flex-grow: 1;
                                }

                                .description-section h1 {
                                    font-size: 24px;
                                    font-weight: 700;
                                    color: #f8fafc;
                                }

                                .description-section .time {
                                    display: flex;
                                    align-items: center;
                                    color: #e2e8f0;
                                    font-size: 14px;
                                    margin: 10px 0;
                                }

                                .description-section h6 {
                                    color: #cbd5e1;
                                    font-size: 16px;
                                    font-weight: 700;
                                    margin-bottom: 4px;
                                }

                                .description-section p {
                                    color: #f8fafc;
                                    font-size: 14px;
                                }

                                @media (max-width: 768px) {
                                    .bg-sandeep {
                                        height: 60vh;
                                        flex-shrink: 0;
                                    }

                                    .pulse-con {
                                        font-size: 20px;
                                        padding: 6px 16px;
                                        top: 75%;
                                    }

                                    .pulse-wrapper {
                                        width: 38px;
                                        height: 38px;
                                    }

                                    .play-img {
                                        width: 20px;
                                        height: 24px;
                                    }

                                    .description-section h1 {
                                        font-size: 20px;
                                    }

                                    .description-section h6 {
                                        font-size: 14px;
                                    }

                                    .description-section p {
                                        font-size: 13px;
                                    }
                                }


                                .what-you-will-learn-bg {
                                    background-color: #1e293b;
                                }

                                .what-you-will-learn-h3 {
                                    color: #f1f5f9;
                                    font-family: Inter, sans-serif;
                                    font-size: 30px;
                                    font-weight: 600;
                                    line-height: 36px;
                                }



                                .what-you-will-learn-h6 {
                                    color: #f1f5f9;
                                    margin-bottom: 8px;
                                    font-family: Inter, sans-serif;
                                    font-size: 20px;
                                    font-weight: 700;
                                    line-height: 28px;
                                }

                                .what-you-will-learn-p1 {
                                    color: #e2e8f0;
                                    font-family: Inter, sans-serif;
                                    font-size: 16px;
                                    line-height: 24px;

                                }


                                .what-you-will-learn-p2 {
                                    color: #e2e8f0;
                                    width: 614px;
                                    margin-bottom: 24px;
                                    font-family: Inter, sans-serif;
                                    font-size: 16px;
                                    line-height: 24px;
                                }

                                .what-you-will-learn-Experience {
                                    color: #e2e8f0;
                                    margin-bottom: 16px;
                                    font-family: Inter, sans-serif;
                                    font-size: 16px;
                                    font-weight: 600;
                                    line-height: 24px;
                                }

                                .what-you-will-learn-list-heading {
                                    color: #f1f5f9;
                                    font-family: Inter, sans-serif;
                                    font-size: 30px;
                                    font-weight: 600;
                                    line-height: 36px;
                                }

                                .what-you-will-learn-list-items {
                                    color: #e2e8f0;
                                    margin-left: 16px;
                                    font-family: Inter, sans-serif;
                                    font-size: 18px;
                                    line-height: 28px;
                                }

                                #trendingContent {
                                    display: block;
                            </style>








                            <div class="container main-row-container" id="trendingContent">
                                <div class="scroll-container">


                                    <!-- Card 1 -->
                                    <div class="card-wrapper-trending">
                                        <div class="bg-sandeep" data-video="https://www.youtube.com/embed/YDfL0TfKS3M">
                                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/sandeep.png" class="bg-image" />
                                            <div class="pulse-con">
                                                Trailer
                                                <div class="pulse-wrapper">
                                                    <div class="pulse-ring"></div>
                                                    <div class="pulse-ring"></div>
                                                    <div class="pulse-ring"></div>
                                                    <div class="play-icon">
                                                        <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/64533d2ddcff965e7b00edbb_Vector.png" class="play-img" />
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="description-section">
                                            <h1>An Engineering Manager at Uber Teaches Programming</h1>
                                            <div class="time">
                                                <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" />
                                                <span class="pl-2">45:17 Mins</span>
                                            </div>
                                            <h6>Sandeep Gorthi</h6>
                                            <p>Engineering Manager at Uber</p>
                                            <a href="#" data-toggle="modal" data-target="#sandeepModal">
                                                What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                            </a>
                                        </div>
                                    </div>

                                    <!-- Card 2 -->
                                    <div class="card-wrapper-trending">
                                        <div class="bg-sandeep" data-video="https://www.youtube.com/embed/pDpwlapFss8">
                                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/pritesh.png" class="bg-image" />
                                            <div class="pulse-con">
                                                Trailer
                                                <div class="pulse-wrapper">
                                                    <div class="pulse-ring"></div>
                                                    <div class="pulse-ring"></div>
                                                    <div class="pulse-ring"></div>
                                                    <div class="play-icon">
                                                        <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/64533d2ddcff965e7b00edbb_Vector.png" class="play-img" />
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="description-section">
                                            <h1>A Sr. Recruiter at Amazon Teaches Acing Interviews</h1>
                                            <div class="time">
                                                <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" />
                                                <span class="pl-2">41.07 Mins</span>
                                            </div>
                                            <h6>Pritesh Malode</h6>
                                            <p>Senior Recruiter at Amazon</p>
                                            <a href="#" data-toggle="modal" data-target="#priteshModal">
                                                What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                            </a>
                                        </div>
                                    </div>

                                    <!-- Card 3 -->
                                    <div class="card-wrapper-trending">
                                        <div class="bg-sandeep" data-video="https://www.youtube.com/embed/BKe0tIy4u0k">
                                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/sanjay.png" class="bg-image" />
                                            <div class="pulse-con">
                                                Trailer
                                                <div class="pulse-wrapper">
                                                    <div class="pulse-ring"></div>
                                                    <div class="pulse-ring"></div>
                                                    <div class="pulse-ring"></div>
                                                    <div class="play-icon">
                                                        <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/64533d2ddcff965e7b00edbb_Vector.png" class="play-img" />
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="description-section">
                                            <h1>A Global CEO Teaches Mastering Time Management</h1>
                                            <div class="time">
                                                <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" />
                                                <span class="pl-2">56:32 Mins</span>
                                            </div>
                                            <h6>Sanjay Sehgal</h6>
                                            <p>Chairman & CEO at Msys Technologies</p>
                                            <a href="#" data-toggle="modal" data-target="#sanjayModal">
                                                What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                            </a>
                                        </div>
                                    </div>

                                </div>
                            </div>





                        </div>









                        <div class="tab-content" id="allContent">
                            <style>
                                body {
                                    font-family: 'Roboto', sans-serif;
                                    background-color: #f1f5f9;
                                    margin: 0;
                                    padding: 20px;
                                }

                                .slider-container {
                                    position: relative;
                                    max-width: 1000px;
                                    margin: auto;
                                    overflow: hidden;
                                    /* hide overflow so no partial cards show */

                                    border-radius: 20px;

                                    background-color: transparent;
                                }

                                .cards-wrapper {
                                    display: flex;
                                    gap: 30px;
                                    transition: transform 0.4s ease;
                                    will-change: transform;

                                }

                                .card-wrapper {
                                    background-color: #fff;
                                    border-radius: 16px;
                                    box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15);
                                    flex-shrink: 0;
                                    /* control width with media queries */
                                    display: flex;
                                    flex-direction: column;
                                    justify-content: space-between;
                                    overflow: hidden;
                                }

                                /* Card width - 3 cards exactly fit container */
                                @media (min-width: 768px) {
                                    .card-wrapper {
                                        width: calc((100% - 40px) / 3);
                                        /* 20px gap * 2 = 40px total gap */
                                    }
                                }

                                /* Mobile: show ~1.5 cards with scroll */
                                @media (max-width: 767px) {
                                    .cards-wrapper {
                                        overflow-x: auto;
                                        scroll-snap-type: x mandatory;
                                        -webkit-overflow-scrolling: touch;
                                        scrollbar-width: none;
                                        gap: 65px;
                                        padding-bottom: 10px;
                                        padding-top: 10px;
                                        background-color: transparent;
                                    }

                                    .cards-wrapper: :-webkit-scrollbar {
                                        display: none;
                                        /* Chrome, Safari */
                                    }

                                    .card-wrapper {
                                        width: 70vw;
                                        scroll-snap-align: center;
                                        margin: 0 5px;
                                    }

                                    .track-button {
                                        display: none !important;
                                    }


                                }





                                /* Image section */
                                .img-section {
                                    position: relative;
                                    width: 100%;
                                    aspect-ratio: 16 / 9;
                                    overflow: hidden;
                                }

                                .img-section img {
                                    width: 100%;
                                    height: 100%;
                                    object-fit: cover;
                                    display: block;
                                }

                                /* Description section exactly as you gave */
                                .description-section {
                                    background-color: #1e293b;
                                    padding: 20px;
                                    flex-grow: 1;
                                    color: #f8fafc;
                                    display: flex;
                                    flex-direction: column;
                                    justify-content: space-between;
                                }

                                .description-section h1 {
                                    font-size: 24px;
                                    font-weight: 700;
                                    margin: 0 0 10px;
                                }

                                .description-section .time {
                                    display: flex;
                                    align-items: center;
                                    color: #e2e8f0;
                                    font-size: 14px;
                                    margin: 10px 0;
                                }

                                .description-section h6 {
                                    color: #cbd5e1;
                                    font-size: 16px;
                                    font-weight: 700;
                                    margin: 0 0 4px;
                                }

                                .description-section p {
                                    font-size: 14px;
                                    margin: 0 0 10px;
                                }

                                .description-section a {
                                    color: #60a5fa;
                                    font-weight: 600;
                                    text-decoration: none;
                                    align-self: flex-start;
                                    display: inline-flex;
                                    align-items: center;
                                }

                                .description-section a img {
                                    margin-left: 5px;
                                    width: 12px;
                                    height: 12px;
                                }



                                .track-button {
                                    background-color: #334155;
                                    border-radius: 25px;
                                    justify-content: center;
                                    align-items: center;
                                    width: 50px;
                                    height: 50px;
                                    display: flex;
                                    cursor: pointer;
                                    flex-shrink: 0;
                                }



                                .slider-nav-wrapper {
                                    display: flex;
                                    align-items: center;
                                    justify-content: center;
                                    gap: 20px;
                                    /* Gap between arrows and slider */
                                    padding: 0 10px;
                                    width: 100%;
                                    margin-top: 20px;
                                }
                            </style>

                            <div class="slider-nav-wrapper d-flex align-items-center justify-content-center ">

                                <!-- Left Arrow -->
                                <div class="track-button " id="leftBtnAll">
                                    <img loading="lazy" src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c402ed682553d6_Icon.svg" alt="Left Arrow">
                                </div>



                                <div class="slider-container">








                                    <div class="cards-wrapper" id="cardsWrapperAll">










                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c65ced331713c1b1b2dc_irshad-thumbnail.webp" class="bg-image" alt="Background" />

                                            </div>

                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1> Learn the fundamentals of AWS from an Expert</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:00:55 mins</span>
                                                </div>
                                                <h6>Irshad Chohan</h6>
                                                <p>Senior Solutions Architect at AWS</p>
                                                <a href="#" data-toggle="modal" data-target="#irshadModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>








                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c9ef1acc87ac5abbaa62_sriram-thumbnail.webp" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1> What happens at Samsung Electronics Headquarters South Korea</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">49:26 mins</span>
                                                </div>
                                                <h6>Sriram Varun Vobilisetty</h6>
                                                <p>Product Manager at ALLEN Digital</p>
                                                <a href="#" data-toggle="modal" data-target="#varunModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>
                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c3b977eb17ab2fe49ddb_krishna-raghavan-thumbnail.webp" class="bg-image" alt="Background" />

                                            </div>



                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1> Discover what the Top 1% Professionals do differently</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">41:23 mins</span>
                                                </div>
                                                <h6>Krishna Raghavan</h6>
                                                <p>People and Tech Leader</p>
                                                <a href="#" data-toggle="modal" data-target="#KrishnaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>


                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690bf2c4727b379bef9754b_ankur-thumbnail.webp" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Senior Data Scientist teaches you about building a Career in AI </h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">47:47 mins</span>
                                                </div>
                                                <h6>Ankur Debnath</h6>
                                                <p>Senior Data Scientist at S and P Global</p>
                                                <a href="#" data-toggle="modal" data-target="#AnkurModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>





                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b7c2dc4fade04120f946_tezan-thumbnail.webp" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Find out How to become a Data Scientist</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:06:34 mins</span>
                                                </div>
                                                <h6>Tezan Sahu</h6>
                                                <p>Bing Autosuggest expert</p>
                                                <a href="#" data-toggle="modal" data-target="#TezanModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b14ce49b9ed3c0a7499c_sandeep-chandra-thumbnail.webp" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Product Management from a Microsoft Expert</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:01:43 mins</span>
                                                </div>
                                                <h6>Sandeep Chadda</h6>
                                                <p>Product Manager at Microsoft</p>
                                                <a href="#" data-toggle="modal" data-target="#ChaddaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690abec51e34cbc9072482b_Johan-thumbinail.webp" class="bg-image" alt="Background" />

                                            </div>

                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Learn Internet of Things from a Global Expert</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">36:55 mins</span>
                                                </div>
                                                <h6>Johan Stokking</h6>
                                                <p>CTO & Co-Founder of The Things Industries</p>
                                                <a href="#" data-toggle="modal" data-target="#JohanModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>










                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/shyama.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Machine Learning Engineer at Liftoff Teaches Data Science</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">46:57 Mins</span>
                                                </div>
                                                <h6>Shyama Dorbala</h6>
                                                <p>ML Engineer at Liftoff Mobiles</p>
                                                <a href="#" data-toggle="modal" data-target="#ShyamaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>








                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/rahul-garg.png" class="bg-image" alt="Background" />

                                            </div>
                                            <div class="description-section">
                                                <h1>GSOC Alumuni Teaches You About Cracking GSOC</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">46 Mins</span>
                                                </div>
                                                <h6>Rahul Garg</h6>
                                                <p>IIIT Hyderabad, GSOC Alumnus</p>
                                                <a href="#" data-toggle="modal" data-target="#RahulModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>



                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/sivay-lamba.png" class="bg-image" alt="Background" />

                                            </div>


                                            <div class="description-section">
                                                <h1>GSOC Alumuni Teaches You About Cracking GSOC</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">47 Mins</span>
                                                </div>
                                                <h6>Mr. Shivay Lamba</h6>
                                                <p>CTO, DarkHorse</p>
                                                <a href="#" data-toggle="modal" data-target="#ShivayModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/nirmal-manoj.png" class="bg-image" alt="Background" />

                                            </div>




                                            <div class="description-section">
                                                <h1>GSOC Alumuni Teaches You About the GSOC Process</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">46 Mins</span>
                                                </div>
                                                <h6>Nirmal Manoj</h6>
                                                <p>IIIT Hyderabad, GSOC Alumnus</p>
                                                <a href="#" data-toggle="modal" data-target="#NirmalModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>



                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/nikhil.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Software Engineer at Uber Teaches You About Coding</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">14:18 Mins</span>
                                                </div>
                                                <h6>Nikhil VAVS</h6>
                                                <p>Software Engineer at Uber</p>
                                                <a href="#" data-toggle="modal" data-target="#NikhilModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/priyatham-bollimpalli.png" class="bg-image" alt="Background" />

                                            </div>



                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Data Scientist at Microsoft Teaches you About Data Science</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:07:43 Mins</span>
                                                </div>
                                                <h6>Priyatham Bollimpalli</h6>
                                                <p>Data & Applied Scientist II at Microsoft</p>
                                                <a href="#" data-toggle="modal" data-target="#PriyathamModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/shri-dana-kishor.png" class="bg-image" alt="Background" />

                                            </div>



                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>An IAS Officer Teaches You About Impact Making</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:30:56 Mins</span>
                                                </div>
                                                <h6>Shri Dhana Kishore</h6>
                                                <p>IAS, MD - HMWSSB</p>
                                                <a href="#" data-toggle="modal" data-target="#KishoreModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/hari-tn.png" class="bg-image" alt="Background" />

                                            </div>



                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>The HR Head of Big Basket Teaches You About Building a Career</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">43:19 Mins</span>
                                                </div>
                                                <h6>Hari TN</h6>
                                                <p>Head HR, Big Basket</p>
                                                <a href="#" data-toggle="modal" data-target="#HariModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>





                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/girish-akash.png" class="bg-image" alt="Background" />

                                            </div>



                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Placement Head at NxtWave Teaches You About Paid Internships</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:06:05 Mins</span>
                                                </div>
                                                <h6>Girish Akash Yeswanth</h6>
                                                <p>VP of Corporate Relations at NxtWave </p>
                                                <a href="#" data-toggle="modal" data-target="#GirishModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>
                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/ram-ganesh.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>The CEO of Cyber Eye Teaches You About Cyber Security</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">41:34 Mins</span>
                                                </div>
                                                <h6>Ram Ganesh</h6>
                                                <p>CEO of CyberEye </p>
                                                <a href="#" data-toggle="modal" data-target="#RamModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>



                                        </div>


                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/trivikrama-kothinti-2.png" class="bg-image" alt="Background" />

                                            </div>



                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>An AI/ML Expert Teaches You About Advanced Technologies</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">41:34 Mins</span>
                                                </div>
                                                <h6>Trivikrama Kothinti</h6>
                                                <p>AI/ML Expert, Alumus of IIT Delhi </p>
                                                <a href="#" data-toggle="modal" data-target="#TrivikramaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>





                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/rakesh-mishra.png" class="bg-image" alt="Background" />

                                            </div>



                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>The Co-founder of Uhana Teaches You About 5G</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">48:49 Mins</span>
                                                </div>
                                                <h6>Rakesh Mishra</h6>
                                                <p>Co-founder of Uhana (Acquired by VMware), PhD at Stanford University </p>
                                                <a href="#" data-toggle="modal" data-target="#RakeshModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>



                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/deepa-wadhwani.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>HR Lead of ADP Teaches Mastering Interviews</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">31:09 Mins</span>
                                                </div>
                                                <h6>Deepa Wadhwani</h6>
                                                <p>Director - Lead Acquisition of ADP </p>
                                                <a href="#" data-toggle="modal" data-target="#DeepaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>


                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/naveen.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Lead at SuperK Teaches Career Designing</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">58:58 Mins</span>
                                                </div>
                                                <h6>Naveen Thontepu</h6>
                                                <p>Head of Engineering at SuperK </p>
                                                <a href="#" data-toggle="modal" data-target="#NaveenModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>



                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/giridhar.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Research Engineer at IBM Teaches Building Coding Skills</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">45:48 Mins</span>
                                                </div>
                                                <h6>Giridhar Ganapavarapu</h6>
                                                <p>Research Engineer, IBM New York</p>
                                                <a href="#" data-toggle="modal" data-target="#GiridharModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>










                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/shiva-kumar.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Chief Technology Officer at Slice Teaches Leadership</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">01:06:52 Mins</span>
                                                </div>
                                                <h6>Shiva Kumar</h6>
                                                <p>Chief Technology Officer at Slice</p>
                                                <a href="#" data-toggle="modal" data-target="#ShivaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>







                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/sanjay.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Global CEO Teaches Mastering Time Management</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">56:32 Mins</span>
                                                </div>
                                                <h6>Sanjay Sehgal</h6>
                                                <p>Chairman & CEO at Msys Technologies</p>
                                                <a href="#" data-toggle="modal" data-target="#sanjayModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>










                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/sandeep.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>An Engineering Manager at Uber Teaches Programming</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">45:17 Mins</span>
                                                </div>
                                                <h6>Sandeep Gorthi</h6>
                                                <p>Engineering Manager at Uber</p>
                                                <a href="#" data-toggle="modal" data-target="#sandeepModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/architha-nagelli.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Lead Engineer at Meesho Busts Popular Coding Myths</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">35:04 Mins</span>
                                                </div>
                                                <h6>Architha Nagelli</h6>
                                                <p>Lead Software Engineer, Meesho</p>
                                                <a href="#" data-toggle="modal" data-target="#ArchithaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>







                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/panel-2.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>MAANG Experts Teach You About Securing Dream Jobs</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:00:11 Mins</span>
                                                </div>
                                                <h6>Expert Panel</h6>

                                                <a href="#" data-toggle="modal" data-target="#MAANGModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>






                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/panel-1.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>HR Leaders Teach
                                                    You About Acing Interviews</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:09:54 Mins</span>
                                                </div>
                                                <h6>Expert Panel</h6>

                                                <a href="#" data-toggle="modal" data-target="#HRModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>





                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/panel-3.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Expert Engineers Teach You About 4.0 Technologies</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:00:11 Mins</span>
                                                </div>
                                                <h6>Expert Panel</h6>

                                                <a href="#" data-toggle="modal" data-target="#ExpertModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>



                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/pritesh.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Sr. Recruiter at Amazon Teaches You about Acing Interviews</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">41.07 Mins</span>
                                                </div>
                                                <h6>Pritesh Malode</h6>
                                                <p>Senior Recruiter at Amazon</p>
                                                <a href="#" data-toggle="modal" data-target="#priteshModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/govind-goyal.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>GSOC Mentor Teaches You About Acing GSOC Applications</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">47 Mins</span>
                                                </div>
                                                <h6>Govind Goyal</h6>
                                                <p>2x GSOC Mentor</p>
                                                <a href="#" data-toggle="modal" data-target="#GovindModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>





                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/goutam.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>An Engineer at Meta Teaches You About Designing Technology</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">50:46 Mins
                                                    </span>
                                                </div>
                                                <h6>Goutam Reddy</h6>
                                                <p>Platform Security Engineer Meta USA</p>
                                                <a href="#" data-toggle="modal" data-target="#GoutamModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>






                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/ashok-vardhan.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Software Engineer at Google Teaches Google Mindset</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:23:53 Mins
                                                    </span>
                                                </div>
                                                <h6>Ashok Vardhan Viswanadha</h6>
                                                <p>Staff Software Engineer at Google</p>
                                                <a href="#" data-toggle="modal" data-target="#AshokModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>





                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/sri-vidhya.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Scientist at Apple Teaches You About Machine Learning</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">41:27 Mins
                                                    </span>
                                                </div>
                                                <h6>Sri Vidya Pranavi</h6>
                                                <p>Machine Learning Scientist at Apple</p>
                                                <a href="#" data-toggle="modal" data-target="#PranaviModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/kiran.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>An Engineer at Google Teaches Thriving in Tech & Life</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">54:27 Mins
                                                    </span>
                                                </div>
                                                <h6>Sai Kiran Gorthi</h6>
                                                <p>Software Engineer at Google</p>
                                                <a href="#" data-toggle="modal" data-target="#SaiModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>





                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/abhinav.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Software Engineer at Twitter Teaches Coder's Mindset</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">

                                                        50:36 Mins

                                                    </span>
                                                </div>
                                                <h6>Abhinav Reddy</h6>
                                                <p>Software Development Engineer, Twitter</p>
                                                <a href="#" data-toggle="modal" data-target="#AbhinavModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>






                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/siva-ghani-reddy.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Sr. Manager at Microsoft Teaches Product Management</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">
                                                        01:01:13 Mins

                                                    </span>
                                                </div>
                                                <h6>Siva Ghani Reddy</h6>
                                                <p>Senior Product Manager at Microsoft</p>
                                                <a href="#" data-toggle="modal" data-target="#SivaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>












                                    </div>


                                </div>





                                <!-- Right Arrow -->
                                <div class="track-button" id="rightBtnAll">
                                    <img loading="lazy" src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c402b55d25544e_cheveron-left.png" alt="Right Arrow">
                                </div>

                            </div>


                        </div>


                        <div class="tab-content" id="techContent">
                            <div class="slider-nav-wrapper d-flex align-items-center justify-content-center">

                                <!-- Left Arrow -->
                                <div class="track-button " id="leftBtnTech">
                                    <img loading="lazy" src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c402ed682553d6_Icon.svg" alt="Left Arrow">
                                </div>



                                <div class="slider-container">








                                    <div class="cards-wrapper" id="cardsWrapperTech">







                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690bf2c4727b379bef9754b_ankur-thumbnail.webp" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Senior Data Scientist teaches you about building a Career in AI </h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">47:47 mins</span>
                                                </div>
                                                <h6>Ankur Debnath</h6>
                                                <p>Senior Data Scientist at S and P Global</p>
                                                <a href="#" data-toggle="modal" data-target="#AnkurModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>





                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b7c2dc4fade04120f946_tezan-thumbnail.webp" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Find out How to become a Data Scientist</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:06:34 mins</span>
                                                </div>
                                                <h6>Tezan Sahu</h6>
                                                <p>Bing Autosuggest expert</p>
                                                <a href="#" data-toggle="modal" data-target="#TezanModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b14ce49b9ed3c0a7499c_sandeep-chandra-thumbnail.webp" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Product Management from a Microsoft Expert</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:01:43 mins</span>
                                                </div>
                                                <h6>Sandeep Chadda</h6>
                                                <p>Product Manager at Microsoft</p>
                                                <a href="#" data-toggle="modal" data-target="#ChaddaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690abec51e34cbc9072482b_Johan-thumbinail.webp" class="bg-image" alt="Background" />

                                            </div>

                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Learn Internet of Things from a Global Expert</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">36:55 mins</span>
                                                </div>
                                                <h6>Johan Stokking</h6>
                                                <p>CTO & Co-Founder of The Things Industries</p>
                                                <a href="#" data-toggle="modal" data-target="#JohanModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>










                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/shyama.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Machine Learning Engineer at Liftoff Teaches Data Science</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">46:57 Mins</span>
                                                </div>
                                                <h6>Shyama Dorbala</h6>
                                                <p>ML Engineer at Liftoff Mobiles</p>
                                                <a href="#" data-toggle="modal" data-target="#ShyamaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>





















                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/nikhil.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Software Engineer at Uber Teaches You About Coding</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">14:18 Mins</span>
                                                </div>
                                                <h6>Nikhil VAVS</h6>
                                                <p>Software Engineer at Uber</p>
                                                <a href="#" data-toggle="modal" data-target="#NikhilModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/priyatham-bollimpalli.png" class="bg-image" alt="Background" />

                                            </div>



                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Data Scientist at Microsoft Teaches you About Data Science</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:07:43 Mins</span>
                                                </div>
                                                <h6>Priyatham Bollimpalli</h6>
                                                <p>Data & Applied Scientist II at Microsoft</p>
                                                <a href="#" data-toggle="modal" data-target="#PriyathamModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>


                                        </div>





























                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/naveen.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Lead at SuperK Teaches Career Designing</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">58:58 Mins</span>
                                                </div>
                                                <h6>Naveen Thontepu</h6>
                                                <p>Head of Engineering at SuperK </p>
                                                <a href="#" data-toggle="modal" data-target="#NaveenModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>



                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/giridhar.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Research Engineer at IBM Teaches Building Coding Skills</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">45:48 Mins</span>
                                                </div>
                                                <h6>Giridhar Ganapavarapu</h6>
                                                <p>Research Engineer, IBM New York</p>
                                                <a href="#" data-toggle="modal" data-target="#GiridharModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>





























                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/sandeep.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>An Engineering Manager at Uber Teaches Programming</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">45:17 Mins</span>
                                                </div>
                                                <h6>Sandeep Gorthi</h6>
                                                <p>Engineering Manager at Uber</p>
                                                <a href="#" data-toggle="modal" data-target="#sandeepModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/architha-nagelli.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Lead Engineer at Meesho Busts Popular Coding Myths</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">35:04 Mins</span>
                                                </div>
                                                <h6>Architha Nagelli</h6>
                                                <p>Lead Software Engineer, Meesho</p>
                                                <a href="#" data-toggle="modal" data-target="#ArchithaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>


































                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/goutam.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>An Engineer at Meta Teaches You About Designing Technology</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">50:46 Mins
                                                    </span>
                                                </div>
                                                <h6>Goutam Reddy</h6>
                                                <p>Platform Security Engineer Meta USA</p>
                                                <a href="#" data-toggle="modal" data-target="#GoutamModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>






                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/ashok-vardhan.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Software Engineer at Google Teaches Google Mindset</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:23:53 Mins
                                                    </span>
                                                </div>
                                                <h6>Ashok Vardhan Viswanadha</h6>
                                                <p>Staff Software Engineer at Google</p>
                                                <a href="#" data-toggle="modal" data-target="#AshokModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>
























                                    </div>
                                </div>



                                <!-- Right Arrow -->
                                <div class="track-button" id="rightBtnTech">
                                    <img loading="lazy" src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c402b55d25544e_cheveron-left.png" alt="Right Arrow">
                                </div>

                            </div>
                        </div>


                        <div class="tab-content" id="careerContent">
                            <div class="slider-nav-wrapper d-flex align-items-center justify-content-center">

                                <!-- Left Arrow -->
                                <div class="track-button" id="leftBtnCareer">
                                    <img loading="lazy" src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c402ed682553d6_Icon.svg" alt="Left Arrow">
                                </div>



                                <div class="slider-container">








                                    <div class="cards-wrapper" id="cardsWrapperCareer">




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/pritesh.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Sr. Recruiter at Amazon Teaches You about Acing Interviews</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">41.07 Mins</span>
                                                </div>
                                                <h6>Pritesh Malode</h6>
                                                <p>Senior Recruiter at Amazon</p>
                                                <a href="#" data-toggle="modal" data-target="#priteshModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>









                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/girish-akash-2.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Placement Head at NxtWave Teaches You About Internships</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:30:56 Mins</span>
                                                </div>
                                                <h6>Girish Akash Yeswanth</h6>
                                                <p>VP of Corporate Relations at NxtWave </p>
                                                <a href="#" data-toggle="modal" data-target="#GirishModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>


























                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/trivikrama-kothinti.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>An AI/ML Expert Teaches You About Building ML Models</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:36:33 Mins</span>
                                                </div>
                                                <h6>Trivikrama Kothinti</h6>
                                                <p>AI/ML Expert, Alumnus of IIT Delhi
                                                    (AIR 93) </p>
                                                <a href="#" data-toggle="modal" data-target="#TrivikramaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>







                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/naveen.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Lead at SuperK Teaches Career Designing</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">58:58 Mins</span>
                                                </div>
                                                <h6>Naveen Thontepu</h6>
                                                <p>Head of Engineering at SuperK </p>
                                                <a href="#" data-toggle="modal" data-target="#NaveenModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>









                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/shashank.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Co-Founder of Nxtwave Teaches Elevating Presentations</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:36:33 Mins</span>
                                                </div>
                                                <h6>Shashank Gujjala</h6>
                                                <p>Co-Founder Nxtwave , IIT Bombay </p>
                                                <a href="#" data-toggle="modal" data-target="#ShashankModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>










                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/sri-vidhya.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Scientist at Apple Teaches You About Machine Learning</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">41:27 Mins</span>
                                                </div>
                                                <h6>Sri Vidya Pranavi</h6>
                                                <p>Machine Learning Scientist at Apple </p>
                                                <a href="#" data-toggle="modal" data-target="#PranaviModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>









                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/kalmeshwar.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>The DCP of Cyberabad Teaches Building Cyber-Safe Cities</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">35 :10 Mins</span>
                                                </div>
                                                <h6>Shri Kalmeshwar Shingenavar</h6>
                                                <p>DCP of Cyberabad, IPS </p>
                                                <a href="#" data-toggle="modal" data-target="#KalmeshwarModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>
















                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/shri-dana-kishor.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>An IAS Officer Teaches You About Impact Making</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:30:56 Mins</span>
                                                </div>
                                                <h6>Shri Dhana Kishore</h6>
                                                <p>IAS, MD - HMWSSB</p>
                                                <a href="#" data-toggle="modal" data-target="#KishoreModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>










                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/siva-ghani-reddy.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Sr. Manager at Microsoft Teaches Product Management</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">01:01:13 Mins</span>
                                                </div>
                                                <h6>Siva Ghani Reddy</h6>
                                                <p>Senior Product Manager at Microsoft</p>
                                                <a href="#" data-toggle="modal" data-target="#SivaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>





                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/hari-tn.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>The HR Head of Big Basket Teaches You About Building a Career</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">43:19 Mins</span>
                                                </div>
                                                <h6>Hari TN</h6>
                                                <p>Head HR, Big Basket</p>
                                                <a href="#" data-toggle="modal" data-target="#HariModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>








                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/deepa-wadhwani.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>HR Lead of ADP Teaches Mastering Interviews</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">31:09 Mins</span>
                                                </div>
                                                <h6>Deepa Wadhwani</h6>
                                                <p>Director - Lead Acquisition of ADP</p>
                                                <a href="#" data-toggle="modal" data-target="#DeepaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>



                                    </div>
                                </div>



                                <!-- Right Arrow -->
                                <div class="track-button" id="rightBtnCareer">
                                    <img loading="lazy" src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c402b55d25544e_cheveron-left.png" alt="Right Arrow">
                                </div>

                            </div>
                        </div>



                        <div class="tab-content" id="cxoContent">
                            <div class="slider-nav-wrapper d-flex align-items-center justify-content-center">

                                <!-- Left Arrow -->
                                <div class="track-button " id="leftBtnCxo">
                                    <img loading="lazy" src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c402ed682553d6_Icon.svg" alt="Left Arrow">
                                </div>



                                <div class="slider-container">








                                    <div class="cards-wrapper" id="cardsWrapperCxo">





                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/shiva-kumar.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Chief Technology Officer at Slice Teaches Leadership</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">01:06:52 Mins</span>
                                                </div>
                                                <h6>Shiva Kumar</h6>
                                                <p>Chief Technology Officer at Slice</p>
                                                <a href="#" data-toggle="modal" data-target="#ShivaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>








                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/sanjay-sehgal.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A CEO at Msys Teaches Innovation & Entrepreneurship</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">49:07 Mins</span>
                                                </div>
                                                <h6>Sanjay Sehgal</h6>
                                                <p>Chairman & CEO at Msys Technologies</p>
                                                <a href="#" data-toggle="modal" data-target="#sanjayModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>







                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/rakesh-mishra.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>The Co-founder of Uhana Teaches You About 5G</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">48:49 Mins</span>
                                                </div>
                                                <h6>Rakesh Mishra</h6>
                                                <p>Co-founder of Uhana (Acquired by VMware), PhD at Stanford University</p>
                                                <a href="#" data-toggle="modal" data-target="#RakeshModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>









                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/ram-ganesh.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>The CEO of Cyber Eye Teaches You About Cyber Security</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">41:34 Mins</span>
                                                </div>
                                                <h6>Ram Ganesh</h6>
                                                <p>CEO of CyberEye</p>
                                                <a href="#" data-toggle="modal" data-target="#RamModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>



                                    </div>
                                </div>



                                <!-- Right Arrow -->
                                <div class="track-button" id="rightBtnCxo">
                                    <img loading="lazy" src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c402b55d25544e_cheveron-left.png" alt="Right Arrow">
                                </div>

                            </div>
                        </div>




                        <div class="tab-content" id="productivityContent">
                            <div class="slider-nav-wrapper d-flex align-items-center justify-content-center">



                                <div class="slider-container">




                                    <div class="cards-wrapper" id="cardsWrapperProductivity">









                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/kiran.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>An Engineer at Google Teaches Thriving in Tech & Life</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">54:27 Mins</span>
                                                </div>
                                                <h6>Sai Kiran Gorthi</h6>
                                                <p>Software Engineer at Google</p>
                                                <a href="#" data-toggle="modal" data-target="#SaiModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>





















                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/sanjay.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>A Global CEO Teaches Mastering Time Management</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">56:32 Mins</span>
                                                </div>
                                                <h6>Sanjay Sehgal</h6>
                                                <p>Chairman & CEO at Msys Technologies</p>
                                                <a href="#" data-toggle="modal" data-target="#sanjayModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>








                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c3b977eb17ab2fe49ddb_krishna-raghavan-thumbnail.webp" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Discover what the Top 1% Professionals do differently</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">41:23 mins</span>
                                                </div>
                                                <h6>Krishna Raghavan</h6>
                                                <p>People and Tech Leader</p>
                                                <a href="#" data-toggle="modal" data-target="#KrishnaModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>













                                    </div>
                                </div>




                            </div>
                        </div>


                        <div class="tab-content" id="gsocContent">
                            <div id="gsocContent" class="slider-nav-wrapper d-flex align-items-center justify-content-center">

                                <!-- Left Arrow -->
                                <div class="track-button " id="leftBtnGsoc">
                                    <img loading="lazy" src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c402ed682553d6_Icon.svg" alt="Left Arrow">
                                </div>



                                <div class="slider-container">








                                    <div class="cards-wrapper" id="cardsWrapperGsoc">






                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/nirmal-manoj.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>GSOC Alumuni teaches You About the GSOC Process</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">46 Mins</span>
                                                </div>
                                                <h6>Nirmal Manoj</h6>
                                                <p>IIIT Hyderabad, GSOC Alumnus</p>
                                                <a href="#" data-toggle="modal" data-target="#NirmalModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>


                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/rahul-garg.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>GSOC Alumuni Teaches You About Cracking GSOC</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">46 Mins</span>
                                                </div>
                                                <h6>Rahul Garg</h6>
                                                <p>IIIT Hyderabad, GSOC Alumnus</p>
                                                <a href="#" data-toggle="modal" data-target="#RahulModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>









                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/sivay-lamba.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>GSOC Mentor Teaches You About Success Strategies for GSOC</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">47 Mins</span>
                                                </div>
                                                <h6>Mr. Shivay Lamba</h6>
                                                <p>CTO, DarkHorse</p>
                                                <a href="#" data-toggle="modal" data-target="#ShivayModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>






                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/govind-goyal.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>GSOC Mentor Teaches You About Acing GSOC Applications</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">47 Mins</span>
                                                </div>
                                                <h6>Govind Goyal</h6>
                                                <p>2x GSOC Mentor</p>
                                                <a href="#" data-toggle="modal" data-target="#GovindModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>

                                    </div>
                                </div>



                                <!-- Right Arrow -->
                                <div class="track-button" id="rightBtnGsoc">
                                    <img loading="lazy" src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c402b55d25544e_cheveron-left.png" alt="Right Arrow">
                                </div>

                            </div>
                        </div>



                        <div class="tab-content" id="panelContent">
                            <div class="slider-nav-wrapper d-flex align-items-center justify-content-center">





                                <div class="slider-container">








                                    <div class="cards-wrapper" id="cardsWrapperPanel">




                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/panel-3.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>Expert Engineers Teach You About 4.0 Technologies</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:00:11 Mins</span>
                                                </div>
                                                <h6 class="mb-5">Expert Panel</h6>

                                                <a href="#" data-toggle="modal" data-target="#ExpertModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>

















                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/panel-1.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>HR Leaders Teach
                                                    You About Acing Interviews</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:09:54 Mins</span>
                                                </div>
                                                <h6 class="mb-5">Expert Panel</h6>

                                                <a href="#" data-toggle="modal" data-target="#HRModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>


































                                        <div class="card-wrapper">

                                            <!-- Background Image + Button -->
                                            <div class="img-section">
                                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/panel-2.png" class="bg-image" alt="Background" />

                                            </div>


                                            <!-- Description Section -->
                                            <div class="description-section">
                                                <h1>MAANG Experts Teach You About Securing Dream Jobs</h1>
                                                <div class="time">
                                                    <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4027fbd255446_clock.png" alt="Clock" />
                                                    <span class="pl-2">1:00:11 Mins</span>
                                                </div>
                                                <h6 class="mb-5">Expert Panel</h6>

                                                <a href="#" data-toggle="modal" data-target="#MAANGModal">
                                                    What You will Learn <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/642c0b2b12c4022b3a2553d7_arrow-right.svg" alt="Arrow" />
                                                </a>
                                            </div>

                                        </div>

                                    </div>
                                </div>





                            </div>
                        </div>

                    </div>

                    <div class="d-flex flex-column justify-content-center text-center ">



                        <div>
                            <a href="#claim-your-free-access-section1"> <button class="vertical-slider-btn1 d-none d-md-block">Claim Free Access</button></a>
                        </div>
                        <div>
                            <p class="vertical-slider-p">Get 1 Podcast worth ₹2000


                                <img class="vector-img" src="https://uploads-ssl.webflow.com/64362e90abbff481a6d25ce8/64362e90abbff450f5d25f9f_Vector%201.png" alt="Free icon" />

                                <span class="vertical-slider-span2">Free</span>
                            </p>
                        </div>

                    </div>





                </div>

            </div>





            <div class="col-12  order-4 student-feedback-slider-parent-container ">
                <style>
                    .student-feedback-slider-parent-container {
                        color: #f1f5f9;
                        white-space: normal;
                        -webkit-text-fill-color: inherit;
                        cursor: auto;
                        mix-blend-mode: normal;
                        background-color: #0f172a;
                        background-clip: border-box;
                        flex-direction: column;
                        align-items: center;
                        max-width: 1200px;
                        margin-bottom: 0;
                        padding-top: 96px;
                        padding-bottom: 96px;
                        font-family: Inter, sans-serif;
                        font-size: 48px;
                        line-height: 72px;


                    }

                    .student-feedback-section-heading {
                        text-align: center;
                        width: 513px;
                        margin-top: 0;
                        margin-bottom: 20px;
                        font-family: Satoshi, sans-serif;
                        font-size: 48px;
                        font-weight: 700;
                        line-height: 72px;
                        margin: auto;
                    }

                    .happy-feedback-heading-container {
                        background-color: #713f1230;
                        border: 1px solid #713f12;
                        border-radius: 33px;
                        align-items: center;
                        width: 35vw;
                        margin-bottom: 48px;
                        padding: 8px 8px;
                        font-size: 20px;
                        line-height: 28px;
                        margin: auto;
                    }

                    .student-feedback-smilie-emoji-2 {
                        width: 32px;
                        margin-right: 40px;
                    }

                    .happy-feeback-slider-section-text {
                        color: #f59e0b;
                        font-family: Inter, sans-serif;
                        font-weight: 500;
                    }



                    .slider-student-feedback-section {
                        max-width: 1000px;
                        margin: auto;
                        padding: 0 10px;
                    }

                    .slider-container-student-feedback-section {
                        overflow: hidden;
                        margin-bottom: 20px;
                    }

                    /* CARDS WRAPPER */
                    .cards-wrapper-student-feedback-section {
                        display: flex;
                        gap: 20px;
                        transition: transform 0.4s ease;
                        scroll-snap-type: x mandatory;
                        -webkit-overflow-scrolling: touch;
                        overflow-x: auto;
                        scrollbar-width: none;
                    }

                    .cards-wrapper-student-feedback-section:-webkit-scrollbar {
                        display: none;
                    }

                    .card-wrapper-student-feedback-section {
                        scroll-snap-align: center;
                        flex-shrink: 0;
                        width: 85vw;
                        background-color: #1e293b;
                        border-radius: 12px;
                        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
                        color: #e2e8f0;
                        display: flex;
                        flex-direction: column;
                        justify-content: flex-start;
                        padding: 16px;
                    }






                    .card-wrapper-student-feedback-section {
                        width: calc((100% - 20px) / 2);
                    }

                    @media (max-width: 767px) {
                        .card-wrapper-student-feedback-section {
                            width: 80vw;

                        }

                        .student-img {
                            width: 14px;
                            height: 14px;
                            object-fit: cover;
                            border-radius: 50%;
                            margin-right: 2px;
                        }

                        .student-h2 {
                            padding-left: 10px;
                            font-size: 4px;
                            line-height: 1;
                        }


                        .text-block-2 {
                            line-height: 1;
                            font-size: 2px;
                            padding-left: 10px;
                        }


                        .student-feedback-text {

                            width: 90%;
                            margin-top: 3vh;

                        }


                        .linkedin-icon {
                            width: 90%;
                            margin-left: 1vw;
                        }

                        .happy-feedback-heading-container {
                            width: 75vw;
                        }

                        .student-feedback-section-heading {
                            width: 80vw;
                            margin-bottom: 20px;
                        }
                    }

                    .student-img {
                        width: 64px;
                        height: 64px;
                        object-fit: cover;
                        border-radius: 50%;
                    }

                    .student-h2 {
                        color: #e2e8f0;

                        font-family: Inter, sans-serif;
                        font-size: 18px;
                        font-weight: 600;
                        line-height: 1.4;
                    }

                    .text-block-2 {
                        font-family: Inter, sans-serif;
                        font-size: 16px;
                        line-height: 1;
                        color: #cbd5e1;
                    }

                    .linkedin-icon {

                        height: 55px;
                    }


                    .student-feedback-text {
                        color: #e2e8f0;
                        font-family: Inter, sans-serif;
                        font-size: 16px;
                        font-weight: 500;
                        line-height: 1.6;
                        padding: 0 10px 16px 10px;
                        word-wrap: break-word;
                    }


                    .linkedin-text {
                        color: #60a5fa;
                        font-size: 16px;
                        line-height: 1.5;
                        text-decoration: none;
                    }

                    /* NAVIGATION SECTION */
                    .slider-controls-student-feedback-section {
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        gap: 16px;
                    }

                    .track-button-student-feedback-section {
                        background-color: transparent;
                        border-radius: 50%;
                        width: 40px;
                        height: 40px;
                        display: flex;
                        align-items: center;
                        justify-content: center;
                        cursor: pointer;
                    }

                    .dots {
                        display: flex;
                        gap: 6px;
                        justify-content: center;
                        margin-top: 10px;
                    }

                    .dot {
                        width: 10px;
                        height: 10px;
                        border-radius: 50%;
                        background-color: #94a3b8;
                        transition: all 0.3s ease;
                    }

                    .dot.active {
                        width: 20px;
                        border-radius: 6px;
                        background-color: #60a5fa;
                    }
                </style>

                <div>
                    <div class="d-flex flex-column justify-content-center">
                        <div>
                            <h2 class="student-feedback-section-heading">
                                Students Say,<br />It’s a Blockbuster!
                            </h2>
                        </div>
                        <div class="happy-feedback-heading-container d-flex  flex-row justify-content-center  ">

                            <div class="student-feedback-smilie-emoji-2 w-embed">
                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/emoji-icon.png" alt="emoji" height="100%" loading="lazy">
                            </div>
                            <div class="happy-feeback-slider-section-text">25000+Happy Feedbacks</div>
                        </div>

                    </div>

                    <div class="slider-student-feedback-section">
                        <!-- Cards at top -->
                        <div class="slider-container-student-feedback-section mt-5">
                            <div class="cards-wrapper-student-feedback-section" id="cardsWrapper-student-feedback-section">
                                <div class="card-wrapper-student-feedback-section">
                                    <div>
                                        <div class="d-flex flex-row justify-content-around">
                                            <div><img class="student-img " src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/neha-panakanapalli-linkedin-profile-pic.png" alt="" loading="lazy"></div>
                                            <div class="d-flex flex-column justify-content-center ">
                                                <h2 class="student-h2">Neha Panakanapalli <span class="text-block-2">. 1st</span></h2>

                                                <div class="text-block-2">Fellow at CCBP 4.0 academy | NxtWave</div>
                                            </div>
                                            <div><img class="linkedin-icon" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/linkedin-logo.svg" alt="" loading="lazy"></div>

                                        </div>

                                        <div class="student-feedback-text">These podcasts are really special! I started listening from a student perspective and ended up learning the product manager's perspective ...<a href="https://www.linkedin.com/posts/neha-panakanapalli-074210247_podcast-language-programming-activity-7007598726974238720-PZje" target="_blank" class="linkedin-text">Read More on LinkedIn</a></div>
                                    </div>
                                </div>
                                <div class="card-wrapper-student-feedback-section">
                                    <div>
                                        <div class="d-flex flex-row justify-content-around ">
                                            <div><img class="student-img" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/rahul-gunturi-linkedin-profile-pic.png" alt="" loading="lazy"></div>
                                            <div class="d-flex flex-column justify-content-center ">
                                                <h2 class="student-h2">Rahul Gunturi
                                                    <span class="text-block-2">. 1st</span>
                                                </h2>

                                                <div class="text-block-2">Fellow at CCBP 4.0 academy | NxtWave</div>
                                            </div>
                                            <div><img class="linkedin-icon" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/linkedin-logo.svg" alt="" loading="lazy"></div>

                                        </div>

                                        <div class="student-feedback-text">These podcasts are beneficial to us as it acts as a bridge, helping us to understand what to do next and how to face situations in life. Thanks ...<a href="https://www.linkedin.com/posts/rrahulguturii_saikirangorthi-nxtwave-google-activity-7030427567677468672-SU3Y" target="_blank" class="linkedin-text">Read More on LinkedIn</a></div>
                                    </div>
                                </div>
                                <div class="card-wrapper-student-feedback-section">
                                    <div>
                                        <div class="d-flex flex-row justify-content-around ">
                                            <div><img class="student-img" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/sai-rohith-linkedin-profile-pic.png" alt="" loading="lazy"></div>
                                            <div class="d-flex flex-column justify-content-center ">
                                                <h2 class="student-h2">Sai Rohith

                                                    <span class="text-block-2">. 1st</span>
                                                </h2>

                                                <div class="text-block-2">Fellow at CCBP 4.0 academy | NxtWave</div>
                                            </div>
                                            <div><img class="linkedin-icon" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/linkedin-logo.svg" alt="" loading="lazy"></div>

                                        </div>

                                        <div class="student-feedback-text">As a CCBP 4.0 Academy student, I feel very lucky that I get access to the knowledge of top-notch experts with ease. Thanks to NxtWave ...<a href="https://www.linkedin.com/posts/rrahulguturii_saikirangorthi-nxtwave-google-activity-7030427567677468672-SU3Y" target="_blank" class="linkedin-text">Read More on LinkedIn</a></div>
                                    </div>
                                </div>
                                <div class="card-wrapper-student-feedback-section">
                                    <div>
                                        <div class="d-flex flex-row justify-content-around ">
                                            <div><img class="student-img" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/rupesh-reddy-loka-linkedin-profile-pic.png" alt="" loading="lazy"></div>
                                            <div class="d-flex flex-column justify-content-center ">
                                                <h2 class="student-h2">Rupesh Reddy Loka


                                                    <span class="text-block-2">. 1st</span>
                                                </h2>

                                                <div class="text-block-2">Fellow at CCBP 4.0 academy | NxtWave</div>
                                            </div>
                                            <div><img class="linkedin-icon" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/linkedin-logo.svg" alt="" loading="lazy"></div>

                                        </div>

                                        <div class="student-feedback-text">After Gowtham sir's podcast, I got really motivated with some of his insights and experiences and also noted some points! He enlightened ...<a href="https://www.linkedin.com/posts/rupesh-reddy-loka_podcast-gowthamreddy-nxtwave-activity-6982297960650850304-uCVU" target="_blank" class="linkedin-text">Read More on LinkedIn</a></div>
                                    </div>
                                </div>
                                <div class="card-wrapper-student-feedback-section">

                                    <div>
                                        <div class="d-flex flex-row justify-content-around ">
                                            <div><img class="student-img" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/gunda-vamshi-linkedin-profile-pic.png" alt="" loading="lazy"></div>
                                            <div class="d-flex flex-column justify-content-center ">
                                                <h2 class="student-h2">Gunda Vamshi



                                                    <span class="text-block-2">. 1st</span>
                                                </h2>

                                                <div class="text-block-2">Fellow at CCBP 4.0 academy | NxtWave</div>
                                            </div>
                                            <div><img class="linkedin-icon" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/linkedin-logo.svg" alt="" loading="lazy"></div>

                                        </div>

                                        <div class="student-feedback-text">Very excellent and learnt many insights from the podcast. I really thank to Archita ma'am for delivering such great insights in the podcast. ...<a href="https://www.linkedin.com/posts/gunda-vamshi-034137216_ccbp-ccbpian-ccbpacademy-activity-6997442879845543936-x8PF" target="_blank" class="linkedin-text">Read More on LinkedIn</a></div>
                                    </div>
                                </div>
                                <div class="card-wrapper-student-feedback-section">

                                    <div>
                                        <div class="d-flex flex-row justify-content-around ">
                                            <div><img class="student-img" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/narasimha-naidu-talari-linkedin-profile-pic.png" alt="" loading="lazy"></div>
                                            <div class="d-flex flex-column justify-content-center ">
                                                <h2 class="student-h2">Narasimha Naidu Talari



                                                    <span class="text-block-2">. 1st</span>
                                                </h2>

                                                <div class="text-block-2">Fellow at CCBP 4.0 academy | NxtWave</div>
                                            </div>
                                            <div><img class="linkedin-icon" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/linkedin-logo.svg" alt="" loading="lazy"></div>

                                        </div>

                                        <div class="student-feedback-text">Ma'am answered all our student questions and shared her experience on how to build the best career in IT! It is very useful to me , Thank you ...<a href="https://www.linkedin.com/posts/narasimha-naidu-talari-553622248_podcast-nxtwaveteam-experience-activity-6997446557964939264-rjPM" target="_blank" class="linkedin-text">Read More on LinkedIn</a></div>
                                    </div>
                                </div>


                                <div class="card-wrapper-student-feedback-section">

                                    <div>
                                        <div class="d-flex flex-row justify-content-around ">
                                            <div><img class="student-img" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/nafiya-linkedin-profile-pic.png" alt="" loading="lazy"></div>
                                            <div class="d-flex flex-column justify-content-center ">
                                                <h2 class="student-h2">
                                                    N S Nafiya




                                                    <span class="text-block-2">. 1st</span>
                                                </h2>

                                                <div class="text-block-2">Fellow at CCBP 4.0 academy | NxtWave</div>
                                            </div>
                                            <div><img class="linkedin-icon" src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/student-testimonials/linkedin-logo.svg" alt="" loading="lazy"></div>

                                        </div>

                                        <div class="student-feedback-text">I learned about Amazon's 4C's of hiring. The podcast provided great insights into the recruiter's perspective and the company's evaluation ...<a href="https://www.linkedin.com/posts/n-s-nafiya_nxtwave-rahulattuluri-ccbpian-activity-7022859013105098752-jL7y" target="_blank" class="linkedin-text">Read More on LinkedIn</a></div>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- Navigation at bottom -->
                        <div class="slider-controls-student-feedback-section d-none  d-md-flex align-items-center justify-content-center">
                            <div class="track-button-student-feedback-section " id="leftBtn-student-feedback-section">
                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/64533d2ddcff961c1800edb8_Icon%20(1).png" alt="←">
                            </div>

                            <div class="dots" id="dotsWrapper"></div>

                            <div class="track-button" id="rightBtn-student-feedback-section">
                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/64533d2ddcff9613ab00edb6_Icon.png" alt="→">
                            </div>
                        </div>
                    </div>





                </div>
            </div>



            <div class="col-12  order-5  nxtwave-empowering-podcast-section">
                <style>
                    .nxtwave-empowering-podcast-section {
                        background-color: #0f172a;
                        background-image: url("https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/64362e90abbff4e843d25fd4_NxtWave's%20Empowering%20Podcast%20Series%20%20to%20Shape%20your%20Dream%20Career.%20(1).png");
                        background-position: 80%;
                        background-size: cover;
                        padding: 96px 110px;
                    }

                    .nxtwave-empowering-podcast-section-h2 {
                        color: #f1f5f9;

                        display: flex;
                        margin-bottom: 48px;
                        font-family: Satoshi, sans-serif;
                        font-size: 48px;
                        font-weight: 700;
                        line-height: 72px;

                    }

                    .nxtwave-empowering-podcast-section-text {
                        color: #e2e8f0;
                        font-family: Inter, sans-serif;
                        font-size: 24px;
                        line-height: 32px;

                    }


                    @media (max-width: 768px) {
                        .nxtwave-empowering-podcast-section-h2 {
                            width: 85vw;

                        }

                        .nxtwave-empowering-podcast-section {
                            padding: 48px 25px;
                        }
                    }
                </style>




                <div class="d-flex flex-column justify-content-around">
                    <div>
                        <h1 class="nxtwave-empowering-podcast-section-h2">NxtWave's Empowering Podcast Series to Shape your Dream Career</h1>
                    </div>

                    <div class="d-flex flex-row  justify-content-start mt-5 align-items-center">
                        <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/nxtwaves-empowering-podcast-section/mic-logo.svg" alt="" height="60px" loading="lazy"></div>
                        <div class="nxtwave-empowering-podcast-section-text">100+ Podcasts</div>
                    </div>


                    <div class="d-flex flex-row  justify-content-start mt-5 align-items-center">
                        <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/nxtwaves-empowering-podcast-section/rupee-logo.svg" alt="" height="60px" loading="lazy"></div>
                        <div class="nxtwave-empowering-podcast-section-text">Each worth ₹2000/-</div>
                    </div>




                    <div class="d-flex flex-row  justify-content-start mt-5 align-items-center">
                        <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/nxtwaves-empowering-podcast-section/flame-logo.svg" alt="" height="60px" loading="lazy"></div>
                        <div class="nxtwave-empowering-podcast-section-text">FREE for NxtWave Academy students</div>
                    </div>





                    <div class="d-flex flex-row  justify-content-start mt-5 ">

                        <a href="#claim-your-free-access-section"> <button class="vertical-slider-btn1 ">Claim Free Access</button></a>

                    </div>
                </div>
            </div>



            <div class="col-12  order-md-6 d-none d-md-block claim-your-free-access-section" id="claim-your-free-access-section1">

                <div class="d-flex flex-row justify-content-center align-items-center">
                    <div>
                        <h5 class="claim-your-free-access-h5">Claim Your<br />
                            Free Access to a Podcast</h5>
                    </div>

                    <div class="otp-form">
                        <style>
                            .otp-form {
                                background: transparent;
                                padding: 30px;

                                width: 100%;
                                max-width: 400px;
                            }



                            .input-field {
                                background-color: rgb(51, 65, 85) !important;
                                color: rgb(248, 250, 252);
                                font-size: 14px;
                                font-weight: 500;
                                line-height: 20px;
                                font-family: Inter, sans-serif;
                                border: 1px solid gray !important;
                                border-radius: 5px;
                                padding: 10px;
                            }

                            .input-field.error {

                                border: 0.5px solid red;
                            }

                            .form-label {
                                font-weight: bold;
                                margin-bottom: 5px;
                            }

                            .input-group .input-group-prepend select {
                                border-top-left-radius: 5px;
                                border-bottom-left-radius: 5px;
                                background-color: rgb(51, 65, 85) !important;
                                color: white;
                                font-family: Inter, sans-serif;
                                font-size: 14px;
                                font-weight: 500;
                                border: 1px solid grey;
                            }

                            .input-group .form-control.input-field {
                                border-top-left-radius: 0;
                                border-bottom-left-radius: 0;
                            }

                            select:focus,
                            input:focus {
                                outline: none !important;
                                box-shadow: none !important;
                            }






                            .claim-your-free-access-section {
                                background-color: #0f172a;

                            }


                            .claim-your-free-access-h5 {
                                --tw-text-opacity: 1;
                                color: rgba(241, 245, 249, var(--tw-text-opacity));
                                font-weight: 700;
                                font-size: 48px;
                                line-height: 72px;
                                font-family: "Satoshi variable", sans-serif;
                            }
                        </style>
                        <form id="otpRequestForm">
                            <div class="form-group">
                                <label class="form-label text-white" for="name">Name</label>
                                <input type="text" class="form-control  input-field" id="name" placeholder="Enter your name" required />
                            </div>

                            <div class="form-group">
                                <label class="form-label  text-white" for="phone">Phone Number</label>
                                <div class="input-group">
                                    <div class="input-group-prepend">
                                        <select id="countryCode" class="form-control">
                                            <option value="+91" selected>+91</option>
                                            <option value="+1">+1</option>
                                            <option value="+44">+44</option>
                                            <option value="+61">+61</option>
                                            <option value="+971">+971</option>
                                        </select>
                                    </div>
                                    <input type="tel" class="form-control input-field" id="phone" placeholder="Enter phone number" required />
                                </div>
                            </div>

                            <button type="submit" class="btn btn-primary btn-block">Get OTP</button>
                        </form>
                        <div id="responseMessage" class="mt-3 text-success text-center"></div>
                    </div>
                </div>
            </div>

            <div class="col-12  order-6 d-md-none claim-your-free-access-section" id="claim-your-free-access-section2">

                <div class="d-flex flex-column justify-content-center align-items-center">
                    <div>
                        <h5 class="claim-your-free-access-h5">Claim Your<br />
                            Free Access to a Podcast</h5>
                    </div>

                    <div class="otp-form">

                        <form id="otpRequestForm">
                            <div class="form-group">
                                <label class="form-label text-white" for="name">Name</label>
                                <input type="text" class="form-control  input-field" id="name" placeholder="Enter your name" required />
                            </div>

                            <div class="form-group">
                                <label class="form-label  text-white" for="phone">Phone Number</label>
                                <div class="input-group">
                                    <div class="input-group-prepend">
                                        <select id="countryCode" class="form-control">
                                            <option value="+91" selected>+91</option>
                                            <option value="+1">+1</option>
                                            <option value="+44">+44</option>
                                            <option value="+61">+61</option>
                                            <option value="+971">+971</option>
                                        </select>
                                    </div>
                                    <input type="tel" class="form-control input-field" id="phone" placeholder="Enter phone number" required />
                                </div>
                            </div>

                            <button type="submit" class="btn btn-primary btn-block">Get OTP</button>
                        </form>
                        <div id="responseMessage" class="mt-3 text-success text-center"></div>
                    </div>
                </div>
            </div>



            <div class="col-12  order-7  section-empty-outer">
                <style>
                    .section-empty-outer {
                        background-image: url("https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/645345c7c2106e1bd1c65a6c_Background%20String.png");
                        background-size: cover;
                    }

                    .section-empty-inner {
                        max-width: 1200px;
                        margin-left: auto;
                        margin-right: auto;
                        padding-top: 48px;
                        padding-bottom: 48px;
                    }

                    .section-empty-text {
                        color: #fff;
                        font-family: Inter, sans-serif;
                        font-size: 18px;
                        font-weight: 400;
                        line-height: 28px;
                    }

                    .footer-ul {
                        list-style-type: none;
                    }
                </style>
                <div class="section-empty-inner">
                    <div class="section-empty-text">* The speaker profiles are as on the recorded date</div>
                </div>
            </div>


            <div class="col-12  order-md-8 footer d-none d-md-block">

                <div class="d-flex flex-column justify-content-around footer ">

                    <div class="d-flex flex-row justify-content-around">
                        <div class="d-flex flex-column justify-content-around ">
                            <div>
                                <a href="https://www.ccbp.in/" target="_blank"> <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/Nxtwave_White_logo.svg" /></a>
                            </div>
                            <div>
                                <h6 class="footer-h6  mt-5 mb-5">Reach Us</h6>
                            </div>
                            <div>
                                <a href="mailto:support@nxtwave.tech" class="footer-email">
                                    <div class="d-flex flex-row justify-content-start">
                                        <div class="mr-3">
                                            <img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3c91504378bb16eca4973_mail-icon.svg" />
                                        </div>
                                        <div>support@nxtwave.tech</div>
                                    </div>
                                </a>
                            </div>
                        </div>

                        <div>
                            <div class="footer-row2-heading ">Quick Links</div>
                            <div class="d-flex flex-row justify-content-around">
                                <div>
                                    <ul class="footer-ul">
                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/?_gl=1*zwrta8*_ga*MTEzNDI2NjQ3Ny4xNzQ2Mjc2Mjg1*_ga_VNJELL2WMV*czE3NTA4NTg0MjMkbzg1JGcxJHQxNzUwODYxMDczJGo2MCRsMCRoMA.." target="_blank">Home</a></li>
                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/academy" target="_blank">Academy</a></li>

                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/intensive" target="_blank">Intensive</a></li>

                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/hire" target="_blank">Hire with us</a></li>


                                    </ul>
                                </div>


                                <div>
                                    <ul class="footer-ul">
                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/contact-us?_gl=1*ab368j*_ga*MTEzNDI2NjQ3Ny4xNzQ2Mjc2Mjg1*_ga_VNJELL2WMV*czE3NTA5MTg3NDUkbzg2JGcxJHQxNzUwOTE4OTQ4JGozMSRsMCRoMA.." target="_blank">Contact Us</a></li>
                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/about" target="_blank">About Us</a></li>

                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/reviews" target="_blank">Reviews </a></li>



                                    </ul>
                                </div>
                            </div>




                        </div>

                        <div>
                            <div class="footer-row2-heading ">Payment Methods</div>
                            <div class="d-flex flex-column justify-content-around ">
                                <div class="d-flex flex-row justify-content-around mb-3 ">
                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3c93dfbc8568fcb27e556_visa-icon.svg" /></div>
                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3c976a29a435d3fc17f27_mastercard-icon.svg" /></div>

                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fcf36619310922216dcb_payment-method-icon3.svg" /></div>




                                </div>

                                <div class="d-flex flex-row justify-content-around ">
                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fcf46ba93fa0919d5828_Razor-pay-icon.svg" /></div>
                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fcf34a02bed6c7dbc750_upi-icon.svg" /></div>

                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fd566ba93f145d9d5b57_rupay-icon.svg" /></div>




                                </div>

                                <div class="d-flex flex-row justify-content-start mt-3">
                                    <div><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/618dff87c4047e7681214d33_location%20on.svg" loading="lazy" alt="" class="mr-2"></div>

                                    <div class="footer-row3-address">NxtWave, WeWork Rajapushpa Summit, Nanakramguda Rd, Financial District, Manikonda Jagir, Telangana 500032</div>

                                </div>
                            </div>
                        </div>






                    </div>



                    <div class="footer-row3-hr"></div>

                    <div class="d-flex flex-row justify-content-between">
                        <div class="d-flex flex-row justify-content-start ">
                            <div><a href="https://www.facebook.com/NxtWave-106729994530632/" target="_blank" class=""><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fd520d11331f5f3b46ef_facebook-icon.svg" loading="lazy" alt="" /></a></div>
                            <div><a href="https://www.instagram.com/ccbp_nxtwave/" target="_blank" class=""><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fe609dc6ce25f2f7078f_instgram-icon.svg" loading="lazy" alt="" /></a></div>
                            <div><a href="https://twitter.com/nxtwave_tech" target="_blank" class=""><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f400cc41af69932df92c8a_twitterimage.svg" loading="lazy" alt="" /></a></div>
                            <div><a href="https://www.linkedin.com/company/nxtwavetech" target="_blank" class=""><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fe1a40dc31c249e1ab99_linkedin-icon.svg" loading="lazy" alt="" /></a></div>
                            <div><a href="https://www.youtube.com/c/NxtWaveTech" target="_blank" class=""><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/62384993d97ad72405dee8d2_Frame%2031%20(1).svg" loading="lazy" alt="" /></a></div>



                        </div>

                        <div class="d-flex flex-row justify-content-around ">
                            <div><a class="footer-row2-links" href="https://www.ccbp.in/privacy-policy?_gl=1*8262ju*_ga*MTEzNDI2NjQ3Ny4xNzQ2Mjc2Mjg1*_ga_VNJELL2WMV*czE3NTA5MTg3NDUkbzg2JGcxJHQxNzUwOTIxNDE4JGo2MCRsMCRoMA.." target="_blank">Privacy Policy</a></div>
                            <div><a class="footer-row2-links pl-3" href="https://www.ccbp.in/cookie-policy" target="_blank">Cookie Policy</a></div>
                            <div><a class="footer-row2-links  pl-3" href="https://www.ccbp.in/terms-and-conditions" target="_blank">Terms and Conditions</a></div>
                            <div><a class="footer-row2-links  pl-3" href="https://www.ccbp.in/grievance-redressal" target="_blank">Grievance Redressal</a></div>
                            <div><a class="footer-row2-links  pl-3" href="https://www.ccbp.in/corporate-information" target="_blank">Corporate Information</a></div>

                        </div>

                    </div>

                </div>

            </div>

            <div class="col-12  order-8 footer  d-md-none">
                <style>
                    .footer {
                        background-color: #0f172a;
                        padding-top: 96px;
                        padding-bottom: 96px;
                        font-family: Inter, sans-serif;
                    }

                    .footer-h6 {
                        color: #5a7184;
                        margin-top: 0;
                        margin-bottom: 0;
                        font-family: Inter, sans-serif;
                        font-size: 18px;
                        font-weight: 700;
                        line-height: 24px;
                        text-decoration: none;
                    }

                    .footer-email {
                        text-decoration: none;

                    }

                    .footer-row2-heading {
                        color: #5a7184;
                        margin-left: 4vw;
                        margin-bottom: 3vh;
                        font-size: 18px;
                        font-weight: 700;
                        line-height: 24px;
                    }

                    .footer-row2-links {
                        opacity: .7;
                        color: #959ead;
                        font-size: 16px;
                        font-weight: 400;
                        line-height: 24px;
                        text-decoration: none;
                        transition: opacity .2s;

                    }

                    .footer-row2-links:hover {
                        color: #ffffff;
                        text-decoration: none;
                    }

                    .footer-row3-img {
                        max-width: 100%;
                        height: auto;
                        padding: 10px;
                    }

                    .footer-row3-address {
                        opacity: .7;
                        color: #959ead;
                        width: 232px;
                        height: 120px;
                        font-size: 16px;
                        font-weight: 400;
                        line-height: 24px;
                    }

                    .footer-row3-hr {
                        background-color: #1e293b;
                        border-radius: 2px;
                        height: 2px;
                        margin-top: 32px;
                        margin-bottom: 32px;
                    }

                    @media(max-width:768px) {
                        .footer-row2-heading {
                            margin-left: 6vw;
                            margin-top: 5vh;
                        }

                        .footer-small-col1 {
                            margin-left: 6vw;
                        }

                    }
                </style>
                <div class="d-flex flex-column justify-content-around footer ">

                    <div class="d-flex flex-column justify-content-around">
                        <div class="d-flex flex-column justify-content-around  footer-small-col1">
                            <div>
                                <a href="https://www.ccbp.in/" target="_blank"> <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/Nxtwave_White_logo.svg" /></a>
                            </div>
                            <div>
                                <h6 class="footer-h6  mt-5 mb-5">Reach Us</h6>
                            </div>
                            <div>
                                <a href="mailto:support@nxtwave.tech" class="footer-email">
                                    <div class="d-flex flex-row justify-content-start">
                                        <div class="mr-3">
                                            <img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3c91504378bb16eca4973_mail-icon.svg" />
                                        </div>
                                        <div>support@nxtwave.tech</div>
                                    </div>
                                </a>
                            </div>
                        </div>

                        <div>
                            <div class="footer-row2-heading ">Quick Links</div>
                            <div class="d-flex flex-row justify-content-start footer-row2-links-container">
                                <div>
                                    <ul class="footer-ul">
                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/?_gl=1*zwrta8*_ga*MTEzNDI2NjQ3Ny4xNzQ2Mjc2Mjg1*_ga_VNJELL2WMV*czE3NTA4NTg0MjMkbzg1JGcxJHQxNzUwODYxMDczJGo2MCRsMCRoMA.." target="_blank">Home</a></li>
                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/academy" target="_blank">Academy</a></li>

                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/intensive" target="_blank">Intensive</a></li>

                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/hire" target="_blank">Hire with us</a></li>


                                    </ul>
                                </div>


                                <div>
                                    <ul class="footer-ul">
                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/contact-us?_gl=1*ab368j*_ga*MTEzNDI2NjQ3Ny4xNzQ2Mjc2Mjg1*_ga_VNJELL2WMV*czE3NTA5MTg3NDUkbzg2JGcxJHQxNzUwOTE4OTQ4JGozMSRsMCRoMA.." target="_blank">Contact Us</a></li>
                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/about" target="_blank">About Us</a></li>

                                        <li><a class="footer-row2-links" href="https://www.ccbp.in/reviews" target="_blank">Reviews </a></li>



                                    </ul>
                                </div>
                            </div>




                        </div>

                        <div>
                            <div class="footer-row2-heading ">Payment Methods</div>
                            <div class="d-flex flex-column justify-content-around ">
                                <div class="d-flex flex-row justify-content-around mb-3 ">
                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3c93dfbc8568fcb27e556_visa-icon.svg" /></div>
                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3c976a29a435d3fc17f27_mastercard-icon.svg" /></div>

                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fcf36619310922216dcb_payment-method-icon3.svg" /></div>




                                </div>

                                <div class="d-flex flex-row justify-content-around ">
                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fcf46ba93fa0919d5828_Razor-pay-icon.svg" /></div>
                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fcf34a02bed6c7dbc750_upi-icon.svg" /></div>

                                    <div><img class="footer-row3-img" src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fd566ba93f145d9d5b57_rupay-icon.svg" /></div>




                                </div>

                                <div class="d-flex flex-row justify-content-start mt-3 footer-small-col1">
                                    <div><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/618dff87c4047e7681214d33_location%20on.svg" loading="lazy" alt="" class="mr-2"></div>

                                    <div class="footer-row3-address ">NxtWave, WeWork Rajapushpa Summit, Nanakramguda Rd, Financial District, Manikonda Jagir, Telangana 500032</div>

                                </div>
                            </div>
                        </div>






                    </div>



                    <div class="footer-row3-hr"></div>

                    <div class="d-flex flex-column justify-content-around footer-small-col1">
                        <div class="d-flex flex-row justify-content-start  ">
                            <div class="mr-3"><a href="https://www.facebook.com/NxtWave-106729994530632/" target="_blank" class=""><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fd520d11331f5f3b46ef_facebook-icon.svg" loading="lazy" alt="" /></a></div>
                            <div class="mr-3"><a href="https://www.instagram.com/ccbp_nxtwave/" target="_blank" class=""><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fe609dc6ce25f2f7078f_instgram-icon.svg" loading="lazy" alt="" /></a></div>
                            <div class="mr-3"><a href="https://twitter.com/nxtwave_tech" target="_blank" class=""><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f400cc41af69932df92c8a_twitterimage.svg" loading="lazy" alt="" /></a></div>
                            <div class="mr-3"><a href="https://www.linkedin.com/company/nxtwavetech" target="_blank" class=""><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/61f3fe1a40dc31c249e1ab99_linkedin-icon.svg" loading="lazy" alt="" /></a></div>
                            <div class="mr-3"><a href="https://www.youtube.com/c/NxtWaveTech" target="_blank" class=""><img src="https://cdn.prod.website-files.com/5fa61cbbf0d432b3230f62b1/62384993d97ad72405dee8d2_Frame%2031%20(1).svg" loading="lazy" alt="" /></a></div>



                        </div>

                        <div class="d-flex flex-column justify-content-around pb-3 pt-3 ">
                            <div><a class="footer-row2-links" href="https://www.ccbp.in/privacy-policy?_gl=1*8262ju*_ga*MTEzNDI2NjQ3Ny4xNzQ2Mjc2Mjg1*_ga_VNJELL2WMV*czE3NTA5MTg3NDUkbzg2JGcxJHQxNzUwOTIxNDE4JGo2MCRsMCRoMA.." target="_blank">Privacy Policy</a></div>
                            <div><a class="footer-row2-links " href="https://www.ccbp.in/cookie-policy" target="_blank">Cookie Policy</a></div>
                            <div><a class="footer-row2-links  " href="https://www.ccbp.in/terms-and-conditions" target="_blank">Terms and Conditions</a></div>
                            <div><a class="footer-row2-links  " href="https://www.ccbp.in/grievance-redressal" target="_blank">Grievance Redressal</a></div>
                            <div><a class="footer-row2-links  " href="https://www.ccbp.in/corporate-information" target="_blank">Corporate Information</a></div>

                        </div>

                    </div>

                </div>

            </div>

        </div>
    </div>

    <script>
        const wrapper = document.getElementById("cardsWrapper-student-feedback-section");
        const cards = wrapper.querySelectorAll(".card-wrapper-student-feedback-section");
        const prevBtn = document.getElementById("leftBtn-student-feedback-section");
        const nextBtn = document.getElementById("rightBtn-student-feedback-section");
        const dotsWrapper = document.getElementById("dotsWrapper");

        let currentIndex = 0;

        const updateSlider = () => {
            const cardWidth = cards[0].offsetWidth + 20;
            wrapper.scrollTo({
                left: currentIndex * cardWidth,
                behavior: "smooth"
            });
            updateDots();
        };

        const updateDots = () => {
            const dots = dotsWrapper.querySelectorAll(".dot");
            dots.forEach(dot => dot.classList.remove("active"));
            if (dots[currentIndex]) dots[currentIndex].classList.add("active");
        };

        for (let i = 0; i < cards.length; i++) {
            const dot = document.createElement("div");
            dot.classList.add("dot");
            if (i === 0) dot.classList.add("active");
            dot.addEventListener("click", () => {
                currentIndex = i;
                updateSlider();
            });
            dotsWrapper.appendChild(dot);
        }

        nextBtn.addEventListener("click", () => {
            currentIndex = (currentIndex + 1) % cards.length;
            updateSlider();
        });

        prevBtn.addEventListener("click", () => {
            currentIndex = (currentIndex - 1 + cards.length) % cards.length;
            updateSlider();
        });

        wrapper.addEventListener("scroll", () => {
            const cardWidth = cards[0].offsetWidth + 20;
            const newIndex = Math.round(wrapper.scrollLeft / cardWidth);
            if (newIndex !== currentIndex) {
                currentIndex = newIndex;
                updateDots();
            }
        });
    </script>


    <script>
        const wrapper = document.getElementById("vertical-slider");
        const items = wrapper.children.length;
        const itemHeight = 90;
        let index = 0;

        setInterval(() => {
            index++;
            wrapper.style.transition = "transform 0.6s ease-in-out";
            wrapper.style.transform = `translateY(-${index * itemHeight}px)`;

            if (index === items) {
                setTimeout(() => {
                    wrapper.style.transition = "none";
                    wrapper.style.transform = "translateY(0)";
                    index = 0;
                }, 600);
            }
        }, 2500);
    </script>
    <!-- JS Script for Video Loop -->
    <script>
        const videoList = [
            'https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/landing-section-bg-videos/mobile-videos/ritesh-amazon.mp4',
            'https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/landing-section-bg-videos/mobile-videos/sandeep-uber.mp4',
            'https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/landing-section-bg-videos/mobile-videos/sanjay-sehgal-mysys.mp4',
            'https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/landing-section-bg-videos/mobile-videos/shiva-ghani-microsoft.mp4',
            'https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/landing-section-bg-videos/mobile-videos/siva-kumar-slice.mp4',
            'https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/landing-section-bg-videos/mobile-videos/naveen-superk.mp4'
        ];

        let currentVideo = 0;
        const videoElement = document.getElementById('bg-video');

        function playVideo(index) {
            videoElement.src = videoList[index];
            videoElement.load();
            videoElement.play();
        }

        videoElement.addEventListener('ended', () => {
            currentVideo = (currentVideo + 1) % videoList.length;
            playVideo(currentVideo);
        });

        playVideo(currentVideo);
    </script>


    <script>
        function initDesktopSlider(wrapperId, leftBtnId, rightBtnId) {
            const cardsWrapper = document.getElementById(wrapperId);
            if (!cardsWrapper || cardsWrapper.getAttribute("data-initialized") === "true") return;

            const cardWidth = cardsWrapper.querySelector(".card-wrapper").offsetWidth + 30;
            const visibleCards = 3;
            let position = 0;

            const allCards = cardsWrapper.querySelectorAll(".card-wrapper");
            const totalCards = allCards.length;

            const cloneFirst = [];
            const cloneLast = [];
            for (let i = 0; i < visibleCards; i++) {
                cloneFirst.push(allCards[i].cloneNode(true));
                cloneLast.push(allCards[totalCards - 1 - i].cloneNode(true));
            }

            cloneFirst.forEach(node => cardsWrapper.appendChild(node));
            cloneLast.reverse().forEach(node => cardsWrapper.insertBefore(node, cardsWrapper.firstChild));

            const updatedTotal = cardsWrapper.querySelectorAll(".card-wrapper").length;
            position = visibleCards;
            cardsWrapper.style.transform = `translateX(-${cardWidth * position}px)`;

            function slide(direction) {
                if (direction === 'right') {
                    position += visibleCards;
                    cardsWrapper.style.transition = 'transform 0.5s ease';
                    cardsWrapper.style.transform = `translateX(-${cardWidth * position}px)`;

                    setTimeout(() => {
                        if (position >= updatedTotal - visibleCards) {
                            cardsWrapper.style.transition = 'none';
                            position = visibleCards;
                            cardsWrapper.style.transform = `translateX(-${cardWidth * position}px)`;
                        }
                    }, 500);
                } else {
                    position -= visibleCards;
                    cardsWrapper.style.transition = 'transform 0.5s ease';
                    cardsWrapper.style.transform = `translateX(-${cardWidth * position}px)`;

                    setTimeout(() => {
                        if (position < visibleCards) {
                            cardsWrapper.style.transition = 'none';
                            position = updatedTotal - visibleCards * 2;
                            cardsWrapper.style.transform = `translateX(-${cardWidth * position}px)`;
                        }
                    }, 500);
                }
            }

            document.getElementById(leftBtnId)?.addEventListener("click", () => slide('left'));
            document.getElementById(rightBtnId)?.addEventListener("click", () => slide('right'));

            cardsWrapper.setAttribute("data-initialized", "true");
        }

        function initMobileSlider(wrapperId) {
            const wrapper = document.getElementById(wrapperId);
            if (!wrapper || wrapper.getAttribute("data-initialized") === "true") return;

            for (let i = 0; i < 3; i++) {
                wrapper.appendChild(wrapper.children[i].cloneNode(true));
            }

            wrapper.addEventListener("scroll", () => {
                const scrollEnd = wrapper.scrollWidth - wrapper.clientWidth;
                if (wrapper.scrollLeft >= scrollEnd - 5) {
                    wrapper.scrollLeft = 0;
                }
            });

            wrapper.setAttribute("data-initialized", "true");
        }
    </script>

    <script>
        const tags = document.querySelectorAll('.div-a');
        const contentMap = {
            trendingTab: 'trendingContent',
            allTab: 'allContent',
            techTab: 'techContent',
            careerTab: 'careerContent',
            cxoTab: 'cxoContent',
            productivityTab: 'productivityContent',
            gsocTab: 'gsocContent',
            panelTab: 'panelContent'
        };

        // IDs of wrappers and buttons per tab
        const sliderIds = {

            allTab: {
                wrapper: 'cardsWrapperAll',
                leftBtn: 'leftBtnAll',
                rightBtn: 'rightBtnAll'
            },
            techTab: {
                wrapper: 'cardsWrapperTech',
                leftBtn: 'leftBtnTech',
                rightBtn: 'rightBtnTech'
            },
            careerTab: {
                wrapper: 'cardsWrapperCareer',
                leftBtn: 'leftBtnCareer',
                rightBtn: 'rightBtnCareer'
            },
            cxoTab: {
                wrapper: 'cardsWrapperCxo',
                leftBtn: 'leftBtnCxo',
                rightBtn: 'rightBtnCxo'
            },
            productivityTab: {
                wrapper: 'cardsWrapperProductivity',
                leftBtn: 'leftBtnProductivity',
                rightBtn: 'rightBtnProductivity'
            },
            gsocTab: {
                wrapper: 'cardsWrapperGsoc',
                leftBtn: 'leftBtnGsoc',
                rightBtn: 'rightBtnGsoc'
            },
            panelTab: {
                wrapper: 'cardsWrapperPanel',
                leftBtn: 'leftBtnPanel',
                rightBtn: 'rightBtnPanel'
            }
        };

        tags.forEach(tag => {
            tag.addEventListener('click', () => {
                tags.forEach(t => t.classList.remove('selected'));
                tag.classList.add('selected');

                Object.values(contentMap).forEach(id => {
                    const section = document.getElementById(id);
                    if (section) section.style.display = 'none';
                });

                const contentId = contentMap[tag.id];
                if (contentId) {
                    const content = document.getElementById(contentId);
                    if (content) {
                        content.style.display = 'block';

                        const ids = sliderIds[tag.id];
                        if (ids) {
                            if (window.innerWidth >= 768) {
                                initDesktopSlider(ids.wrapper, ids.leftBtn, ids.rightBtn);
                            } else {
                                initMobileSlider(ids.wrapper);
                            }
                        }
                    }
                }
            });
        });
    </script>






    <!-- Video Modal -->
    <div class="modal fade" id="videoModal" tabindex="-1">
        <div class="modal-dialog modal-lg modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header">
                    <button class="close" data-dismiss="modal">&times;</button>
                </div>
                <div class="embed-responsive embed-responsive-16by9">
                    <iframe id="youtubeVideo" class="embed-responsive-item" src="" allowfullscreen></iframe>
                </div>
            </div>
        </div>
    </div>
    <script>
        const videoModal = $('#videoModal');
        const iframe = document.getElementById('youtubeVideo');

        $('.bg-sandeep').on('click', function() {
            const videoURL = $(this).data('video') + '?autoplay=1&mute=1&rel=0&showinfo=0&enablejsapi=1';
            iframe.src = videoURL;
            videoModal.modal('show');
        });

        videoModal.on('hidden.bs.modal', function() {
            iframe.src = '';
        });
    </script>























    <!-- sandeep modal-->
    <div class="modal fade" id="sandeepModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/sandeep-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">Sandeep Gorthi</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Engineering Manager at Uber</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Master The Art of Coding </p>
                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/amazon-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/yahoo-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy"></div>


                        <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/grab-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy"></div>


                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Debunk Programming Myths</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">The Path From Developer to Manager</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Work Cultures in Giant Tech Companies</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Cultivating a Love for Tech : Internships & Competitions.</div>
                        </div>

                    </div>




                </div>
            </div>
        </div>
    </div>






    <!-- pritesh modal-->
    <div class="modal fade" id="priteshModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/pritesh-popup-pic.png" width="72px" alt="pritesh"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">Pritesh Malode</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Senior Recruiter at Amazon</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Unlocking the Secrets of the Interview Process </p>
                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/amazon-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/ncr-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy"></div>


                        <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/genpact-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy"></div>


                        <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/byjus-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy"></div>


                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">What Companies are Looking For?</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">What Does Amazon Look for in a Candidate?</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                What Questions are Asked During Interviews?</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">What is the Amazon Culture Like?</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">What is the Most Sought-After Skill and Trait by Recruiters?</div>
                        </div>


                    </div>




                </div>
            </div>
        </div>
    </div>




    <!-- sanjaymodal-->
    <div class="modal fade" id="sanjayModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/sanjay-popup-pic.png" width="72px" alt="pritesh"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">Sanjay Sehgal</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Chairman & CEO at Msys Technologies </p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">A CEO's Guide to Effective Time Management </p>
                    <div class="what-you-will-learn-Experience">Experience</div>
                    <div class="what-you-will-learn-p2 mt-4">Featured in Forbes ,Venture and Angel Investor, Philantrophist, Recognised as the "Most Innovative digital transformation CEO"</div>

                    <div class="d-flex flex-row justify-content-start">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/msys-company-logo.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>
                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>





                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">The CEO Approach to Time Management</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Four Mantras for Effective Time Managementr</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                How to Prioritize Time Efficiently</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Insights on How to Stay Focused</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Top Three Time Management Frameworks</div>
                        </div>

                    </div>


                </div>
            </div>
        </div>
    </div>













    <!-- irshadModal-->
    <div class="modal fade" id="irshadModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c65bbe46002313697190_irshad-profile.webp" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Irshad Chohan</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Senior Solutions Architect at AWS</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Expert in technology reusability, new tech adoption, vendor partnerships, delivery model improvement, and developing tech leaders. </p>
                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c65b0bd457331ef172cd_aws.webp" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c65ba386ce3f21314e79_tcs.webp" alt="" width="87.17px" height="36px" loading="lazy"></div>





                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">How AWS Works</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Cloud Computing</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Design Principles</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Hottest AWS Jobs</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Learning AWS</div>
                        </div>

                    </div>




                </div>
            </div>
        </div>
    </div>






    <!-- varunModal-->
    <div class="modal fade" id="varunModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c9f07efc3f53d81d6d5f_sriram-frofile.webp" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Sriram Varun Vobilisetty</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Product Manager at ALLEN Digital</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Seasoned Product Manager with 4+ years of experience in building and scaling consumer products across AI, Voice Assistants, and EdTech. </p>
                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-column justify-content-around">
                        <div>
                            <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c9ef1acc87ac5abbaa45_Sumsung.webp" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>



                        <div>
                            <p class="what-you-will-learn-p2 mt-4">Alumnus of IIT Kanpur</p>
                        </div>



                        <div><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c9f05dcb6ff9d8baef3c_IIT-Kanpur.webp" alt="" width="87.17px" height="36px" loading="lazy"></div>





                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">AI/ML Stories from Samsung</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Samsung's Work Culture</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Teams at Samsung</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Key Skills for AI/ML Career</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Tips to Upskill</div>
                        </div>

                    </div>




                </div>
            </div>
        </div>
    </div>


    <!-- Krishna Raghavan-->
    <div class="modal fade" id="KrishnaModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c3b94fb7af71878c2717_krishna-raghavan-profile.webp" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Krishna Raghavan</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">People and Tech Leader</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Tech leader with 20+ years of experience, adept at building high-performance teams and driving strategic outcomes.</p>
                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-column justify-content-around">
                        <div class="d-flex flex-row justify-content-around">
                            <div>
                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c3b96985afbe2d18a7a8_flipcart.webp" alt="" width="87.17px" height="36px" loading="lazy">
                            </div>


                            <div><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c3b9cfbf732e3c2b31ca_yahoo.webp" alt="" width="87.17px" height="36px" loading="lazy"></div>



                            <div><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c3b977eb17ab2fe49dd2_cleartrip.webp" alt="" width="87.17px" height="36px" loading="lazy"></div>

                        </div>


                        <div>
                            <p class="what-you-will-learn-p2 mt-4">Tech leader with 20+ years of experience, adept at building high-performance teams and driving strategic outcomes.</p>
                        </div>




                        <div><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690c3b91acc87ac5ab76e1c_denison.webp" alt="" width="87.17px" height="36px" loading="lazy"></div>


                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Time Management</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Effective Goal-setting</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Tips for Focus and Consistency</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Discovering your potential</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Strategies for growth</div>
                        </div>



                    </div>




                </div>
            </div>
        </div>
    </div>





    <!-- Ankur Debnath-->
    <div class="modal fade" id="AnkurModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690bf2ccfbf732e3c287663_ankur-profile.webp" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Ankur Debnath</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Senior Data Scientist at S & P Global</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Senior Data Scientist, AI researcher, published in Speech, NLP, and Temporal Data Mining.</p>
                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-column justify-content-around">
                        <div class="d-flex flex-row justify-content-around">
                            <div>
                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690bf2caba666ed22f12758_s%26p-logo.webp" alt="" width="87.17px" height="36px" loading="lazy">
                            </div>


                            <div><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690bf2cf8be43f70430bf6f_master-card.webp" alt="" width="87.17px" height="36px" loading="lazy"></div>





                        </div>


                        <div>
                            <p class="what-you-will-learn-p2 mt-4">Indian Institute of Science</p>
                        </div>




                        <div><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690bf2ce753f85e1e455585_ankur-education.webp" alt="" width="87.17px" height="36px" loading="lazy"></div>


                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Top AI Job Roles</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Must-have skills</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                How do Data Scientists Work</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">AI in Industries</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Future of AI</div>
                        </div>



                    </div>




                </div>
            </div>
        </div>
    </div>






    <!-- Tezan Sahu-->
    <div class="modal fade" id="TezanModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b7c2e6c1510bacf7c243_tezan-profile.webp" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Tezan Sahu</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Bing Autosuggest expert</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Bing Autosuggest expert, Amazon #1 best-selling author, and mentor to 100+ aspiring data scientists and software developers.</p>
                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-column justify-content-around">

                        <div>
                            <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b14cdce95af5e33cb196_miscrosoft.webp" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>






                        <div>
                            <p class="what-you-will-learn-p2 mt-4">Alumnus of IIT Bombay
                            </p>
                        </div>




                        <div><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b7c25123d6d445b3b9a1_tezan-education.webp" alt="" width="87.17px" height="36px" loading="lazy"></div>


                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Roadmap to Data Science</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Github Copilot</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Skills to become a Data Scientist</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Building a great portfolio</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Networking & Job Opportunities</div>
                        </div>



                    </div>




                </div>
            </div>
        </div>
    </div>







    <!-- Sandeep Chadda-->
    <div class="modal fade" id="ChaddaModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b14c9edff95c3e779920_sandeep-chandra-profile.webp" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Sandeep Chadda</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Product Manager at Microsoft</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">18+ Years of Experience in product and program management, driving innovation and adoption across diverse industries.</p>
                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-column justify-content-around">

                        <div class="d-flex flex-row justify-content-around">

                            <div>
                                <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b14cdce95af5e33cb196_miscrosoft.webp" alt="" width="87.17px" height="36px" loading="lazy">
                            </div>

                            <div><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b14cd47400f039589d57_infosys.webp" alt="" width="87.17px" height="36px" loading="lazy"></div>

                        </div>



                        <div>
                            <p class="what-you-will-learn-p2 mt-4">Alumnus of IIM Ahmedabad
                            </p>
                        </div>




                        <div><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690b2e8062f8a79b709c477_sandeep-chandra-edu.webp" alt="" width="87.17px" height="36px" loading="lazy"></div>


                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Fundamentals of Product Management</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Becoming a Product Manager</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Most used PM Jargons</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Product Building</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">How to land your dream job</div>
                        </div>



                    </div>




                </div>
            </div>
        </div>
    </div>



    <!-- Johan Stokking-->
    <div class="modal fade" id="JohanModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690abed9231e567792c9ae1_Johan-profile.webp" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Johan Stokking</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">CTO & Co-Founder of The Things Industries</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Expertise in technical strategy, business development,<br /> and early-stage prototyping.</p>
                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-column justify-content-around">



                        <div>
                            <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690abec60199e4d33b98447_Johan-exprince.webp" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <p class="what-you-will-learn-p2 mt-4">Expertise in technical strategy, business development,<br /> and early-stage prototyping.</p>
                        </div>


                        <div>
                            <img src="https://cdn.prod.website-files.com/64362e90abbff481a6d25ce8/6690abec847f34386dafbe25_Johan-education.webp" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">IoT Architecture</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Platforms & Tools</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                IoT Skills and Opportunities</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Future of IoT</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">LoRaWAN</div>
                        </div>



                    </div>




                </div>
            </div>
        </div>
    </div>


    <!-- Shyama Dorbala-->
    <div class="modal fade" id="ShyamaModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/shyama-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Shyama Dorbala</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">ML Engineer at Liftoff Mobiles</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Decoding the Science of Data / Decoding Data Science</p>
                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-row justify-content-around">



                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/google-company-logo.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>




                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/oracle-company-logo.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>




                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/liftoff-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Problem Solving as a ML Engineer</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Life at Google, NVIDIA, and Oracle</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Data Science Vs Machine Learning</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Evolution of Data Science and ML</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Essentials for a Data Science Career</div>
                        </div>



                    </div>




                </div>
            </div>
        </div>
    </div>




    <!--Rahul Garg  -->
    <div class="modal fade" id="RahulModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/rahul-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Rahul Garg</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">The Elite Few Who Cracked GSOC</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">GSOC 101: Understanding the Basics</p>
                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-column justify-content-around">


                        <div>
                            <p class="what-you-will-learn-p2 mt-4">The Elite Few Who Cracked GSOC
                            </p>
                        </div>


                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/google-summer-of-code-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>



                        <div>
                            <p class="what-you-will-learn-p2 mt-4">Student of IIIT Hyderabad
                            </p>
                        </div>

                        <div>
                            <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/iit-hyderabad-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Introduction to Google Summer of Code</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">A Guide to Participating in GSOC</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                AIMGSOC: The Ultimate 12-Week Prep</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Tips for Beginners</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Insights from GSOC Alumnus: Secrets to Success</div>
                        </div>



                    </div>




                </div>
            </div>
        </div>
    </div>



    <!-- Shivay Lamba-->
    <div class="modal fade" id="ShivayModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/sivay-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Shivay Lamba</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">CTO at DarkHorse</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Navigating the World of Open Source : Mentor Insights</p>
                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-column justify-content-around">


                        <div>
                            <p class="what-you-will-learn-p2 mt-4">2 Times GSOC Mentor
                            </p>
                        </div>


                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/google-summer-of-code-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>






                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Inside a GSOC Mentor's Mind</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">GSOC Mentorship: Why It Matters</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Open Source Projects v Internships</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Navigating GSOC Contribution Guidelines</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Crafting Winning GSOC Proposals</div>
                        </div>





                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Essential Skills for GSOC Success</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Strategies to Ace Your GSOC Application</div>
                        </div>



                    </div>




                </div>
            </div>
        </div>
    </div>






    <!-- Nirmal Manoj-->
    <div class="modal fade" id="NirmalModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/nirmal-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Nirmal Manoj</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">The Elite Few Who Cracked GSOC</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">GSOC Essentials: A Step by Step Guide</p>
                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-column justify-content-around">


                        <div>
                            <p class="what-you-will-learn-p2 mt-4">The Elite Few Who Cracked GSOC
                            </p>
                        </div>


                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/google-summer-of-code-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>



                        <div>
                            <p class="what-you-will-learn-p2 mt-4">Student of IIIT Hyderabad
                            </p>
                        </div>



                        <div>
                            <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/iit-hyderabad-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>
                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Decoding GSOC Phases</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Acing your Pre Applications</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                GSOC Prep Pro Tips</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Busting GSOC Myths</div>
                        </div>



                    </div>




                </div>
            </div>
        </div>
    </div>


    <!-- Nikhil VAVS-->
    <div class="modal fade" id="NikhilModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/nikhil-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Nikhil VAVS</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Software Engineer at Uber</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Building for the Future </p>
                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/flipkart-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                        <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/uber-logo.svg" alt="" width="87.17px" height="36px" loading="lazy"></div>


                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">The Journey of a Top Backend Engineer</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Startup vs MNC - Speaker Insights</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                In-Demand Skills for Tech Professionals</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">The Path to Landing Top Tech Jobs</div>
                        </div>



                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Beyond Academics: Internships & Career Growth in Tech</div>
                        </div>







                    </div>




                </div>
            </div>
        </div>
    </div>





    <!-- Priyatham Bollimpalli-->
    <div class="modal fade" id="PriyathamModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/priyatham-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Priyatham Bollimpalli</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Data & Applied Scientist II at Microsoft, Redmond, USA</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Unpacking Data Science </p>
                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-column justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/microsoft-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Alumnus of IIIT Guwahati</p>
                        </div>

                        <div><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/iit-guwahati-logo.svg" alt="" width="87.17px" height="36px" loading="lazy"></div>


                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Personal Journey</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">AI, ML & Deep Learning</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Inside Microsoft's Culture</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Microsoft Project Insights</div>
                        </div>



                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Data Science: Trends & Scope</div>
                        </div>






                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Essential Skills for Data Science</div>
                        </div>







                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">NLP: Scope & Challenges</div>
                        </div>
                    </div>




                </div>
            </div>
        </div>
    </div>






    <!-- Shri Dhana Kishore-->
    <div class="modal fade" id="KishoreModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/dana-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Shri Dhana Kishore</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">IAS MD - HMWSSB</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">4.0 Technologies in Governance </p>
                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-row justify-content-start">
                        <div>
                            <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/national-amblum-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>
                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Impact of Technology in Governance</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Governance 1.0 to 4.0: A Journey</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Challenges to Governance 4.0</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Making an Impact</div>
                        </div>


                    </div>




                </div>
            </div>
        </div>
    </div>




    <!--Hari TN -->
    <div class="modal fade" id="HariModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/hari-tn-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Hari TN</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Head HR, Big Basket</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">The Future of Work: Insights on Tomorrow's Workplace</p>
                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-column justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/big-basket-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <p class="what-you-will-learn-p2 mt-4">Alumnus of IIT Madras, IIM Calcutta</p>
                        </div>

                        <div class="d-flex flex-row justify-content-start">
                            <div>
                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/iit-madras-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                            </div>

                            <div>
                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/iim-calcutta-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                            </div>


                        </div>

                    </div>


                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Impact of Technology in Governance</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Governance 1.0 to 4.0: A Journey</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Challenges to Governance 4.0</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Making an Impact</div>
                        </div>


                    </div>




                </div>
            </div>
        </div>
    </div>




    <!--Girish Akash Yeswanth-->
    <div class="modal fade" id="GirishModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/girish-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Girish Akash Yeswanth</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">VP of Corporate Relations at NxtWave</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Paid Internships 101</p>
                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-column justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/nxtwave-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <p class="what-you-will-learn-p2 mt-4">Alumnus of IIT Kharagpur
                            </p>
                        </div>

                        <div>
                            <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/iit-kharagpur-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Strategies for 2nd-Year Internship</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Internship FAQ's</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Understanding Paid Internships</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Balancing Academics with Internships</div>
                        </div>


                    </div>




                </div>
            </div>
        </div>
    </div>




    <!--Ram Ganesh-->
    <div class="modal fade" id="RamModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/ram-ganesh%3Dpopup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Ram Ganesh</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">CEO of CyberEye</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Cybersecurity Essentials</p>
                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/meta-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/drdo-company-logo.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>




                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/apple-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>



                        <div>
                            <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/6446464e68ab70c904d656ef_Ram%20Ganesh.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>




                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Evolution of Cybersecurity</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Types of Social Engineering</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Common Cyber Frauds</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Exploring Cyber Attacks</div>
                        </div>



                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Staying Safe Onlines</div>
                        </div>





                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Preventing Cyber Attacks</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Cybercrime Reporting</div>
                        </div>




                    </div>




                </div>
            </div>
        </div>
    </div>




    <!--Trivikrama Kothinti-->
    <div class="modal fade" id="TrivikramaModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/trivikram-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Trivikrama Kothinti</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">AI/ML Expert</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">A Glimpse into the Future of Technology</p>
                    <p class="what-you-will-learn-p1 ml-3 mt-2">Alumnus of IIT Delhi (AIR 93)</p>

                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-row justify-content-start">
                        <div>
                            <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/iit-delhi-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Impact of 4.0 Tech on Lifestyle</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Advancements in Healthcare</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Future Trends in Agirculture</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Tips for Career Growth</div>
                        </div>

                    </div>




                </div>
            </div>
        </div>
    </div>



    <!--Rakesh Mishra-->
    <div class="modal fade" id="RakeshModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/rakesh-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Rakesh Mishra</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Co-founder of Uhana (Acquired by VMware)</p>
                        </div>
                    </div>


                    <p class="what-you-will-learn-p2 mt-4">Understanding 5G</p>

                    <div class="what-you-will-learn-Experience">Experience</div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">PhD at Stanford University, B.Tech & M.Tech from IIT Madras</p>

                    <div class="d-flex flex-row justify-content-start">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/stanford-log.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>



                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/iit-madras-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>
                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Introduction to Telecommunication Networks</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Different Generations of Networking Technologies</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Capabilites and Potential of 5G</div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">5G Applications</div>
                        </div>

                    </div>




                </div>
            </div>
        </div>
    </div>


    <!--Deepa Wadhwani-->
    <div class="modal fade" id="DeepaModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/deepa-wadhwani-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Deepa Wadhwani</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Director - Lead Acquisition of ADP</p>
                        </div>
                    </div>

                    <p class="what-you-will-learn-p2 mt-4">The Ultimate Interview Handbook</p>


                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-row justify-content-start">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/adp-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Crafting a Standout Resume</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Excelling in Job Interviews</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Skills vs.College: What Matters More?
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">

                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Strategies for A Progressive Career</div>
                        </div>

                    </div>




                </div>
            </div>
        </div>
    </div>



    <!--Naveen Thontepu-->
    <div class="modal fade" id="NaveenModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/naveen-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>


                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">
                                Naveen Thontepu</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Head of Engineering at <br />SuperK</p>
                        </div>
                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">From Mechanics to Code: A Success Story.</p>


                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/amazon-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/superk-company-logo.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                        <div>
                            <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/6442621e8ea7e709b9849e6e_rapido%201.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Making a Switch From Mechanical to Software</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">The Blue Print of Product Engineering</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Startup vs. MNC: Finding the Right Fit
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Key Skills to Succeed in Product Engineering</div>
                        </div>



                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Future Trends and Technologies</div>
                        </div>

                    </div>




                </div>
            </div>
        </div>
    </div>



    <!--Giridhar Ganapavarapu-->
    <div class="modal fade" id="GiridharModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/giridhar-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">

                                Giridhar Ganapavarapu</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Research Engineer, IBM New York</p>
                        </div>
                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Breaking The Barriers to Success</p>


                    <div class="what-you-will-learn-Experience">Experience</div>
                    <p class="what-you-will-learn-p1 ml-3 mt-2">6 patents, 8 publications</p>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Outstanding technical achievement award 2019, 2020, 2021</p>
                    <div class="d-flex flex-row justify-content-start">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/ibm-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>
                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                From Sattenpally to IBM: The Inspiring Journey</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">The Researcher's Guide to Approaching Problems</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Diving Deep into ML, AI, and Data Science
                            </div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                The Machine Learning Workflow Demystified
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Roadmap to Your Career in Machine Learning</div>
                        </div>



                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Building Coding Skills: A Guide</div>
                        </div>

                    </div>




                </div>
            </div>
        </div>
    </div>


    <!--Shiva Kumar-->
    <div class="modal fade" id="ShivaModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/shiva-kumar-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">

                                Shiva Kumar</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">CTO at Slice</p>
                        </div>
                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Explore The Dynamic Role Of a CTO
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/slice-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/myntra-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/microsoft-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>
                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                A Day In The Life of a CTO</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Work Cultures in MNC's, Unicorn & Young Startups</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Story of Slice and Its Road to Becoming a Unicorn
                            </div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                How to Stand Out as a Fresh Hire
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">How to Build a Learning Community</div>
                        </div>

                    </div>




                </div>
            </div>
        </div>
    </div>



    <!--Architha Nagelli-->
    <div class="modal fade" id="ArchithaModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/archita-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">


                                Architha Nagelli</h6>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Lead Software Engineer, Meesho</p>
                        </div>
                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Cracking the Developer's Code
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/meesho-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/factset-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/amazon-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>
                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Lessons from a Developer's Journey</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">Building Alexa: A Project Experience</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Understanding Application Notifications in Coding
                            </div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Approaching Coding Challenges
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Navigating the Software Development Process</div>
                        </div>





                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Amazon Hiring experience</div>
                        </div>

                    </div>




                </div>
            </div>
        </div>
    </div>





    <!--Govind Goyal-->
    <div class="modal fade" id="GovindModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/govind-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">


                                Govind Goyal</h6>
                        </div>
                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Expert Strategies for GSOC Application Success
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">2 Times GSOC Mentor</p>



                    <div class="d-flex flex-row justify-content-start">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/google-summer-of-code-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                From Contributor to GSOC Mentor : Insights</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                The Dos and Don'ts of GSOC Application</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Mastering Documentation
                            </div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Maintaining Code Consistency in GSOC
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Mentor Tips for building a great profile</div>
                        </div>






                    </div>




                </div>
            </div>
        </div>
    </div>






    <!--Goutam Reddy-->
    <div class="modal fade" id="GoutamModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/goutam-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">


                                Goutam Reddy</h6>



                            <p class="what-you-will-learn-p1 ml-3 mt-2">Platform Security Engineer, Meta USA</p>

                        </div>

                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Exploring Cyber Security
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>

                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/meta-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/microsoft-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>




                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/drdo-company-logo.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>
                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Personal Journey From DRDO to Microsoft</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Tips For Designing a Security System</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Overview of Common Types of Malware
                            </div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Ethics and Tools of the Dark Web
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Understanding Cyber Warfare</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Securities Technology : Future Trends & Opportunities</div>
                        </div>






                    </div>




                </div>
            </div>
        </div>
    </div>





    <!--Ashok Vardhan Viswanadha-->
    <div class="modal fade" id="AshokModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/ashok-vardhan-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">


                                Ashok Vardhan Viswanadha</h6>



                            <p class="what-you-will-learn-p1 ml-3 mt-2">Staff Software Engineer at Google</p>

                        </div>

                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">The Path to Google
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Worked 9+ years & Interviewed 100+ candidates at Google</p>

                    <div class="d-flex flex-row justify-content-start">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/google-company-logo.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                    </div>




                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Google Interview Process : A Guide</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Speaker's Insights and Journey</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Balancing Work and Life
                            </div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Busting Popular Myths
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Tips for accelerating Growth</div>
                        </div>





                    </div>




                </div>
            </div>
        </div>
    </div>




    <!--
Sri Vidya Pranavi-->
    <div class="modal fade" id="PranaviModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/sri-vidhya-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">


                                Sri Vidya Pranavi</h6>



                            <p class="what-you-will-learn-p1 ml-3 mt-2">Machine Learning Scientist at Apple</p>

                        </div>

                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">The Journey to Apple
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-column justify-content-start">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/apple-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>
                        <div>
                            <p class="what-you-will-learn-p1 ml-3 mt-2">Alumnus of IIT Kharagpur, Masters from Carnegie Mellon University</p>
                        </div>

                        <div class="d-flex flex-row justify-content-start">
                            <div>
                                <img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/iit-kharagpur-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                            </div>


                            <div>
                                <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/carnegie-mellon-university-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                            </div>

                        </div>




                        <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                        <div class="mt-4">
                            <div class="d-flex flex-row justify-content-start">
                                <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                                <div class="what-you-will-learn-list-items ">

                                    Life at Apple</div>
                            </div>

                            <div class="d-flex flex-row justify-content-start mt-4">
                                <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                                <div class="what-you-will-learn-list-items ">

                                    Building a Career in ML</div>
                            </div>




                            <div class="d-flex flex-row justify-content-start mt-4">
                                <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                                <div class="what-you-will-learn-list-items ">

                                    AI vs ML: Basics
                                </div>
                            </div>

                            <div class="d-flex flex-row justify-content-start mt-4">
                                <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                                <div class="what-you-will-learn-list-items ">

                                    Building a Profile for Top Universities
                                </div>
                            </div>


                            <div class="d-flex flex-row justify-content-start mt-4">
                                <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                                <div class="what-you-will-learn-list-items ">
                                    Career Options After College: A Guide</div>
                            </div>





                            <div class="d-flex flex-row justify-content-start mt-4">
                                <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                                <div class="what-you-will-learn-list-items ">
                                    A Non-CS Student's Guide to MNC's</div>
                            </div>




                            <div class="d-flex flex-row justify-content-start mt-4">
                                <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                                <div class="what-you-will-learn-list-items ">
                                    Work Culture at Europe vs USA</div>
                            </div>



                        </div>
                    </div>




                </div>
            </div>
        </div>
    </div>




    <!--
Sai Kiran Gorthi-->
    <div class="modal fade" id="SaiModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/sai-kiran-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">


                                Sai Kiran Gorthi</h6>



                            <p class="what-you-will-learn-p1 ml-3 mt-2">An Engineer at google</p>

                        </div>

                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Living a Fulfilling Life in Tech: A Google Engineer's Perspective
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Worked on scaling Google Pay from 0 - 50 Million users

                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/google-company-logo.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/amazon-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                    </div>







                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                Speaker's Journey to Google</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                How to Jumpstart One's Career Early</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Experiences From Building Google Pay
                            </div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                A Glimpse Into the Life of a Backend Engineer at Google
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Practical Tips for Boosting Productivity</div>
                        </div>





                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Insights into Understanding Algorithms and Coding</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Managing Oneself and Finding Balance.</div>
                        </div>



                    </div>
                </div>




            </div>
        </div>
    </div>



    <!--Abhinav Reddy-->
    <div class="modal fade" id="AbhinavModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/abhinav-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">


                                Abhinav Reddy</h6>



                            <p class="what-you-will-learn-p1 ml-3 mt-2">Software Development Engineer at Twitter</p>

                        </div>

                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Fast-Tracking a Tech Career
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/twitter.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/amazon-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/booking-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>



                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/paysafe-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>



                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/cisco-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>



                    </div>







                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                The Twitter Engineer's Roadmap</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Software Engineer's Approach to Problem Solving</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Accelerating Your Student Journey: Tips and Tricks
                            </div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Working at FAANG Companies: Lessons Learned
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Navigating the Open Source Community</div>
                        </div>





                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Building Your Personal Brand</div>
                        </div>







                    </div>
                </div>




            </div>
        </div>
    </div>



    <!--Siva Ghani Reddy-->
    <div class="modal fade" id="SivaModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/siva-ghani-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">


                                Siva Ghani Reddy</h6>



                            <p class="what-you-will-learn-p1 ml-3 mt-2">Senior Product Manager at Microsoft</p>

                        </div>

                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Shaping Ideas Into Successful Products
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-row justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/microsoft-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/mcafee-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/adp-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>





                    </div>







                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                Fundamentals Of Product Management</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                How Ideas are Shaped Into Products</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                Work Culture at Microsoft
                            </div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Microsoft Internships and Opportunities
                            </div>
                        </div>


                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Stratergies for Career Diversification</div>
                        </div>





                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">
                                Advice for Career Building</div>
                        </div>







                    </div>
                </div>




            </div>
        </div>
    </div>




    <!--Shashank Gujjala-->
    <div class="modal fade" id="ShashankModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/shashank-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2">


                                Shashank Gujjala</h6>



                            <p class="what-you-will-learn-p1 ml-3 mt-2">Co-Founder Nxtwave , IIT Bombay</p>

                        </div>

                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Learn The Art of Effective Communication
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>


                    <div class="d-flex flex-column justify-content-around">
                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/nxtwave-company-logo.svg" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>

                        <div>
                            <p class="what-you-will-learn-p1 ml-3 mt-2 text-bold">Alumnus of IIT Bombay
                            </p>
                        </div>


                        <div>
                            <img src="https://cdn.prod.website-files.com/642c0b2b12c402f7d9255170/643a3ddcc9e88904a8eb45bd_logo%20(6)%201.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>




                    </div>







                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                Effective Learning Techniques</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                Guildlines For an Impactful Presentation</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                Ways to Publish and Promote Your Work
                            </div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Blue Print For a Model Presentation
                            </div>
                        </div>







                    </div>
                </div>




            </div>
        </div>
    </div>






    <!--Kalmeshwar  Shingenavar-->
    <div class="modal fade" id="KalmeshwarModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header what-you-will-learn-bg  ">
                    <h3 class="modal-title what-you-will-learn-h3">Meet Your Speaker</h3>
                    <button type="button" class="close text-white" data-dismiss="modal">&times;</button>
                </div>
                <div class="modal-body what-you-will-learn-bg  text-white">
                    <div class="d-flex flex-row justify-content-start">
                        <div class="mr-1"><img src="https://nxtwave.imgix.net/ccbp-website/podcast/rare-collection-of-insider-knowledge/kalmeshwar-popup-pic.png" width="72px" alt="sandeep" loading="lazy"></div>

                        <div>
                            <h6 class="what-you-will-learn-h6 ml-3 mt-2"> Shri Kalmeshwar Shingenavar</h6>



                            <p class="what-you-will-learn-p1 ml-3 mt-2">DCP of Cyberabad, IPS</p>

                        </div>

                    </div>

                    <p class="what-you-will-learn-p1 ml-3 mt-2">Building Bridges: Law Enforcement and Technology
                    </p>


                    <div class="what-you-will-learn-Experience">Experience</div>




                    <div class="d-flex flex-column justify-content-around">


                        <div>
                            <p class="what-you-will-learn-p1 ml-3 mt-2 text-bold">Dy. Comissioner of Police - Crimes, Cyberabad Police, Telangana State Police

                            </p>
                        </div>

                        <div>
                            <img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/cyberabad-police-company-logo.png" alt="" width="87.17px" height="36px" loading="lazy">
                        </div>


                    </div>







                    <div class="what-you-will-learn-list-heading mt-5">What You will Learn</div>



                    <div class="mt-4">
                        <div class="d-flex flex-row justify-content-start">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                The ABC's of Cyber Attacks</div>
                        </div>

                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                Introduction to Cyber Cell and Cyber Crimes Act</div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                Engineers' Role in Securing Cities
                            </div>
                        </div>




                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">

                                Staying Safe Online: Tips for Students
                            </div>
                        </div>







                        <div class="d-flex flex-row justify-content-start mt-4">
                            <div><img src="https://nxtwave-website-media-files.s3.ap-south-1.amazonaws.com/ccbp-website/podcast/rare-collection-of-insider-knowledge/tick-mark.svg" alt="image not found" /></div>
                            <div class="what-you-will-learn-list-items ">


                                Cybersecurity Careers: Opportunities and Impact.
                            </div>
                        </div>



                    </div>
                </div>




            </div>
        </div>
    </div>

</body>

</html>
