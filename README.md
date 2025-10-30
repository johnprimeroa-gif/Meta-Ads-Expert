<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meta Ads Expert - El Sistema para Campañas Rentables</title>
    
<script src="https://cdn.tailwindcss.com"></script>
    
<link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght400;600;700;900;950&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        /* Estilos de transición y sombra para el botón CTA */
        .cta-button {
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px 0 rgba(59, 130, 246, 0.4);
        }
        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px 0 rgba(59, 130, 246, 0.6);
        }

        /* Estilo para la barra de desplazamiento */
        ::-webkit-scrollbar { width: 10px; }
        ::-webkit-scrollbar-track { background: #111827; }
        ::-webkit-scrollbar-thumb {
            background: #1e3a8a; 
            border-radius: 5px;
        }
        ::-webkit-scrollbar-thumb:hover { background: #2563eb; }

        /* Cursor pointer para botones de Hotmart que se activan con JS */
        .hotmart-button {
            cursor: pointer;
        }
        
        /* Estilos específicos para la alineación de precios inicial */
        #initial-price-group {
            display: flex;
            align-items: baseline;
            justify-content: center;
        }
        
        /* Estilos para el contenedor de precios después de aplicar el cupón */
        #price-container.coupon-applied {
            justify-content: flex-start; /* Alineación a la izquierda */
        }
        #price-container.coupon-applied > div {
            align-self: center; /* Centrar verticalmente los tachados */
        }
        #price-container.coupon-applied #finalPriceDisplay {
            align-self: center; /* Centrar verticalmente el precio final */
        }

        /* FIX SCROLL: Asegura que el ancla no quede oculta bajo el header fijo (aprox 64px) */
        #contenido {
            scroll-margin-top: 5rem; 
        }
    </style>
</head>
<body class="bg-gray-900 text-white">

    <!-- Header Fijo -->
<header class="bg-gray-900/90 backdrop-blur-md sticky top-0 z-50 border-b border-gray-700">
        <nav class="container mx-auto px-4 sm:px-6 py-4 flex justify-between items-center">
            <h1 class="text-xl sm:text-2xl font-black">
                Meta Ads <span class="text-blue-400">Expert</span>
            </h1>
            <!-- CTA Header - Botón de compra (se actualiza al aplicar cupón) -->
            <a href="#" id="header-cta" class="hotmart-button bg-blue-600 text-white font-semibold text-sm sm:text-base px-4 py-2 sm:px-5 sm:py-2 rounded-lg hover:bg-blue-700 transition-colors">
                Obtener E-book
            </a>
        </nav>
    </header>

    <!-- Sección Principal (Hero) -->
<main class="container mx-auto px-4 sm:px-6 py-16 md:py-24 text-center">
        <div class="max-w-4xl mx-auto">
            <span class="text-blue-400 font-semibold uppercase tracking-wider text-sm sm:text-base">John S.H.</span>
            <h2 class="text-4xl sm:text-5xl md:text-7xl font-extrabold text-white mt-3 mb-6 leading-tight">
                Deja de Botar Dinero en Meta Ads.
            </h2>
            <p class="text-base sm:text-lg md:text-xl text-gray-300 mb-10 max-w-3xl mx-auto">
                Descubre el sistema exacto para construir, testear y escalar campañas rentables. Esto no es teoría, es la guía práctica que transforma clics en clientes.
            </p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <!-- CTA Principal - Botón de compra (se actualiza al aplicar cupón) -->
                <a href="#" id="hero-cta" class="hotmart-button cta-button bg-blue-600 text-white font-bold text-base sm:text-lg px-8 py-3 sm:px-10 sm:py-4 rounded-lg shadow-lg">
                    ¡QUIERO EL SISTEMA AHORA!
                </a>
                <a href="#contenido" id="scrollContent" class="bg-gray-700 text-white font-bold text-base sm:text-lg px-8 py-3 sm:px-10 sm:py-4 rounded-lg hover:bg-gray-600 transition-colors">
                    Ver el contenido
                </a>
            </div>
        </div>
    </main>

    <!-- Sección de Puntos de Dolor -->
<section class="bg-gray-800 py-16 md:py-24">
        <div class="container mx-auto px-4 sm:px-6 max-w-6xl">
            <div class="text-center mb-12">
                <h3 class="text-3xl md:text-4xl font-bold text-white mb-4">¿Te suena familiar?</h3>
                <p class="text-lg text-gray-400 max-w-2xl mx-auto">
                    La mayoría de la gente pierde dinero en Meta Ads. Este e-book es para ti si...
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
                
                <div class="bg-gray-900 p-6 sm:p-8 rounded-xl shadow-lg border border-gray-700">
                    <div class="text-3xl sm:text-4xl mb-4">💸</div>
                    <!-- TEXTO ACTUALIZADO: ROAS malísimo -->
                    <h4 class="text-xl font-semibold text-white mb-2">ROAS malísimo</h4>
                    <p class="text-gray-400 text-sm sm:text-base">Inviertes $100.000 CLP y (con suerte) sacas $110.000 CLP. Tus campañas apenas sobreviven y no tienes idea de cómo hacerlas rentables.</p>
                </div>
                
                <div class="bg-gray-900 p-6 sm:p-8 rounded-xl shadow-lg border border-gray-700">
                    <div class="text-3xl sm:text-4xl mb-4">🤯</div>
                    <h4 class="text-xl font-semibold text-white mb-2">Estás abrumado</h4>
                    <p class="text-gray-400 text-sm sm:text-base">Pixel, CAPI, TOFU, BOFU, CBO, ABO... Estás paralizado por la complejidad técnica y no sabes por dónde empezar.</p>
                </div>
                
                <div class="bg-gray-900 p-6 sm:p-8 rounded-xl shadow-lg border border-gray-700">
                    <div class="text-3xl sm:text-4xl mb-4">📉</div>
                    <h4 class="text-xl font-semibold text-white mb-2">Tus anuncios no funcionan</h4>
                    <p class="text-gray-400 text-sm sm:text-base">Lanzas creativos que crees geniales, pero nadie hace clic. Tu CTR está por los suelos y tu CPA por las nubes.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Contenido/Características -->
<section id="contenido" class="py-16 md:py-24 bg-gray-900">
        <div class="container mx-auto px-4 sm:px-6 max-w-6xl grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
            
            <div>
                <img src="https://placehold.co/500x600/0F172A/38BDF8?text=Meta+Ads+Expert" alt="Portada del E-book Meta Ads Expert por John S.H." class="rounded-lg shadow-2xl mx-auto w-full max-w-xs sm:max-w-md border-2 border-blue-500">
            </div>

            
            <div class="space-y-6">
                <h3 class="text-3xl md:text-4xl font-bold mb-6">El sistema exacto para dejar de adivinar</h3>
                <p class="text-base sm:text-lg text-gray-300 mb-6">"Meta Ads Expert" no es teoría. Es un manual de campo. Esto es solo una parte de lo que dominarás:</p>
                
                <div class="flex items-start gap-4">
                    <div class="bg-blue-600 p-2 rounded-full flex-shrink-0 mt-1">
                        <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                    </div>
                    <div>
                        <h4 class="text-lg sm:text-xl font-semibold">Arquitectura de Campañas Full-Funnel</h4>
                        <p class="text-gray-400 text-sm sm:text-base">El systema exacto (TOFU, MOFU, BOFU) para guiar a un extraño frío hasta convertirlo en cliente.</p>
                    </div>
                </div>

                <div class="flex items-start gap-4">
                    <div class="bg-blue-600 p-2 rounded-full flex-shrink-0 mt-1">
                        <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                    </div>
                    <div>
                        <h4 class="text-lg sm:text-xl font-semibold">El Método HSO: Creativos que Convierten</h4>
                        <p class="text-gray-400 text-sm sm:text-base">Domina la fórmula Hook → Story → Offer para crear anuncios que detienen el scroll y fuerzan el clic.</p>
                    </div>
                </div>
                
                <div class="flex items-start gap-4">
                    <div class="bg-blue-600 p-2 rounded-full flex-shrink-0 mt-1">
                        <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                    </div>
                    <div>
                        <h4 class="text-lg sm:text-xl font-semibold">Métricas que Importan (y cómo leerlas)</h4>
                        <p class="text-gray-400 text-sm sm:text-base">Aprende qué métricas deciden si pausar o escalar. Deja de mirar el CTR y enfócate en el ROAS y CPA.</p>
                    </div>
                </div>
                
                <!-- PUNTO DE RETARGETING (del cambio anterior) -->
                <div class="flex items-start gap-4">
                    <div class="bg-blue-600 p-2 rounded-full flex-shrink-0 mt-1">
                        <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                    </div>
                    <div>
                        <h4 class="text-lg sm:text-xl font-semibold">El Secreto del Retargeting Efectivo</h4>
                        <p class="text-gray-400 text-sm sm:text-base">Convierte visitantes en clientes. Descubre los 3 tipos de retargeting y los mensajes de alta conversión.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Testimonios -->
    <section class="py-16 md:py-24 bg-gray-800 border-t border-gray-700">
        <div class="container mx-auto px-4 sm:px-6 max-w-4xl text-center">
            <h3 class="text-3xl md:text-4xl font-bold text-white mb-12">Resultados. No opiniones.</h3>
            <div class="space-y-8 md:space-y-0 md:grid md:grid-cols-2 md:gap-8">
                
                <div class="bg-gray-900 p-6 sm:p-8 rounded-lg shadow-lg text-left border border-gray-700">
                    <div class="flex items-center mb-4">
                        <img class="w-10 h-10 sm:w-12 sm:h-12 rounded-full mr-4 object-cover" src="https://placehold.co/100x100/1E3A8A/FFFFFF?text=A.L." alt="Foto de Ana L.">
                        <div>
                            <p class="font-semibold text-white">Ana L.</p>
                            <p class="text-xs sm:text-sm text-blue-400">Fundadora de E-commerce</p>
                        </div>
                    </div>
                    <p class="text-gray-300 italic text-sm sm:text-base">"Estaba a punto de rendirme con Meta Ads. Compré el e-book y en la primera semana, aplicando solo el Capítulo 4 (HSO), mi CPA bajó un 40%. Increíble."</p>
                </div>
                
                <div class="bg-gray-900 p-6 sm:p-8 rounded-lg shadow-lg text-left border border-gray-700">
                    <div class="flex items-center mb-4">
                        <img class="w-10 h-10 sm:w-12 sm:h-12 rounded-full mr-4 object-cover" src="https://placehold.co/100x100/1E3A8A/FFFFFF?text=M.R." alt="Foto de Marcos R.">
                        <div>
                            <p class="font-semibold text-white">Marcos R.</p>
                            <p class="text-xs sm:text-sm text-blue-400">Consultor de Marketing</p>
                        </div>
                    </div>
                    <p class="text-gray-300 italic text-sm sm:text-base">"Este e-book es un atajo. Dejé de probar 'cosas' y empecé a seguir un sistema. Mi ROAS se duplicó al aplicar el modelo de arquitectura full-funnel del Capítulo 3."</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Sección de Cupón -->
<section id="coupon-generator" class="bg-gray-900 py-16 md:py-24 border-t border-gray-700">
        <div class="container mx-auto px-4 sm:px-6 max-w-3xl text-center">
            
            <!-- Inicialmente Azul, cambia a Esmeralda al aplicar cupón -->
            <div id="coupon-box" class="bg-gradient-to-br from-blue-900 to-blue-800 text-white p-6 sm:p-10 md:p-12 rounded-xl shadow-2xl border border-blue-600">
                <h3 class="text-2xl sm:text-3xl md:text-4xl font-extrabold mt-4 mb-4">
                    🎁 ¡Descuento Secreto Desbloqueado! 🎁
                </h3>
                
                <!-- Texto de descuento -->
                <p class="text-base sm:text-lg text-blue-300 mb-8 font-semibold">
                    Pero espera... antes de pagar, escribe "quiero mi descuento" para desbloquear el código secreto del 33,35% ($5.000 CLP) sobre el precio de oferta y pagar aún menos.
                </p>

                <div class="flex flex-col sm:flex-row gap-4 mb-6">
                    <input type="text" id="couponInput" placeholder="Escribe aquí 'quiero mi descuento'" class="w-full p-3 rounded-lg bg-gray-700 text-white border border-gray-600 focus:border-blue-500 focus:outline-none placeholder:text-gray-400" />
                    
                    <button id="applyCouponButton" class="sm:w-auto bg-blue-600 text-white font-bold text-lg px-8 py-3 rounded-lg hover:bg-blue-700 transition-colors shadow-lg">
                        Aplicar
                    </button>
                </div>

                <div id="couponMessage" class="h-6 text-blue-300 text-sm font-medium"></div>

                <div id="couponCodeDisplay" class="hidden mt-4">
                    
                    <p class="text-base sm:text-lg font-semibold text-blue-300">¡Cupón Aplicado! Código: <span class="coupon-code-span text-xl sm:text-2xl font-extrabold text-white bg-blue-700 p-1 rounded">METAEXPERT25</span></p>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Compra Final -->
<section id="comprar" class="bg-gray-800 py-16 md:py-24 border-t border-gray-700">
        <div class="container mx-auto px-4 sm:px-6 max-w-3xl text-center">
            <div class="bg-gradient-to-br from-gray-700 to-gray-800 text-white p-6 sm:p-10 md:p-16 rounded-xl shadow-2xl border border-blue-500">
                <span class="text-blue-400 font-semibold uppercase text-sm sm:text-base">Acceso inmediato</span>
                <h3 class="text-3xl sm:text-4xl md:text-5xl font-extrabold mt-4 mb-6">Consigue tu Ebook "Meta Ads Expert"</h3>
                
                <!-- Bloque de precios: Estructura inicial -->
                <div id="price-container" class="flex flex-col sm:flex-row items-baseline justify-center gap-4 mb-4">
                    
                    <!-- Grupo de precios iniciales (59.990 tachado y 14.990 destacado) -->
                    <div id="initial-price-group" class="flex items-baseline gap-2">
                         <!-- Precio Original (59.990) -->
                        <p id="originalPriceContainer" class="text-xl sm:text-2xl font-bold text-gray-500 line-through transition-all duration-300">
                            <span id="originalPrice">$59.990</span>
                        </p>
                        
                        <!-- Precio de Oferta (14.990) - Inicialmente destacado -->
                        <p id="currentPriceContainer" class="text-4xl sm:text-5xl font-extrabold text-white transition-all duration-300">
                            <span id="currentPrice">$14.990</span>
                        </p>
                    </div>
                   
                    <!-- Precio Final (9.990) - Inicialmente oculto, solo aparece con el cupón -->
                    <p id="finalPriceDisplay" class="text-4xl sm:text-5xl font-extrabold text-emerald-400 hidden transition-all duration-300">
                        $9.990
                    </p>
                </div>

                <!-- Mensaje de precio final: $9.990 CLP con código (Centralizado y con salto de línea) -->
                <p id="couponAppliedMessage" class="hidden text-emerald-400 text-base sm:text-xl font-bold mb-8 text-center leading-relaxed">
                    ¡$5.000 CLP de Descuento Extra Aplicados! <br/>
                    Precio Final: $9.990 solo aplicando el código METAEXPERT25
                </p>

                <!-- TEXTO FINAL ACTUALIZADO -->
                <p class="text-sm sm:text-base text-gray-300 mb-8">
                    Oferta de lanzamiento. Pago único. Acceso de por vida a nuestro Ebook.
                </p>
                <!-- CTA Final - Botón de compra (se actualiza al aplicar cupón) -->
                <a href="#" id="final-cta" 
                   class="hotmart-button cta-button w-full bg-blue-600 text-white font-bold text-lg sm:text-xl px-10 py-4 sm:py-5 rounded-lg shadow-lg block">
                    ¡SÍ, QUIERO EL ACCESO AHORA!
                </a>
                
                <!-- Texto de garantía -->
                <p class="text-gray-400 text-xs sm:text-sm mt-6">Garantía de 7 días: si no crees que este e-book vale 4 veces a su precio original, te devuelvo tu dinero. Sin preguntas.</p>
            </div>
        </div>
    </section>

    <!-- Footer -->
<footer class="bg-gray-900 text-gray-500 py-12 border-t border-gray-800">
        <div class="container mx-auto px-4 sm:px-6 text-center text-sm">
            <p>&copy; 2025 Meta Ads Expert por John S.H. Todos los derechos reservados.</p>
            <div class="flex justify-center gap-6 mt-4">
                <a href="#" class="hover:text-white">Política de Privacidad</a>
                <a href="#" class="hover:text-white">Términos de Uso</a>
            </div>
        </div>
    </footer>

    <!-- JavaScript para Scroll Suave y Cupón -->
<script>
        // === GESTIÓN DE SCROLL SUAVE ===
        const scrollLink = document.getElementById('scrollContent');
        
        // Se ha implementado scroll-margin-top en el CSS para la compensación del header.
        if (scrollLink) {
            scrollLink.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    // Usamos solo scrollIntoView y dejamos que el CSS (scroll-margin-top) 
                    // maneje la compensación del header fijo.
                    targetElement.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        }
        
        // === GESTIÓN DE CUPÓN DE DESCUENTO ===
        const couponInput = document.getElementById('couponInput');
        const applyCouponButton = document.getElementById('applyCouponButton');
        const couponMessage = document.getElementById('couponMessage');
        const couponCodeDisplay = document.getElementById('couponCodeDisplay');
        
        const priceContainer = document.getElementById('price-container');
        const originalPriceContainer = document.getElementById('originalPriceContainer'); // 59.990
        const currentPriceContainer = document.getElementById('currentPriceContainer'); // 14.990
        const finalPriceDisplay = document.getElementById('finalPriceDisplay'); // 9.990
        const couponAppliedMessage = document.getElementById('couponAppliedMessage');
        const couponBox = document.getElementById('coupon-box');
        const couponCodeSpan = document.querySelector('.coupon-code-span');
        const hotmartButtons = document.querySelectorAll('.hotmart-button'); 
        
        // URLs y códigos
        const BASE_HOTMART_URL = "https://pay.hotmart.com/D102652988X";
        const COUPON_CODE_PARAM = "a4hjpu5h"; 
        const COUPON_HOTMART_URL = `${BASE_HOTMART_URL}?off=${COUPON_CODE_PARAM}`; 
        const BASE_HOTMART_URL_NO_DISCOUNT = `${BASE_HOTMART_URL}?checkoutMode=2`; 
        
        // Constantes de Precios
        const BASE_FULL_PRICE = 59990;
        const BASE_OFFER_PRICE = 14990; 
        const FINAL_PRICE = 9990; 
        const TARGET_INPUT = "quiero mi descuento";
        const DISPLAY_COUPON_CODE = "METAEXPERT25"; 

        let isCouponApplied = false;

        function formatPrice(price) {
            return `$${price.toLocaleString('es-CL')}`;
        }

        applyCouponButton.addEventListener('click', () => {
            // Manejamos las mayúsculas/minúsculas aquí
            const inputValue = couponInput.value.toLowerCase().trim();

            if (isCouponApplied) {
                couponMessage.textContent = "El descuento ya está aplicado.";
                return;
            }

            if (inputValue === TARGET_INPUT) {
                // Aplicar descuento
                isCouponApplied = true;
                
                // 1. Actualizar precios en la UI (Sección Final)
                
                // 1.1 Mover y tachar el precio de oferta (14.990)
                currentPriceContainer.classList.add('text-gray-500', 'line-through', 'text-xl', 'sm:text-2xl');
                currentPriceContainer.classList.remove('text-white', 'text-4xl', 'sm:text-5xl');
                
                // 1.2 Mostrar el precio final (9.990)
                finalPriceDisplay.classList.remove('hidden');

                // 1.3 Reajustar el contenedor principal para la alineación a la izquierda
                priceContainer.classList.add('coupon-applied', 'justify-start', 'gap-2');
                priceContainer.classList.remove('justify-center');
                
                // 2. Actualizar links de Hotmart con el código de descuento
                hotmartButtons.forEach(button => {
                    button.href = COUPON_HOTMART_URL;
                    // Cambiar color de los botones a esmeralda
                    button.classList.remove('bg-blue-600', 'hover:bg-blue-700');
                    button.classList.add('bg-emerald-600', 'hover:bg-emerald-700');
                });

                // 3. Mostrar mensajes y deshabilitar input
                couponMessage.textContent = `¡Cupón ${DISPLAY_COUPON_CODE} aplicado con éxito!`;
                couponCodeDisplay.classList.remove('hidden');
                couponAppliedMessage.classList.remove('hidden');
                couponInput.disabled = true;
                applyCouponButton.disabled = true;

                // 4. Estilizar la caja para indicar éxito (Tonos de Verde Esmeralda)
                couponBox.classList.remove('from-blue-900', 'to-blue-800', 'border-blue-600');
                couponBox.classList.add('from-emerald-700', 'to-emerald-600', 'border-emerald-400'); 
                
                // Estilizar el código del cupón para que destaque
                couponCodeSpan.classList.remove('bg-blue-700');
                couponCodeSpan.classList.add('bg-emerald-500'); 
                
            } else if (inputValue === "") {
                couponMessage.textContent = "Por favor, escribe el texto solicitado para el cupón.";
            } else {
                couponMessage.textContent = `Texto incorrecto. Por favor, escribe: "${TARGET_INPUT}".`;
            }
        });
        
        // Inicializar links y precios
        document.addEventListener('DOMContentLoaded', () => {
            // Inicializar Hotmart URLs (base sin descuento)
            hotmartButtons.forEach(button => {
                button.href = BASE_HOTMART_URL_NO_DISCOUNT;
            });
            
            // Asegurar que los precios iniciales se muestren correctamente
            document.getElementById('originalPrice').textContent = formatPrice(BASE_FULL_PRICE); // $59.990 CLP
            document.getElementById('currentPrice').textContent = formatPrice(BASE_OFFER_PRICE); // $14.990 CLP
            
            // Asegurar que el 59.990 se vea pequeño y tachado al inicio
            originalPriceContainer.classList.add('text-xl', 'sm:text-2xl');
            
            // Asegurar que el 14.990 se vea grande y NO tachado al inicio
            currentPriceContainer.classList.remove('line-through');
        });
    </script>

</body>
</html>
