<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
    <meta name="theme-color" content="#ff6a00">
    <title>Daraz Pro Max - মোবাইলের জন্য সেরা</title>
    <link rel="manifest" href="data:application/manifest+json,{
        'name': 'Daraz Pro Max',
        'short_name': 'Daraz',
        'start_url': '.',
        'display': 'standalone',
        'background_color': '#ff6a00',
        'theme_color': '#ff6a00',
        'icons': [{'src': 'data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTkyIiBoZWlnaHQ9IjE5MiIgdmlld0JveD0iMCAwIDE5MiAxOTIiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxjaXJjbGUgY3g9Ijk2IiBjeT0iOTYiIHI9Ijk2IiBmaWxsPSIjRkY2QTAwIi8+CjxwYXRoIGQ9Ik0xMjAgMTI1QzEyMCAxMzEuMjUgMTE0LjI1IDEzNSAxMDggMTM1SDg0Qzc3Ljc1IDEzNSA3MiAxMzEuMjUgNzIgMTI1VjEwNUM3MiA4OC43NSA3Ny43NSA4NCA4NCA4NEgxMDhDMTI0LjI1IDg0IDEyMCA4OC43NSAxMjAgOTVWMTI1Wk0xMjAgNzBDMTIwIDc2LjI1IDExNC4yNSA3MiAxMDggNzJINzhDMc4uNzUgNzIgNzIgNzYuMjUgNzIgNzBWNzBIMTIwVjcwWiIgZmlsbD0id2hpdGUiLz4KPC9zdmc+', 'sizes': '192x192', 'type': 'image/svg+xml'}]
    }">
    <link rel="apple-touch-icon" href="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTkyIiBoZWlnaHQ9IjE5MiIgdmlld0JveD0iMCAwIDE5MiAxOTIiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxjaXJjbGUgY3g9Ijk2IiBjeT0iOTYiIHI9Ijk2IiBmaWxsPSIjRkY2QTAwIi8+CjxwYXRoIGQ9Ik0xMjAgMTI1QzEyMCAxMzEuMjUgMTE0LjI1IDEzNSAxMDggMTM1SDg0Qzc3Ljc1IDEzNSA3MiAxMzEuMjUgNzIgMTI1VjEwNUM3MiA4OC43NSA3Ny43NSA4NCA4NCA4NEgxMDhDMTI0LjI1IDg0IDEyMCA4OC43NSAxMjAgOTVWMTI1Wk0xMjAgNzBDMTIwIDc2LjI1IDExNC4yNSA3MiAxMDggNzJINzhDMc8uNzUgNzIgNzIgNzYuMjUgNzIgNzBWNzBIMTIwVjcwWiIgZmlsbD0id2hpdGUiLz4KPC9zdmc+">
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Bengali:wght@400;500;600;700&family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        :root {
            --primary: #ff6a00;
            --primary-dark: #e55a00;
            --secondary: #ff8c42;
            --accent: #00b894;
            --dark: #1a1a1a;
            --light: #f8f9fa;
            --white: #ffffff;
            --shadow: 0 8px 32px rgba(0,0,0,0.1);
            --shadow-lg: 0 20px 40px rgba(0,0,0,0.15);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        html {
            scroll-behavior: smooth;
            font-size: 16px;
            overflow-x: hidden;
        }

        body {
            font-family: 'Noto Sans Bengali', 'Poppins', sans-serif;
            line-height: 1.6;
            background: var(--light);
            color: var(--dark);
            overscroll-behavior: none;
            touch-action: manipulation;
        }

        /* ===== LOADING SCREEN ===== */
        .splash-screen {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100vh;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            z-index: 9999;
            transition: opacity 0.6s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .splash-screen.hidden {
            opacity: 0;
            pointer-events: none;
        }

        .splash-logo {
            font-size: clamp(2rem, 8vw, 3.5rem);
            font-weight: 700;
            color: white;
            margin-bottom: 2rem;
            text-shadow: 0 4px 20px rgba(0,0,0,0.3);
            animation: pulse 2s infinite;
        }

        .splash-spinner {
            width: 60px;
            height: 60px;
            border: 4px solid rgba(255,255,255,0.2);
            border-top: 4px solid white;
            border-radius: 50%;
            animation: spin 1s linear infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        @keyframes spin {
            to { transform: rotate(360deg); }
        }

        /* ===== BOTTOM NAVIGATION ===== */
        .bottom-nav {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            background: var(--white);
            display: flex;
            justify-content: space-around;
            padding: 0.8rem 0;
            box-shadow: var(--shadow-lg);
            z-index: 1000;
            backdrop-filter: blur(20px);
        }

        .nav-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 0.3rem;
            color: #666;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 12px;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            flex: 1;
        }

        .nav-item.active,
        .nav-item:active {
            color: var(--primary);
            background: rgba(255, 106, 0, 0.1);
            transform: translateY(-2px);
        }

        .nav-icon {
            font-size: 1.4rem;
        }

        .nav-label {
            font-size: 0.7rem;
            font-weight: 500;
        }

        /* ===== MAIN CONTENT ===== */
        .main-content {
            padding-bottom: 90px;
            min-height: 100vh;
        }

        .page {
            display: none;
            animation: slideInUp 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .page.active {
            display: block;
        }

        @keyframes slideInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* ===== SEARCH BAR ===== */
        .search-header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            padding: 1.5rem 1.5rem 1rem;
            position: sticky;
            top: 0;
            z-index: 900;
        }

        .search-container {
            position: relative;
            background: rgba(255,255,255,0.95);
            border-radius: 25px;
            padding: 1rem 1.5rem 1rem 4rem;
            box-shadow: var(--shadow);
            backdrop-filter: blur(20px);
        }

        .search-input {
            width: 100%;
            border: none;
            background: none;
            font-size: 1rem;
            outline: none;
            color: var(--dark);
        }

        .search-icon {
            position: absolute;
            left: 1.5rem;
            top: 50%;
            transform: translateY(-50%);
            color: var(--primary);
            font-size: 1.2rem;
        }

        .search-suggestions {
            position: absolute;
            top: 100%;
            left: 0;
            right: 0;
            background: white;
            border-radius: 0 0 20px 20px;
            max-height: 200px;
            overflow-y: auto;
            box-shadow: var(--shadow-lg);
            display: none;
            z-index: 1000;
        }

        .suggestion-item {
            padding: 1rem 1.5rem;
            border-bottom: 1px solid #f0f0f0;
            cursor: pointer;
            transition: background 0.2s ease;
        }

        .suggestion-item:hover,
        .suggestion-item.active {
            background: rgba(255, 106, 0, 0.1);
        }

        /* ===== FLASH SALE BANNER ===== */
        .flash-banner {
            background: linear-gradient(135deg, #ff4757, #ff6b7a);
            color: white;
            padding: 1rem;
            margin: 1.5rem;
            border-radius: 20px;
            display: flex;
            align-items: center;
            gap: 1rem;
            animation: slideInLeft 0.6s ease;
            cursor: pointer;
        }

        @keyframes slideInLeft {
            from { transform: translateX(-100%); opacity: 0; }
            to { transform: translateX(0); opacity: 1; }
        }

        .flash-icon { font-size: 1.5rem; }
        .flash-timer {
            background: rgba(0,0,0,0.2);
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-weight: 600;
            font-size: 0.9rem;
        }

        /* ===== CATEGORIES GRID ===== */
        .categories-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(110px, 1fr));
            gap: 1rem;
            padding: 1.5rem;
        }

        .category-card {
            background: white;
            border-radius: 20px;
            padding: 1.5rem 1rem;
            text-align: center;
            box-shadow: var(--shadow);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            cursor: pointer;
            aspect-ratio: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        .category-card:hover,
        .category-card.active {
            transform: translateY(-8px) scale(1.05);
            box-shadow: var(--shadow-lg);
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
        }

        .category-icon {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        .category-name {
            font-size: 0.85rem;
            font-weight: 600;
        }

        /* ===== PRODUCTS LIST ===== */
        .products-list {
            padding: 1rem;
        }

        .product-card {
            background: white;
            border-radius: 20px;
            margin-bottom: 1.5rem;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            display: flex;
        }

        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-lg);
        }

        .product-image {
            width: 120px;
            height: 120px;
            background: linear-gradient(135deg, #f8f9fa, #e9ecef);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.5rem;
            flex-shrink: 0;
        }

        .product-info {
            padding: 1.2rem;
            flex: 1;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .product-title {
            font-size: 1rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
            line-height: 1.3;
        }

        .product-price-row {
            display: flex;
            align-items: baseline;
            gap: 0.5rem;
            margin-bottom: 0.8rem;
        }

        .price {
            font-size: 1.3rem;
            font-weight: 700;
            color: var(--primary);
        }

        .old-price {
            text-decoration: line-through;
            color: #999;
            font-size: 0.9rem;
        }

        .rating-row {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            margin-bottom: 1rem;
        }

        .stars {
            color: #ffd700;
            font-size: 0.9rem;
        }

        .add-cart-btn {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            border: none;
            padding: 0.8rem 1.5rem;
            border-radius: 25px;
            font-weight: 600;
            cursor: pointer;
            align-self: flex-start;
            transition: all 0.3s ease;
            font-size: 0.9rem;
        }

        .add-cart-btn:active {
            transform: scale(0.98);
        }

        /* ===== FLOATING ACTION BUTTON ===== */
        .fab {
            position: fixed;
            bottom: 90px;
            right: 20px;
            width: 60px;
            height: 60px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            border: none;
            border-radius: 50%;
            color: white;
            font-size: 1.5rem;
            box-shadow: var(--shadow-lg);
            cursor: pointer;
            z-index: 1001;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .fab:hover {
            transform: scale(1.1);
        }

        /* ===== MODALS ===== */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.6);
            display: none;
            justify-content: center;
            align-items: center;
            z-index: 2000;
            backdrop-filter: blur(10px);
        }

        .modal-overlay.active {
            display: flex;
        }

        .cart-modal {
            background: white;
            width: 95%;
            max-width: 500px;
            max-height: 85vh;
            border-radius: 25px;
            overflow: hidden;
            transform: scale(0.8) translateY(30px);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .modal-overlay.active .cart-modal {
            transform: scale(1) translateY(0);
        }

        .modal-header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 1.5rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .modal-title {
            font-size: 1.3rem;
            font-weight: 700;
        }

        .close-modal {
            background: rgba(255,255,255,0.2);
            border: none;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            color: white;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .cart-item {
            display: flex;
            padding: 1.2rem;
            border-bottom: 1px solid #f0f0f0;
            align-items: center;
            gap: 1rem;
        }

        .cart-item-image {
            width: 70px;
            height: 70px;
            border-radius: 15px;
            font-size: 2rem;
            display: flex;
            align-items: center;
            justify-content: center;
            background: #f8f9fa;
        }

        .quantity-selector {
            display: flex;
            align-items: center;
            gap: 0.8rem;
            background: #f8f9fa;
            padding: 0.5rem;
            border-radius: 25px;
        }

        .qty-btn {
            width: 35px;
            height: 35px;
            border: 2px solid #ddd;
            background: white;
            border-radius: 50%;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 600;
            transition: all 0.2s ease;
        }

        .qty-btn:active {
            background: var(--primary);
            color: white;
            border-color: var(--primary);
        }

        .remove-btn {
            background: #ff4757;
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.8rem;
            cursor: pointer;
        }

        .checkout-section {
            padding: 1.5rem;
            background: linear-gradient(135deg, #f8f9fa, white);
        }

        .total-row {
            display: flex;
            justify-content: space-between;
            font-size: 1.2rem;
            font-weight: 700;
            margin-bottom: 1.5rem;
        }

        .checkout-btn {
            width: 100%;
            background: linear-gradient(135deg, var(--accent), #00cec9);
            color: white;
            border: none;
            padding: 1.2rem;
            border-radius: 20px;
            font-size: 1.1rem;
            font-weight: 700;
            cursor: pointer;
        }

        /* ===== NOTIFICATION ===== */
        .toast {
            position: fixed;
            top: 20px;
            right: 20px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 1rem 1.5rem;
            border-radius: 20px;
            box-shadow: var(--shadow-lg);
            transform: translateX(100%);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            z-index: 3000;
            max-width: 90vw;
        }

        .toast.show {
            transform: translateX(0);
        }

        .toast.success {
            background: linear-gradient(135deg, var(--accent), #00cec9);
        }

        .toast.error {
            background: linear-gradient(135deg, #ff4757, #ff6b7a);
        }

        /* ===== RESPONSIVE & MOBILE OPTIMIZATIONS ===== */
        @media (max-width: 480px) {
            html { font-size: 15px; }
            
            .search-header {
                padding: 1rem 1rem 0.8rem;
            }
            
            .categories-grid {
                grid-template-columns: repeat(4, 1fr);
                gap: 0.8rem;
                padding: 1rem;
            }
            
            .product-card {
                margin-bottom: 1rem;
            }
        }

        /* ===== PWA INSTALL PROMPT ===== */
        .install-prompt {
            position: fixed;
            bottom: 110px;
            left: 20px;
            right: 20px;
            background: white;
            padding: 1.2rem;
            border-radius: 20px;
            box-shadow: var(--shadow-lg);
            display: none;
            z-index: 2001;
        }

        /* ===== CUSTOM SCROLLBAR ===== */
        ::-webkit-scrollbar {
            width: 4px;
        }

        ::-webkit-scrollbar-track {
            background: transparent;
        }

        ::-webkit-scrollbar-thumb {
            background: var(--primary);
            border-radius: 2px;
        }
    </style>
</head>

<body>
    <!-- SPLASH SCREEN -->
    <div class="splash-screen" id="splash">
        <div class="splash-logo">
            🛒 Daraz Pro Max
        </div>
        <div class="splash-spinner"></div>
    </div>

    <!-- MAIN CONTENT -->
    <div class="main-content">
        <!-- HOME PAGE -->
        <div id="home" class="page active">
            <!-- SEARCH BAR -->
            <div class="search-header">
                <div class="search-container">
                    <i class="fas fa-search search-icon"></i>
                    <input type="text" class="search-input" id="searchInput" placeholder="অনুসন্ধান করুন...">
                    <div class="search-suggestions" id="searchSuggestions"></div>
                </div>
            </div>

            <!-- FLASH SALE -->
            <div class="flash-banner" onclick="scrollToProducts()">
                <i class="fas fa-bolt flash-icon"></i>
                <div>
                    <strong>🔥 ফ্ল্যাশ সেল!</strong><br>
                    <small>৭০% পর্যন্ত ছাড়</small>
                </div>
                <div class="flash-timer" id="flashTimer">02:47:23</div>
            </div>

            <!-- CATEGORIES -->
            <div class="categories-grid" id="categoriesGrid">
                <!-- Categories will be populated by JS -->
            </div>

            <!-- PRODUCTS -->
            <div class="products-list" id="productsList">
                <!-- Products will be populated by JS -->
            </div>
        </div>

        <!-- CART PAGE -->
        <div id="cart" class="page">
            <div style="padding: 1.5rem; text-align: center; padding-top: 3rem;">
                <i class="fas fa-shopping-cart" style="font-size: 4rem; color: #ddd; margin-bottom: 1rem;"></i>
                <h3>কার্ট পেজ</h3>
                <p>কার্ট আইটেমগুলো এখানে দেখাবে</p>
            </div>
        </div>

        <!-- PROFILE PAGE -->
        <div id="profile" class="page">
            <div style="padding: 2rem; text-align: center;">
                <i class="fas fa-user-circle" style="font-size: 6rem; color: #ddd; margin-bottom: 1rem;"></i>
                <h2>প্রোফাইল</h2>
                <p>আপনার প্রোফাইল সেটিংস</p>
            </div>
        </div>
    </div>

    <!-- BOTTOM NAVIGATION -->
    <nav class="bottom-nav">
        <a href="#" class="nav-item active" data-page="home">
            <i class="fas fa-home nav-icon"></i>
            <span class="nav-label">হোম</span>
        </a>
        <a href="#" class="nav-item" data-page="cart">
            <i class="fas fa-shopping-cart nav-icon"></i>
            <span class="nav-label">কার্ট</span>
            <span class="cart-badge" id="cartBadge">0</span>
        </a>
        <a href="#" class="nav-item" data-page="profile">
            <i class="fas fa-user nav-icon"></i>
            <span class="nav-label">প্রোফাইল</span>
        </a>
    </nav>

    <!-- FAB -->
    <button class="fab" onclick="openCartModal()" title="কার্ট খোলুন">
        <i class="fas fa-shopping-cart"></i>
    </button>

    <!-- CART MODAL -->
    <div class="modal-overlay" id="cartModal">
        <div class="cart-modal">
            <div class="modal-header">
                <div class="modal-title">
                    <i class="fas fa-shopping-cart"></i>
                    শপিং কার্ট
                </div>
                <button class="close-modal" onclick="closeCartModal()">
                    <i class="fas fa-times"></i>
                </button>
            </div>
            <div id="modalCartItems" style="max-height: 400px; overflow-y: auto;"></div>
            <div class="checkout-section">
                <div class="total-row">
                    <span>মোট:</span>
                    <span class="total-price" id="modalTotal">৳ ০</span>
                </div>
                <button class="checkout-btn" onclick="completeOrder()">
                    <i class="fas fa-credit-card"></i> চেকআউট করুন
                </button>
            </div>
        </div>
    </div>

    <!-- TOAST NOTIFICATION -->
    <div class="toast" id="toast"></div>

    <!-- PWA INSTALL PROMPT -->
    <div class="install-prompt" id="installPrompt">
        <div style="display: flex; align-items: center; gap: 1rem;">
            <i class="fas fa-download" style="color: var(--primary); font-size: 1.5rem;"></i>
            <div>
                <strong>Daraz Pro Max ইনস্টল করুন</strong>
                <br><small>হোম স্ক্রিনে অ্যাড করুন</small>
            </div>
        </div>
        <div style="display: flex; gap: 0.5rem; margin-top: 1rem;">
            <button onclick="installPWA()" style="flex: 1; padding: 0.8rem; background: var(--primary); color: white; border: none; border-radius: 12px; font-weight: 600;">ইনস্টল</button>
            <button onclick="hideInstallPrompt()" style="flex: 1; padding: 0.8rem; background: #f0f0f0; border: none; border-radius: 12px;">পরে</button>
        </div>
    </div>

    <script>
        // ===== DATA =====
        const categories = [
            { name: 'সব', icon: '🏠', value: 'all' },
            { name: 'ইলেকট্রনিক্স', icon: '📱', value: 'electronics' },
            { name: 'ফ্যাশন', icon: '👗', value: 'fashion' },
            { name: 'হোম', icon: '🏠', value: 'home' },
            { name: 'স্পোর্টস', icon: '⚽', value: 'sports' },
            { name: 'বই', icon: '📚', value: 'books' }
        ];

        const products = [
            {id:1, name:"iPhone 16 Pro Max", price:129999, oldPrice:149999, category:"electronics", rating:4.9, image:"📱", badge:"নতুন"},
            {id:2, name:"MacBook Pro M3", price:219999, oldPrice:249999, category:"electronics", rating:4.8, image:"💻"},
            {id:3, name:"AirPods Pro 2", price:24999, oldPrice:29999, category:"electronics", rating:4.7, image:"🎧"},
            {id:4, name:"Sony Camera", price:189999, category:"electronics", rating:4.9, image:"📷"},
            {id:5, name:"Apple Watch", price:79999, category:"electronics", rating:4.8, image:"⌚"},
            {id:6, name:"Nike Air Max", price:12999, oldPrice:15999, category:"fashion", rating:4.6, image:"👟"},
            {id:7, name:"Gucci Bag", price:89999, category:"fashion", rating:4.7, image:"👜"},
            {id:8, name:"Sofa Set", price:129999, category:"home", rating:4.7, image:"🛋️"},
            {id:9, name:"Smart TV 65\"", price:89999, category:"electronics", rating:4.8, image:"📺"},
            {id:10, name:"Yoga Mat", price:4999, category:"sports", rating:4.7, image:"🧘"},
            {id:11, name:"Protein Powder", price:3999, category:"sports", rating:4.6, image:"💪"},
            {id:12, name:"Dining Table", price:59999, category:"home", rating:4.6, image:"🍽️"}
        ];

        let cart = JSON.parse(localStorage.getItem('daraz_cart')) || [];
        let currentProducts = [...products];
        let searchSuggestions = [];
        let deferredPrompt;

        // ===== INIT =====
        document.addEventListener('DOMContentLoaded', initApp);

        function initApp() {
            hideSplash();
            renderCategories();
            renderProducts();
            updateCartBadge();
            initEventListeners();
            startFlashTimer();
            requestPWAInstall();
            
            // Service Worker for PWA
            if ('serviceWorker' in navigator) {
                navigator.serviceWorker.register('data:text/javascript;base64,' + btoa(`
                    self.addEventListener('install', e => {
                        self.skipWaiting();
                    });
                    self.addEventListener('activate', e => {
                        self.clients.claim();
                    });
                    self.addEventListener('fetch', e => {
                        e.respondWith(fetch(e.request));
                    });
                `));
            }
        }

        // ===== UI FUNCTIONS =====
        function hideSplash() {
            setTimeout(() => {
                document.getElementById('splash').classList.add('hidden');
            }, 2000);
        }

        function showToast(message, type = 'success') {
            const toast = document.getElementById('toast');
            toast.textContent = message;
            toast.className = `toast ${type} show`;
            setTimeout(() => toast.classList.remove('show'), 3000);
        }

        function switchPage(pageId) {
            document.querySelectorAll('.page').forEach(page => page.classList.remove('active'));
            document.querySelectorAll('.nav-item').forEach(item => item.classList.remove('active'));
            
            document.getElementById(pageId).classList.add('active');
            document.querySelector(`[data-page="${pageId}"]`).classList.add('active');
        }

        // ===== NAVIGATION =====
        function initEventListeners() {
            // Bottom nav
            document.querySelectorAll('.nav-item').forEach(item => {
                item.addEventListener('click', (e) => {
                    e.preventDefault();
                    switchPage(item.dataset.page);
                });
            });

            // Search
            const searchInput = document.getElementById('searchInput');
            searchInput.addEventListener('input', handleSearch);
            searchInput.addEventListener('focus', showSuggestions);
            searchInput.addEventListener('blur', hideSuggestions);

            // Category clicks
            document.getElementById('categoriesGrid').addEventListener('click', handleCategoryClick);

            // Prevent zoom on iOS
            document.addEventListener('gesturestart', function (e) { e.preventDefault(); });
            document.addEventListener('touchmove', function (e) { e.preventDefault(); }, { passive: false });
        }

        // ===== SEARCH & FILTER =====
        function handleSearch(e) {
            const query = e.target.value.toLowerCase();
            searchSuggestions = products.filter(p => 
                p.name.toLowerCase().includes(query) && query.length > 0
            ).slice(0, 4);

            renderSearchSuggestions();
            filterProducts(query);
        }

        function showSuggestions() {
            if (searchSuggestions.length > 0) {
                document.getElementById('searchSuggestions').style.display = 'block';
            }
        }

        function hideSuggestions() {
            setTimeout(() => {
                document.getElementById('searchSuggestions').style.display = 'none';
            }, 200);
        }

        function renderSearchSuggestions() {
            const suggestionsEl = document.getElementById('searchSuggestions');
            if (searchSuggestions.length === 0) {
                suggestionsEl.style.display = 'none';
                return;
            }

            suggestionsEl.innerHTML = searchSuggestions.map(suggestion => `
                <div class="suggestion-item" onclick="selectSuggestion('${suggestion.name}')">
                    <strong>${suggestion.name}</strong> - ৳${suggestion.price.toLocaleString()}
                </div>
            `).join('');
            suggestionsEl.style.display = 'block';
        }

        function selectSuggestion(name) {
            document.getElementById('searchInput').value = name;
            filterProducts(name.toLowerCase());
            hideSuggestions();
        }

        function filterProducts(query = '') {
            let filtered = products.filter(p => 
                p.name.toLowerCase().includes(query) || query === ''
            );
            currentProducts = filtered;
            renderProducts();
        }

        // ===== CATEGORIES =====
        function renderCategories() {
            const grid = document.getElementById('categoriesGrid');
            grid.innerHTML = categories.map(cat => `
                <div class="category-card" data-category="${cat.value}">
                    <div class="category-icon">${cat.icon}</div>
                    <div class="category-name">${cat.name}</div>
                </div>
            `).join('');
        }

        function handleCategoryClick(e) {
            const categoryCard = e.target.closest('.category-card');
            if (!categoryCard) return;

            const category = categoryCard.dataset.category;
            document.querySelectorAll('.category-card').forEach(card => 
                card.classList.remove('active')
            );
            categoryCard.classList.add('active');

            if (category === 'all') {
                currentProducts = [...products];
            } else {
                currentProducts = products.filter(p => p.category === category);
            }
            renderProducts();
        }

        // ===== PRODUCTS =====
        function renderProducts() {
            const list = document.getElementById('productsList');
            if (currentProducts.length === 0) {
                list.innerHTML = `
                    <div style="text-align: center; padding: 3rem; color: #666;">
                        <i class="fas fa-search" style="font-size: 4rem; margin-bottom: 1rem; opacity: 0.5;"></i>
                        <h3>প্রোডাক্ট পাওয়া যায়নি</h3>
                        <p>অন্য সার্চ ট্রাই করুন</p>
                    </div>
                `;
                return;
            }

            list.innerHTML = currentProducts.map(product => `
                <div class="product-card">
                    <div class="product-image">${product.image}</div>
                    <div class="product-info">
                        <div>
                            <h3 class="product-title">${product.name}</h3>
                            <div class="product-price-row">
                                <span class="price">৳${product.price.toLocaleString()}</span>
                                ${product.oldPrice ? `<span class="old-price">৳${product.oldPrice.toLocaleString()}</span>` : ''}
                            </div>
                            <div class="rating-row">
                                <span class="stars">${'★'.repeat(Math.floor(product.rating))}</span>
                                <span>(${product.rating})</span>
                            </div>
                        </div>
                        <button class="add-cart-btn" onclick="addToCart(${product.id})">
                            <i class="fas fa-cart-plus"></i> কার্টে যোগ করুন
                        </button>
                    </div>
                </div>
            `).join('');
        }

        // ===== CART FUNCTIONS =====
        function addToCart(productId) {
            const product = products.find(p => p.id === productId);
            const cartItem = cart.find(item => item.id === productId);
            
            if (cartItem) {
                cartItem.quantity += 1;
            } else {
                cart.push({ ...product, quantity: 1 });
            }
            
            localStorage.setItem('daraz_cart', JSON.stringify(cart));
            updateCartBadge();
            showToast(`${product.name} কার্টে যোগ হয়েছে! 🛒`);
            
            // Haptic feedback
            if (navigator.vibrate) navigator.vibrate(50);
        }

        function updateCartBadge() {
            const totalItems = cart.reduce((sum, item) => sum + item.quantity, 0);
            const badge = document.getElementById('cartBadge');
            badge.textContent = totalItems;
            badge.style.display = totalItems > 0 ? 'block' : 'none';
        }

        function openCartModal() {
            renderCartModal();
            document.getElementById('cartModal').classList.add('active');
        }

        function closeCartModal() {
            document.getElementById('cartModal').classList.remove('active');
        }

        function renderCartModal() {
            const itemsEl = document.getElementById('modalCartItems');
            const totalEl = document.getElementById('modalTotal');
            
            if (cart.length === 0) {
                itemsEl.innerHTML = `
                    <div style="text-align: center; padding: 3rem; color: #666;">
                        <i class="fas fa-shopping-cart" style="font-size: 4rem; margin-bottom: 1rem; opacity: 0.5;"></i>
                        <h3>কার্ট খালি</h3>
                    </div>
                `;
                totalEl.textContent = '৳ ০';
                return;
            }

            itemsEl.innerHTML = cart.map(item => `
                <div class="cart-item">
                    <div class="cart-item-image">${item.image}</div>
                    <div style="flex: 1;">
                        <h4 style="font-size: 1rem; margin-bottom: 0.5rem;">${item.name}</h4>
                        <div style="font-weight: 700; color: var(--primary); margin-bottom: 0.8rem;">
                            ৳${item.price.toLocaleString()}
                        </div>
                        <div class="quantity-selector">
                            <button class="qty-btn" onclick="updateCartQuantity(${item.id}, -1)">-</button>
                            <span style="font-weight: 600; min-width: 25px;">${item.quantity}</span>
                            <button class="qty-btn" onclick="updateCartQuantity(${item.id}, 1)">+</button>
                        </div>
                    </div>
                    <button class="remove-btn" onclick="removeCartItem(${item.id})">
                        <i class="fas fa-trash"></i>
                    </button>
                </div>
            `).join('');

            const total = cart.reduce((sum, item) => sum + (item.price * item.quantity), 0);
            totalEl.textContent = `৳ ${total.toLocaleString()}`;
        }

        function updateCartQuantity(id, change) {
            const item = cart.find(item => item.id === id);
            if (item) {
                item.quantity += change;
                if (item.quantity <= 0) {
                    removeCartItem(id);
                    return;
                }
                localStorage.setItem('daraz_cart', JSON.stringify(cart));
                updateCartBadge();
                renderCartModal();
            }
        }

        function removeCartItem(id) {
            cart = cart.filter(item => item.id !== id);
            localStorage.setItem('daraz_cart', JSON.stringify(cart));
            updateCartBadge();
            renderCartModal();
            showToast('প্রোডাক্ট মুছে ফেলা হয়েছে', 'error');
        }

        function completeOrder() {
            if (cart.length === 0) {
                showToast('কার্ট খালি!', 'error');
                return;
            }
            
            const total = cart.reduce((sum, item) => sum + (item.price * item.quantity), 0);
            showToast(`অর্ডার সফল! মোট: ৳${total.toLocaleString()} ✅`);
            
            cart = [];
            localStorage.setItem('daraz_cart', JSON.stringify(cart));
            updateCartBadge();
            closeCartModal();
        }

        // ===== UTILITIES =====
        function scrollToProducts() {
            document.getElementById('productsList').scrollIntoView({ behavior: 'smooth' });
        }

        function startFlashTimer() {
            let time = 10683; // 2:47:23
            setInterval(() => {
                time--;
                const hours = Math.floor(time / 3600);
                const minutes = Math.floor((time % 3600) / 60);
                const seconds = time % 60;
                document.getElementById('flashTimer').textContent = 
                    `${hours.toString().padStart(2,'0')}:${minutes.toString().padStart(2,'0')}:${seconds.toString().padStart(2,'0')}`;
            }, 1000);
        }

        // ===== PWA FEATURES =====
        function requestPWAInstall() {
            window.addEventListener('beforeinstallprompt', (e) => {
                e.preventDefault();
                deferredPrompt = e;
                setTimeout(() => {
                    document.getElementById('installPrompt').style.display = 'block';
                }, 3000);
            });
        }

        function installPWA() {
            if (deferredPrompt) {
                deferredPrompt.prompt();
                deferredPrompt.userChoice.then(() => {
                    deferredPrompt = null;
                    hideInstallPrompt();
                });
            }
        }

        function hideInstallPrompt() {
            document.getElementById('installPrompt').style.display = 'none';
        }

        // ===== GESTURE SUPPORT =====
        let touchStartX = 0;
        document.addEventListener('touchstart', (e) => {
            touchStartX = e.touches[0].clientX;
        });

        document.addEventListener('touchend', (e) => {
            const touchEndX = e.changedTouches[0].clientX;
            const diff = touchStartX - touchEndX;
            
            if (Math.abs(diff) > 50) {
                if (diff > 0) {
                    // Swipe left
                    switchPage('cart');
                } else {
                    // Swipe right
                    switchPage('home');
                }
            }
        });

        // Close modal on backdrop click
        document.getElementById('cartModal').addEventListener('click', (e) => {
            if (e.target.classList.contains('modal-overlay')) {
                closeCartModal();
            }
        });

        // Keyboard support
        document.addEventListener('keydown', (e) => {
            if (e.key === 'Escape') closeCartModal();
        });
    </script>
</body>
</html>
