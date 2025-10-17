Freitag, 17. Oktober 2025
22:17

<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dein Mobilfunk - Startseite</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .gradient-text {
            background: linear-gradient(to right, #34D399, #3B82F6);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .hero-card {
            background: #F9FAFB;
            border: 1px solid #E5E7EB;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .hero-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
        }
    </style>
</head>
<body class="bg-white">

    <!-- Header-Sektion -->
    <header class="bg-white/80 backdrop-blur-md sticky top-0 z-50 border-b border-gray-200">
        <nav class="container mx-auto px-4 lg:px-6 py-4">
            <div class="flex justify-between items-center">
                <a href="#" class="flex items-center space-x-2">
                    <svg class="h-8 w-8 text-emerald-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M8.288 15.043A5.242 5.242 0 017.5 14.25a5.25 5.25 0 01-1.68-1.043 5.25 5.25 0 01-1.043-1.68 5.25 5.25 0 010-2.056 5.25 5.25 0 011.043-1.68 5.25 5.25 0 011.68-1.043 5.25 5.25 0 012.056 0 5.25 5.25 0 011.68 1.043 5.25 5.25 0 011.043 1.68 5.25 5.25 0 010 2.056 5.25 5.25 0 01-1.043 1.68 5.25 5.25 0 01-1.68 1.043z" />
                        <path stroke-linecap="round" stroke-linejoin="round" d="M15.712 15.043a5.242 5.242 0 01-.788-.788 5.25 5.25 0 01-1.043-1.68 5.25 5.25 0 010-2.056 5.25 5.25 0 011.043-1.68 5.25 5.25 0 011.68-1.043 5.25 5.25 0 012.056 0 5.25 5.25 0 011.68 1.043 5.25 5.25 0 011.043 1.68 5.25 5.25 0 010 2.056 5.25 5.25 0 01-1.043 1.68 5.25 5.25 0 01-1.68 1.043 5.242 5.242 0 01-.788.788z" />
                    </svg>
                    <span class="text-2xl font-bold text-gray-800">ConnectMe</span>
                </a>
                
                <div class="hidden lg:flex items-center space-x-8">
                    <a href="#" class="text-gray-600 hover:text-emerald-500 font-semibold transition-colors">Angebote</a>
                    <a href="#" class="text-gray-600 hover:text-emerald-500 font-semibold transition-colors">Mobilfunk</a>
                    <a href="#" class="text-gray-600 hover:text-emerald-500 font-semibold transition-colors">Internet</a>
                    <a href="#" class="text-gray-600 hover:text-emerald-500 font-semibold transition-colors">Hilfe & Service</a>
                </div>

                <div class="flex items-center space-x-4">
                    <a href="#" class="text-gray-500 hover:text-emerald-500">
                        <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z" />
                        </svg>
                    </a>
                    <a href="#" class="text-gray-500 hover:text-emerald-500">
                        <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 3h1.386c.51 0 .955.343 1.087.835l.383 1.437M7.5 14.25a3 3 0 00-3 3h15.75m-12.75-3h11.218c.51 0 .962-.343 1.087-.835l1.823-6.831A1.125 1.125 0 0018.142 6H4.498L5.94 11.25l-2.25 0" />
                        </svg>
                    </a>
                    <button id="mobile-menu-button" class="lg:hidden text-gray-500 hover:text-emerald-500">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                        </svg>
                    </button>
                </div>
            </div>
            <!-- Mobiles Menü -->
            <div id="mobile-menu" class="hidden lg:hidden mt-4">
                <a href="#" class="block py-2 px-4 text-sm text-gray-600 hover:bg-gray-100 rounded">Angebote</a>
                <a href="#" class="block py-2 px-4 text-sm text-gray-600 hover:bg-gray-100 rounded">Mobilfunk</a>
                <a href="#" class="block py-2 px-4 text-sm text-gray-600 hover:bg-gray-100 rounded">Internet</a>
                <a href="#" class="block py-2 px-4 text-sm text-gray-600 hover:bg-gray-100 rounded">Hilfe & Service</a>
            </div>
        </nav>
    </header>

    <!-- Hauptinhalt -->
    <main class="container mx-auto px-4 lg:px-6 py-12">
        
        <!-- Helden-Sektion -->
        <section class="text-center mb-20">
            <h1 class="text-4xl md:text-6xl font-bold text-gray-800 mb-4 leading-tight">
                Die Freiheit, die du <span class="gradient-text">verdienst</span>.
            </h1>
            <p class="text-lg text-gray-500 max-w-3xl mx-auto">
                Finde den perfekten Mobilfunk- oder Internettarif, der genau zu deinem Leben passt. Flexibel, fair und ohne Schnickschnack.
            </p>
        </section>

        <!-- Angebots-Karten -->
        <section class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-24">
            <!-- Karte 1: Mobilfunk -->
            <div class="hero-card rounded-2xl p-8 lg:p-12 flex flex-col items-center text-center">
                <div class="bg-emerald-100 text-emerald-600 text-sm font-bold px-4 py-1 rounded-full mb-4">Unser Bestseller</div>
                <h2 class="text-3xl font-bold text-gray-800 mb-2">Allnet Flat M</h2>
                <p class="text-5xl font-bold text-gray-900 mb-2">100 <span class="text-3xl text-gray-500">GB</span></p>
                <p class="text-gray-500 mb-6">mit 5G-Speed surfen</p>
                <ul class="text-left space-y-2 mb-8 text-gray-600">
                    <li class="flex items-center"><svg class="h-5 w-5 text-emerald-500 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" /></svg>Telefon- & SMS-Flat</li>
                    <li class="flex items-center"><svg class="h-5 w-5 text-emerald-500 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" /></svg>EU-Roaming inklusive</li>
                    <li class="flex items-center"><svg class="h-5 w-5 text-emerald-500 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" /></svg>Monatlich kündbar</li>
                </ul>
                <div class="mt-auto w-full">
                    <p class="text-3xl font-bold mb-4">24€ <span class="text-xl font-normal text-gray-500">/ Monat</span></p>
                    <a href="#" class="w-full block bg-emerald-500 text-white font-bold py-3 px-6 rounded-lg hover:bg-emerald-600 transition-colors text-center">Zum Tarif</a>
                </div>
            </div>

            <!-- Karte 2: Internet -->
            <div class="hero-card rounded-2xl p-8 lg:p-12 flex flex-col items-center text-center">
                <div class="bg-blue-100 text-blue-600 text-sm font-bold px-4 py-1 rounded-full mb-4">Internet für Zuhause</div>
                <h2 class="text-3xl font-bold text-gray-800 mb-2">Home Speed 100</h2>
                <p class="text-5xl font-bold text-gray-900 mb-2">100 <span class="text-3xl text-gray-500">MBit/s</span></p>
                <p class="text-gray-500 mb-6">Stabiles & schnelles WLAN</p>
                <ul class="text-left space-y-2 mb-8 text-gray-600">
                     <li class="flex items-center"><svg class="h-5 w-5 text-emerald-500 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" /></svg>Perfekt für Streaming & Homeoffice</li>
                    <li class="flex items-center"><svg class="h-5 w-5 text-emerald-500 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" /></svg>Einfache Installation</li>
                    <li class="flex items-center"><svg class="h-5 w-5 text-emerald-500 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" /></svg>Ohne lange Vertragslaufzeit</li>
                </ul>
                <div class="mt-auto w-full">
                    <p class="text-3xl font-bold mb-4">33€ <span class="text-xl font-normal text-gray-500">/ Monat</span></p>
                    <a href="#" class="w-full block bg-blue-500 text-white font-bold py-3 px-6 rounded-lg hover:bg-blue-600 transition-colors text-center">Zur Verfügbarkeit</a>
                </div>
            </div>
        </section>

        <!-- "Deine Vorteile" Sektion -->
        <section class="mb-24">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-12">Deine Vorteile bei ConnectMe</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="text-center p-6 bg-gray-50 rounded-lg">
                    <div class="flex items-center justify-center h-16 w-16 rounded-full bg-emerald-100 text-emerald-500 mx-auto mb-4">
                        <svg class="h-8 w-8" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" d="M19.5 12c0-1.232-.046-2.453-.138-3.662a4.006 4.006 0 00-3.7-3.7 48.678 48.678 0 00-7.324 0 4.006 4.006 0 00-3.7 3.7c-.092 1.21-.138 2.43-.138 3.662v.114M19.5 12h-15M12 4.5v.001M12 21.75v.001M4.5 12v.001M21.75 12v.001" /></svg>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Top-Netzabdeckung</h3>
                    <p class="text-gray-500">Surfe und telefoniere zuverlässig im besten Netz.</p>
                </div>
                <div class="text-center p-6 bg-gray-50 rounded-lg">
                    <div class="flex items-center justify-center h-16 w-16 rounded-full bg-emerald-100 text-emerald-500 mx-auto mb-4">
                        <svg class="h-8 w-8" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" d="M12 6v6h4.5m4.5 0a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Volle Flexibilität</h3>
                    <p class="text-gray-500">Wähle Tarife, die du monatlich anpassen oder kündigen kannst.</p>
                </div>
                <div class="text-center p-6 bg-gray-50 rounded-lg">
                     <div class="flex items-center justify-center h-16 w-16 rounded-full bg-emerald-100 text-emerald-500 mx-auto mb-4">
                        <svg class="h-8 w-8" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" d="M14.25 7.756a4.5 4.5 0 100 8.488M7.5 10.5h5.25m-5.25 3h5.25M21 12a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Faire Preise</h3>
                    <p class="text-gray-500">Keine versteckten Kosten. Du zahlst nur, was du brauchst.</p>
                </div>
                <div class="text-center p-6 bg-gray-50 rounded-lg">
                     <div class="flex items-center justify-center h-16 w-16 rounded-full bg-emerald-100 text-emerald-500 mx-auto mb-4">
                        <svg class="h-8 w-8" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" d="M9.813 15.904L9 18.75l-.813-2.846a4.5 4.5 0 00-3.09-3.09L2.25 12l2.846-.813a4.5 4.5 0 003.09-3.09L9 5.25l.813 2.846a4.5 4.5 0 003.09 3.09L15.75 12l-2.846.813a4.5 4.5 0 00-3.09 3.09zM18.259 8.715L18 9.75l-.259-1.035a3.375 3.375 0 00-2.455-2.456L14.25 6l1.036-.259a3.375 3.375 0 002.455-2.456L18 2.25l.259 1.035a3.375 3.375 0 002.456 2.456L21.75 6l-1.035.259a3.375 3.375 0 00-2.456 2.456zM16.898 20.553L16.5 21.75l-.398-1.197a3.375 3.375 0 00-2.455-2.456L12.75 18l1.197-.398a3.375 3.375 0 002.455-2.456L16.5 14.25l.398 1.197a3.375 3.375 0 002.456 2.455L20.25 18l-1.197.398a3.375 3.375 0 00-2.456 2.455z" /></svg>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Exzellenter Service</h3>
                    <p class="text-gray-500">Wir sind für dich da, wenn du uns brauchst.</p>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white">
        <div class="container mx-auto px-4 lg:px-6 py-12">
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8 mb-8">
                <div>
                    <h4 class="font-bold mb-4">Shop</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Mobilfunktarife</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Prepaid</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Internet für Zuhause</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Handys</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-4">Hilfe & Service</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Hilfe-Center</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Kontakt</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Mein Konto</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Downloads</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-4">Über ConnectMe</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Unternehmen</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Presse</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Karriere</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-4">Folge uns</h4>
                    <div class="flex space-x-4">
                        <!-- Hier könnten SVG-Icons für soziale Medien platziert werden -->
                        <a href="#" class="text-gray-400 hover:text-white">Facebook</a>
                        <a href="#" class="text-gray-400 hover:text-white">Instagram</a>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-700 pt-6 text-center text-gray-500 text-sm">
                <p>&copy; 2025 ConnectMe. Alle Rechte vorbehalten.</p>
                <div class="mt-2 space-x-4">
                    <a href="#" class="hover:text-white">Impressum</a>
                    <a href="#" class="hover:text-white">Datenschutz</a>
                    <a href="#" class="hover:text-white">AGB</a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // JavaScript für das mobile Menü
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
    </script>
</body>
</html>


Microsoft OneNote abrufen: https://aka.ms/GetOneNoteMobile