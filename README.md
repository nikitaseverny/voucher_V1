# voucher_V1
HTML and CSS voucher with out JS
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Renty Cars Booking</title>
    <style>
        /* Основные стили для body */
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            height: 100%;
        }
        /* Стили для контейнера */
        .container {
            width: 100%;
            max-width: 134.45%; /* 800px / 595px * 100 */
            background: white;
            padding: 3.55%; /* 20px / 842px * 100 */
            box-shadow: 0 0 1.19% rgba(0, 0, 0, 0.1); /* 10px / 842px * 100 */
        }
        /* Общие стили для всех секций */
        .header, .info, .pickup-dropoff-container, .content-section {
            width: 100%;
            box-sizing: border-box;
        }
        /* Стили для заголовка */
        .header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 0.24% solid #ddd; /* 2px / 842px * 100 */
            padding-bottom: 1.19%; /* 10px / 842px * 100 */
        }
        .header .right-text {
            text-align: right;
            font-weight: bold;
            margin-right: 7.06%; /* 42px / 595px * 100 */
        }
        .header .center-text {
            text-align: center;
            font-weight: normal;
            flex: 1;
        }
        /* Стили для информационного блока */
        .info {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: #eee;
            padding: 0.59% 1.19%; /* 5px 10px / 842px * 100 */
        }
        .info div {
            flex: 1;
            padding: 0.59%; /* 5px / 842px * 100 */
            display: flex;
            flex-direction: column;
            justify-content: center;
            height: 5.82%; /* 49px / 842px * 100 */
        }
        .info p {
            margin: 0; /* Убираем отступы у параграфов */
            line-height: 2.97; /* Устанавливаем межстрочный интервал */
        }
        .info .supplier {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-end;
            text-align: right;
            height: 5.82%; /* 49px / 842px * 100 */
        }
        /* Стили для блока с информацией о Pick-Up и Drop-Off */
        .pickup-dropoff-container {
            display: flex;
            justify-content: space-between;
            background: #F4A518;
            padding: 1.19%; /* 10px / 842px * 100 */
            margin-top: 2.37%; /* 20px / 842px * 100 */
            font-weight: bold;
            text-align: center;
            border-radius: 0.71%; /* Скругление углов на 6 пикселей */
        }
        .pickup-dropoff-container div {
            flex: 1;
        }
        /* Стили для контейнера с деталями */
        .details-container {
            display: flex;
            justify-content: space-between;
            gap: 1.19%; /* 10px / 842px * 100 */
            margin-top: 0;
            width: 100%;
        }
        .details {
            flex: 1;
            padding: 1.19%; /* 10px / 842px * 100 */
            background: white;
            border: none;
            text-align: left;
        }
        /* Стили для секций с контентом */
        .content-section {
            margin-top: 2.37%; /* 20px / 842px * 100 */
            padding: 1.19%; /* 10px / 842px * 100 */
            background: #F4A518;
            font-weight: bold;
            width: 100%;
            border-radius: 0.71%; /* Скругление углов на 6 пикселей */
        }
        .text-content {
            padding: 1.19%; /* 10px / 842px * 100 */
            background: white;
            border: 0.12% solid #ddd; /* 1px / 842px * 100 */
            width: 100%;
            box-sizing: border-box;
        }
    </style>
    <script>
        // Скрипт для вывода координат элементов в консоль при загрузке страницы
        window.onload = function() {
            let packageText = document.querySelector('.right-text');
            let supplierText = document.querySelector('.supplier');
            if (packageText && supplierText) {
                let packageRect = packageText.getBoundingClientRect();
                let supplierRect = supplierText.getBoundingClientRect();
                console.log('Package: International POA - X:', packageRect.left, 'Y:', packageRect.top);
                console.log('Supplier: Firefly Car Rental - X:', supplierRect.left, 'Y:', supplierRect.top);
            }
        };
    </script>
</head>
<body>
    <!-- Основной контейнер -->
    <div class="container">
        <!-- Заголовок -->
        <div class="header">
            <img src="Group 235.png" alt="Renty Cars Booking" style="max-width: 100%; height: auto;">
            <div class="center-text">Booking number: RC-6992773</div>
            <div class="right-text">Package: <strong>International POA</strong></div>
        </div>
        
        <!-- Информационный блок -->
        <div class="info">
            <div>
                <p>Confirmation number:</p>
                <p>V1-RC-6992773-5C55</p>
            </div>
            <div>
                <p>Main Driver:</p>
                <p>Mr. Ziad Moustafa</p>
            </div>
            <div>
                <p>Supplier:</p>
                <p><img src="firefly_logo.png" style="height: 2.37%; vertical-align: middle; margin-left: 0.84%;"> Firefly Car Rental</p> <!-- 20px / 842px * 100 и 5px / 595px * 100 -->
            </div>
        </div>
        
        <!-- Блок с информацией о Pick-Up и Drop-Off -->
        <div class="pickup-dropoff-container">
            <div>PICK-UP</div>
            <div>DROP-OFF</div>
        </div>
        
        <!-- Контейнер с деталями -->
        <div class="details-container">
            <div class="details">
                <p><strong>14 February 2024, 14:30</strong></p>
                <p>Hotel Hilton Dubai Jumeirah</p>
                <p>Type: Delivery only</p>
                <p>Phone: 009715249988838</p>
            </div>
            <div class="details">
                <p><strong>14 February 2024, 14:30</strong></p>
                <p>Hotel Hilton Dubai Jumeirah</p>
                <p>Type: Delivery only</p>
                <p>Phone: 009715249988838</p>
            </div>
        </div>
        
        <!-- Секция с информацией о машине -->
        <div class="content-section">Car Details</div>
        <div class="text-content">
            <p><strong>Porsche 718 Cabrio</strong></p>
            <p>2 seats, Air Conditioning, Automatic</p>
            <p>Mileage: 250km per rental</p>
        </div>
        
        <!-- Секция с информацией о защите -->
        <div class="content-section">Protection</div>
        <div class="text-content">
            <p>Full Protection Purchased</p>
            <ul>
                <li>Excess charge for theft</li>
                <li>Towing expenses</li>
                <li>Administrative Fees</li>
            </ul>
        </div>
        
        <!-- Секция с информацией об оплате -->
        <div class="content-section">Payment</div>
        <div class="text-content">
            <p>Pay at Pick-up: <strong>151.79 EUR (~268.56 NZD)</strong></p>
            <p>Refundable Security Deposit: <strong>5000.00 NZD</strong></p>
        </div>
    </div>
</body>
</html>
