# Proyect_Penguin

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pingüino</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #e0f7fa;
        }
        .penguin {
            position: relative;
            width: 100px;
            height: 150px;
            background: rgb(255, 169, 241);
            border-radius: 50px;
            margin-top: 20px;
        }
        .penguin::before {
            content: '';
            position: absolute;
            top: 40px;
            left: 10px;
            width: 80px;
            height: 110px;
            background: white;
            border-radius: 200px;
        }
        .penguin::after {
            content: '';
            position: absolute;
            top: 30px;
            left: 35px;
            width: 30px;
            height: 20px;
            background: orange;
            border-radius: 50%;
            z-index: 1;
        }

        .eyes {
            position: absolute;
            top: 20px;
            left: 20px;
            width: 60px;
            height: 30px;
            display: flex;
            justify-content: space-between;
        }
        .eye {
            width: 15px;
            height: 17px;
            background: white;
            border-radius: 50%;
            border: 2px solid rgb(255, 255, 255);
        }

    
        .pupil {
            width: 14px;
            height: 15px;
            background: black;
            border-radius: 40%;
            position: absolute;
            top: 8px;
            left: px;
        }

        .wing {
            position: absolute;
            width: 19px;
            height: 50px;
            background: rgb(241, 161, 228);
            top: 70px;
            border-radius: 50px;
        }

        .wing.left {
            left: -10px;
            transform: rotate(-10deg);
        }

        .wing.right {
            right: -10px;
            transform: rotate(10deg);
        }

    
        .feet {
            position: absolute;
            width: 50px;
            height: 20px;
            background: transparent;
            top: 139px;
            left: 24px;
            display: flex;
            justify-content: space-between;
            
        }

        .foot {
            width: 20px;
            height: 13px;
            background: orange;
            border-radius: 50% 50% 20% 20%;
            
        }


        
    </style>
</head>
<body>
    <div class="penguin">
        <!-- Ojos -->
        <div class="eyes">
            <div class="eye">
                <div class="pupil"></div>
            </div>
            <div class="eye">
                <div class="pupil"></div>
            </div>
        </div>

        <!-- Aletas -->
        <div class="wing left"></div>
        <div class="wing right"></div>

        <!-- Patas -->
        <div class="feet">
            <div class="foot"></div>
            <div class="foot"></div>
        </div>
    </div>

</body>
</html>
