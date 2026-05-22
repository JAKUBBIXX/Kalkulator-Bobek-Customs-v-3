<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GTA Vehicle Price Viewer</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <!-- Header -->
        <div class="header">
            <h1 class="title">WYBIERZ MODEL</h1>
            <div class="search-container">
                <input type="text" id="searchInput" placeholder="Wyszukaj pojazd..." class="search-box">
            </div>
        </div>

        <!-- Main Content Area -->
        <div class="main-content">
            <!-- Vehicle List -->
            <div class="vehicle-list" id="vehicleList">
                <!-- Vehicles will be populated here -->
            </div>

            <!-- Details Panel -->
            <div class="details-panel" id="detailsPanel">
                <button class="close-btn" onclick="closeDetails()">×</button>
                <div class="details-content">
                    <h2 id="vehicleName" class="vehicle-title"></h2>
                    <div class="price-display">
                        <span class="currency">$</span>
                        <span id="totalPrice" class="total-price">0</span>
                    </div>
                    <table class="price-table">
                        <thead>
                            <tr>
                                <th>KOMPONENT</th>
                                <th>CENA</th>
                            </tr>
                        </thead>
                        <tbody id="priceDetails">
                            <!-- Price details will be populated here -->
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>

    <script src="data.js"></script>
    <script src="script.js"></script>
</body>
</html>
