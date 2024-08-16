<script lang="ts">
    import "$lib/style.scss";
    import { Carousel, Tab } from "bootstrap";
    import { onMount } from "svelte";

    let carousel_elem: HTMLDivElement;

    onMount((): void =>
    {
        new Carousel(carousel_elem,
        {
            interval: 3000
        });
    })
</script>

<div class="mid border-bottom py-3 px-5">
    <a href="/">
        <img src="logo.webp" alt="logo" height="48px" />
    </a>
</div>

<div class="mid pt-5 px-5">
    <p class="big-text fw-semibold gray-800">
        All your online marketing solutions
    </p>
</div>

<div class="right-box-container mt-5">
    <div bind:this={carousel_elem} class="intro-carousel carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img class="intro-image rounded" src="oig-1.webp" alt="oig-1" />
            </div>
            <div class="carousel-item">
                <img class="intro-image rounded" src="oig-2.webp" alt="oig-2" />
            </div>
            <div class="carousel-item">
                <img class="intro-image rounded" src="oig-3.webp" alt="oig-3" />
            </div>
        </div>
    </div>
    <div class="right-box">
        <p class="right-box-text text-white fw-medium mx-3 p-5">
            In the realm of online marketing, brands breathe life through compelling ideas and relevance. The power and sustainability of a brand hinge on its unique concept, shaping a persona that influences thoughts, emotions, and actions. The greater the online relevance, the more profound and impactful the brand's presence becomes.
        </p>
    </div>
</div>

<div class="about-capability-container container mt-5">
    <div class="row">
        <div class="about-capability col">
            <p class="fs-1 fw-semibold gray-800">
                About Us
            </p>
            <p class="fs-5 fw-semibold gray-700">
                BOnline was founded by experienced digital marketing and ad tech professionals who decided to focus on the inclusive and fastest-growing online advertising world
            </p>
            <p class="fs-5 fw-semibold gray-700">
                BOnline ensures expertise in providing online media, online content, online marketing, influencer marketing, and digital PR services
            </p>
        </div>
        <div class="design col">
            <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
                <path fill="#f4821f" d="m 142.89561,55.671734 c 13.09051,25.317914 15.82369,49.916576 8.6311,68.473456 -7.04873,18.70073 -24.02325,31.64739 -46.03257,47.18339 C 83.628666,186.86457 56.72838,205.13375 39.753868,198.66042 22.779357,192.04323 15.874471,160.53969 8.6818813,129.32385 1.6331443,97.964158 -5.7032977,66.60447 6.6679563,41.430406 19.183062,16.112491 51.262012,-3.1636489 78.881556,0.43264612 106.64496,3.8850891 129.94895,30.209967 142.89561,55.671734 Z" />
            </svg>
        </div>
    </div>
</div>

<div class="about-capability-container container mt-5">
    <div class="row">
        <div class="design col">
            <svg viewBox="0 0 240 200" xmlns="http://www.w3.org/2000/svg">
                <path fill="#f4821f" d="M 143.31374,2.3863849 C 155.6345,7.76718 162.88201,22.943783 170.41942,37.29257 c 7.39246,14.348788 15.07481,28.007729 21.45262,45.115902 6.52275,17.108164 11.74096,37.665558 4.9283,53.256078 -6.81265,15.45253 -25.51122,25.80022 -44.35474,37.80353 -18.84352,11.86535 -37.54208,25.52429 -56.965406,26.49007 -19.42332,0.82781 -39.281485,-10.76159 -57.980052,-22.7649 C 18.946525,165.05197 1.6974594,152.63474 0.10300842,136.21642 -1.3464936,119.66012 12.858619,99.240698 20.251076,82.960348 27.788483,66.54202 28.658184,54.40074 32.861737,42.397428 37.065291,30.394114 44.747648,18.52877 55.763858,12.596098 66.925014,6.6634272 81.564984,6.5254582 97.509494,4.1799826 113.45402,1.834508 130.99298,-2.8564414 143.31374,2.3863849 Z" />
            </svg>
        </div>
        <div class="about-capability col">
            <p class="fs-1 fw-semibold gray-800">
                Capabilities
            </p>
            <p class="fs-5 fw-semibold gray-700">
                We work with brands to identify their online marketing goals and opportunities tailored to their requirements and objectives
            </p>
            <p class="fs-5 fw-semibold gray-700">
                At BOnline we offer research to identify an effective way to communicate the online communications
            </p>
            <p class="fs-5 fw-semibold gray-700">
                At BOnline we create online contents that helps brands to achieve effective engagements
            </p>
            <p class="fs-5 fw-semibold gray-700">
                BOnline is here to help clients to achieve long-term ambitions of their business through efficient online marketing solutions
            </p>
        </div>
    </div>
</div>

<div class="tab-info my-5">
    <!-- svelte-ignore a11y-invalid-attribute -->
    <div class="tab-options nav nav-pills mb-3">
        <button class="nav-link rounded-pill active" data-bs-toggle="pill" data-bs-target="#tab-1">Online Marketing</button>
        <button class="nav-link rounded-pill" data-bs-toggle="pill" data-bs-target="#tab-2">Platform Strategy</button>
        <button class="nav-link rounded-pill" data-bs-toggle="pill" data-bs-target="#tab-3">Content Solution</button>
    </div>
    <div class="tab-content">
        <div class="tab-pane fade show active" id="tab-1" role="tabpanel">
            <div class="tab-item">
                <img class="tab-image rounded me-4" src="oig-4.webp" alt="oig-4" />
                <p class="fs-4 fw-semibold gray-700 mb-0">
                    We run Online Advertising Campaigns on selected channels based on business requirements from increasing Online TOMA to driving conversion
                </p>
            </div>
        </div>
        <div class="tab-pane fade" id="tab-2" role="tabpanel">
            <div class="tab-item">
                <p class="fs-4 fw-semibold gray-700 me-4 mb-0">
                    Omnichannel Online Marketing Strategy and Management A comprehensive solution for all online marketing needs.
                </p>
                <img class="tab-image rounded" src="oig-5.webp" alt="oig-5" />
            </div>
        </div>
        <div class="tab-pane fade" id="tab-3" role="tabpanel">
            <div class="tab-item">
                <img class="tab-image rounded me-4" src="oig-6.webp" alt="oig-6" />
                <p class="fs-4 fw-semibold gray-700 mb-0">
                    Human centric designs to drive effective results for online marketing.
                </p>
            </div>
        </div>
    </div>
</div>

<div class="mid border-top py-3 px-5">
    <p class="fs-5 fw-semibold gray-800">Get in Touch</p>
    <div class="info">
        <div class="contact-info">
            <p class="fs-6 fw-semibold gray-700 me-3">
                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-telephone-fill" viewBox="0 0 16 16">
                    <path fill-rule="evenodd" d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.68.68 0 0 0 .178.643l2.457 2.457a.68.68 0 0 0 .644.178l2.189-.547a1.75 1.75 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.6 18.6 0 0 1-7.01-4.42 18.6 18.6 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877z"/>
                </svg>
                +8801832543556
            </p>
            <p class="fs-6 fw-semibold gray-700">
                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-envelope-fill" viewBox="0 0 16 16">
                    <path d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414zM0 4.697v7.104l5.803-3.558zM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586zm3.436-.586L16 11.801V4.697z"/>
                </svg>
                commercial@bonline.digital
            </p>
        </div>
        <a class="link-underline link-underline-opacity-0 d-flex align-items-center" href="https://www.facebook.com/bonline.digital.bd/" style="color: #3B5998;">
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-facebook me-1" viewBox="0 0 16 16">
                <path d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951"/>
            </svg>
            <span class="my-auto">Bonline.Digital</span>
        </a>
    </div>
</div>

<style>
    .mid
    {
        width: 1200px;
        max-width: 100%;
        margin-left: auto;
        margin-right: auto;
    }
    .big-text
    {
        max-width: 600px;
        font-size: 450%;
    }
    .right-box-container
    {
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .intro-carousel
    {
        max-width: 400px;
        margin-left: auto;
        margin-right: auto;
    }
    .intro-image
    {
        max-width: 400px;
    }
    .right-box
    {
        background-color: #f4821f;
        min-width: 50%;
        border-top-left-radius: 32px;
        border-bottom-left-radius: 32px;
    }
    .right-box-text
    {
        font-size: 1.5em;
        max-width: 700px;
    }
    .about-capability-container
    {
        width: 1200px;
        max-width: 90%;
        margin-left: auto;
        margin-right: auto;
    }
    .about-capability
    {
        min-width: 70%;
    }
    .design
    {
        display: flex;
    }
    .tab-item
    {
        display: flex;
    }
    .tab-info
    {
        width: 800px;
        max-width: 90%;
        margin-left: auto;
        margin-right: auto;
    }
    .tab-options
    {
        display: flex;
        justify-content: center;
    }
    .tab-image
    {
        max-height: 150px;
    }
    .info
    {
        display: flex;
        justify-content: space-between;
    }
    .contact-info
    {
        display: flex;
    }
    @media (max-width: 1199px)
    {
        .right-box-container
        {
            display: inline;
            align-items: end;
        }
        .intro-carousel
        {
            margin-right: 2em;
            margin-bottom: 2em;
        }
        .info
        {
            display: block;
        }
        .contact-info
        {
            display: block;
        }
    }
    @media (max-width: 767px)
    {
        .big-text
        {
            font-size: 350%;
        }
        .intro-carousel
        {
            width: 90%;
            margin-right: auto;
            margin-right: auto;
            margin-bottom: 2em;
        }
        .intro-image
        {
            width: 100%;
        }
        .design
        {
            display: none;
        }
    }
    @media (max-width: 450px)
    {
        .big-text
        {
            font-size: 250%;
        }
        .tab-item
        {
            display: block;
        }
        .tab-image
        {   
            margin-top: 1em;
            margin-bottom: 1em;
        }
    }
</style>
