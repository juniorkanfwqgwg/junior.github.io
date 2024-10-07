<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>สแกน QR Code AR</title>
    <!-- A-Frame และ AR.js -->
    <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
    <script src="https://rawgit.com/jeromeetienne/ar.js/1.7.2/aframe/build/aframe-ar.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/110/three.min.js"></script>
    <script src="https://cdn.rawgit.com/mrdoob/three.js/r129/examples/js/loaders/FBXLoader.js"></script>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            overflow: hidden;
            width: 100vw;
            height: 100vh;
        }

        #arView {
            width: 100vw;
            height: 100vh;
            position: relative;
        }

        #arView canvas {
            width: 100% !important;
            height: 100% !important;
        }

        #arView video {
            transform: scaleX(-1); /* กลับด้านแนวนอน */
            width: 100vw;
            height: 100vh;
            object-fit: cover;
        }

        #scanner {
            text-align: center;
            margin-top: 50px;
        }

        button {
            padding: 10px 20px;
            font-size: 18px;
            margin-top: 20px;
            cursor: pointer;
        }
    </style>
</head>
<body>

<div id="scanner">
    <h1>สแกน QR Code AR</h1>
    <p>นำกล้องของคุณสแกน QR Code เพื่อแสดงโมเดล 3D</p>
    <button id="startScan">เริ่มการสแกน</button>
</div>

<div id="arView" style="display:none;">
    <a-scene embedded arjs="sourceType: webcam;" vr-mode-ui="enabled: false">
        <a-marker preset="hiro">
            <a-entity id="fbxModel"></a-entity>
        </a-marker>
        <a-entity camera></a-entity>
    </a-scene>
    <button id="exitAR">ออกจาก AR</button>
</div>

<script>
// ขอสิทธิ์เข้าถึงกล้อง
document.getElementById('startScan').addEventListener('click', () => {
    navigator.mediaDevices.getUserMedia({ video: { facingMode: { ideal: "environment" } } })
    .then((stream) => {
        // สิทธิ์กล้องได้รับการอนุมัติ
        startQRCodeScanner();
    })
    .catch((err) => {
        alert('ไม่สามารถเข้าถึงกล้องได้: ' + err);
    });
});

// ฟังก์ชันแสดง AR หลังจากสแกนสำเร็จ
function startQRCodeScanner() {
    document.getElementById('scanner').style.display = 'none';
    document.getElementById('arView').style.display = 'block';

    var loader = new THREE.FBXLoader();
    loader.load('./Higokumaru.fbx', function(object) {
        var model = document.querySelector('#fbxModel');
        model.setObject3D('mesh', object);
    });
}

// เมื่อคลิกปุ่ม "ออกจาก AR"
document.getElementById('exitAR').addEventListener('click', () => {
    document.getElementById('arView').style.display = 'none';
    document.getElementById('scanner').style.display = 'block';
});
</script>

</body>
</html>


