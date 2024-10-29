<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Awakening Bangkok</title>
    <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/mind-ar@1.2.5/dist/mindar-image-aframe.prod.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body, html {
            width: 100%;
            height: 100%;
            overflow: hidden;
            font-family: Arial, sans-serif;
        }

        /* หน้าแรก */
        .background {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@0355cfaddfc79ff37235fd0030209907f17fb241/BG.png');
            background-size: cover;
            background-position: center;
            filter: brightness(0.7);
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 3;
            cursor: pointer;
        }

        .logo {
            z-index: 4;
        }

        .logo img {
            max-width: 50%;
            height: auto;
        }

        /* หน้าใหม่ (หน้า 2) */
        .background-new {
            display: none;
            align-items: center;
            justify-content: center;
            background-image: url('https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@1a03e934ffc5bffd9a24a369a8426911be010692/MAIN%20OBJECT.png');
            background-size: cover;
            background-position: center;
            width: 100vw;
            height: 100vh;
            position: fixed;
            top: 0;
            left: 0;
            z-index: 2;
        }

        .logo-new {
            position: absolute;
            top: -2%;
            left: 50%;
            transform: translateX(-50%);
            text-align: center;
            mix-blend-mode: screen;
        }

        .logo-new img {
            width: 350px;
        }

        .sticker, .ar {
            position: absolute;
            transform: translateY(-50%);
            cursor: pointer;
            mix-blend-mode: screen;
            transition: transform 0.3s ease, opacity 0.3s ease;
        }

        .sticker {
            top: 50%;
            left: 17%;
            animation: slideUp 2s ease-in-out forwards;
        }

        .ar {
            top: 31%;
            right: 13%;
            animation: slideDown 2s ease-in-out forwards;
        }

        .sticker img, .ar img {
            width: 150px;
            display: block;
        }

        .expand {
            transform: scale(1.1) translateY(-50%);
            opacity: 0.8;
        }

        /* หน้า Interactive Carousel */
        .container {
            display: none;
            width: 100vw;
            height: 100vh;
            background-image: url('https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@8756dba569289668fcf390e249ce499566e9984a/3/BGstik.png');
            background-size: cover;
            background-position: center;
            flex-direction: column;
            align-items: center;
            position: fixed;
            top: 0;
            left: 0;
            z-index: 1;
        }

        .back-button {
            position: absolute;
            top: 120px;
            left: 45px;
            width: 60px;
            height: 60px;
            background-image: url('https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@8756dba569289668fcf390e249ce499566e9984a/3/Top%20R.png');
            background-size: contain;
            background-repeat: no-repeat;
            cursor: pointer;
        }

        .circle {
            width: 500px;
            height: 500px;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-top: 300px;
        }

        .circle-frame {
            position: absolute;
            top: -100px;
            left: 55px;
            width: 110%;
            height: 110%;
            mix-blend-mode: screen;
            background-image: url('https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@afc076b3e8545f459c51ac346182320b5450ffe6/3/Circle.png');
            background-size: contain;
            background-repeat: no-repeat;
            z-index: 1;
        }

        .circle img {
            border-radius: 50%;
            object-fit: cover;
            position: absolute;
            z-index: 0;
            transition: all 0.3s;
        }

        .arrow-left, .arrow-right {
            width: 80px;
            height: 80px;
            background-size: contain;
            background-repeat: no-repeat;
            cursor: pointer;
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            transition: opacity 0.15s;
        }

        .arrow-left {
            left: 77px;
            top: 730px;
            background-image: url('https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@8756dba569289668fcf390e249ce499566e9984a/3/L.png');
        }

        .arrow-right {
            right: 67px;
            top: 730px;
            background-image: url('https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@8756dba569289668fcf390e249ce499566e9984a/3/R.png');
        }

        .item-name {
            width: 500px;
            height: 150px;
            background-image: url('https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@8756dba569289668fcf390e249ce499566e9984a/3/Frame.png');
            background-size: contain;
            background-repeat: no-repeat;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #ffffff;
            font-size: 1.5em;
            margin-top: -145px;
            text-align: center;
        }
    </style>
</head>
<body>
    <!-- หน้าแรก -->
    <div class="background" id="background" onclick="goToNextPage()">
        <div class="logo">
            <img src="https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@0355cfaddfcf79ff37235fd0030209907f17fb241/AWKENING%20LOGO.png" alt="Awakening Bangkok Logo">
        </div>
    </div>

    <!-- หน้าใหม่ (หน้า 2) -->
    <div class="background-new" id="backgroundNew">
        <div class="logo-new">
            <img src="https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@752723f272394a9899c94d7653819849ebecc3ce/Logo%20กลุ่ม.png" alt="Logo">
        </div>
        <div class="sticker" id="sticker" onclick="showCarousel()">
            <img src="https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@752723f272394a9899c94d7653819849ebecc3ce/STRIKER.png" alt="Sticker Button">
        </div>
        <div class="ar" id="ar" onclick="openARPage()">
            <img src="https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@752723f272394a9899c94d7653819849ebecc3ce/AR.png" alt="AR Button">
        </div>
    </div>

    <!-- หน้า Interactive Carousel -->
    <div class="container" id="carouselContainer">
        <div class="back-button" onclick="goBack()"></div>
        <div class="circle" id="imageContainer">
            <div class="circle-frame"></div>
            <img id="currentImage" src="https://via.placeholder.com/400" alt="Image">
        </div>
        <div class="arrow-left" id="arrowLeft" onclick="changeImage('prev')"></div>
        <div class="arrow-right" id="arrowRight" onclick="changeImage('next')"></div>
        <div class="item-name" id="itemName">Tuk Tuk</div>
    </div>

    <!-- หน้า AR -->
    <div id="arPage" style="display: none;">
        <div class="back-button" onclick="goBackFromAR()"></div>
        <div class="phone-icon" id="phoneIcon"></div>
        <div class="capture-button" onclick="capturePhoto()"></div>
        
        <a-scene mindar-image="imageTargetSrc: https://cdn.jsdelivr.net/gh/hiukim/mind-ar-js@1.2.5/examples/image-tracking/assets/band-example/band.mind;" color-space="sRGB" renderer="colorManagement: true, physicallyCorrectLights" embedded vr-mode-ui="enabled: false" device-orientation-permission-ui="enabled: false">
            <a-assets>
                <a-asset-item id="model" src="https://cdn.jsdelivr.net/gh/hiukim/mind-ar-js@1.2.5/examples/image-tracking/assets/band-example/raccoon/scene.gltf"></a-asset-item>
            </a-assets>
            <a-camera position="0 0 0" look-controls="enabled: false"></a-camera>
            <a-entity mindar-image-target="targetIndex: 0">
                <a-gltf-model src="#model" scale="0.1 0.1 0.1" position="0 -0.5 0" rotation="0 0 0" animation-mixer></a-gltf-model>
            </a-entity>
        </a-scene>
    </div>

    <script>
        function goToNextPage() {
            document.getElementById("background").style.display = "none";
            document.getElementById("backgroundNew").style.display = "flex";
        }

        function showCarousel() {
            document.getElementById("backgroundNew").style.display = "none";
            document.getElementById("carouselContainer").style.display = "flex";
            updateDisplay();
        }

        function goBack() {
            document.getElementById("carouselContainer").style.display = "none";
            document.getElementById("backgroundNew").style.display = "flex";
        }

        function goBackFromAR() {
            document.getElementById("arPage").style.display = "none";
            document.getElementById("backgroundNew").style.display = "flex";
        }

        function openARPage() {
            document.getElementById("backgroundNew").style.display = "none";
            document.getElementById("arPage").style.display = "block";

            // เฟดไอคอนโทรศัพท์หลังจาก 3 วินาที
            setTimeout(() => {
                document.getElementById("phoneIcon").style.opacity = "0";
            }, 3000);
        }

        function capturePhoto() {
            const scene = document.querySelector('a-scene');
            scene.components.screenshot.capture('perspective');
            const screenshotData = scene.components.screenshot.getCanvas('perspective').toDataURL("image/png");

            const link = document.createElement('a');
            link.href = screenshotData;
            link.download = 'screenshot.png';
            link.click();
        }

        function changeImage(direction) {
            currentIndex = direction === 'prev' ? (currentIndex - 1 + items.length) % items.length : (currentIndex + 1) % items.length;
            updateDisplay();
        }

        function updateDisplay() {
            const item = items[currentIndex];
            const imageElement = document.getElementById("currentImage");
            imageElement.src = item.src;
            imageElement.style.width = item.width;
            imageElement.style.height = item.height;
            imageElement.style.top = item.top;
            imageElement.style.left = item.left;
            document.getElementById("itemName").textContent = item.name;
        }

        const items = [
            { src: "https://cdn.jsdelivr.net/gh/juniorkanfwqgwg/AWKECDE321@9f25f410e969edd8cf2a6c25a773008e6b6baaf3/Stickers-2/Untitled_Artwork.png", name: "Item 1", width: "300px", height: "300px", top: "40px", left: "95px" },
            { src: "https://via.placeholder.com/400?text=Image+2", name: "Item 2", width: "400px", height: "400px", top: "0px", left: "10px" },
            { src: "https://via.placeholder.com/400?text=Image+3", name: "Item 3", width: "350px", height: "350px", top: "-20px", left: "-10px" },
            { src: "https://via.placeholder.com/400?text=Image+4", name: "Item 4", width: "380px", height: "380px", top: "30px", left: "15px" },
            { src: "https://via.placeholder.com/400?text=Image+5", name: "Item 5", width: "420px", height: "420px", top: "-10px", left: "5px" }
        ];

        let currentIndex = 0;
    </script>
</body>
</html>
