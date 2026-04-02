<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cool Point | Premium Shop & Services</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap');
        body { font-family: 'Inter', sans-serif; scroll-behavior: smooth; }
        .glass-nav { background: rgba(255, 255, 255, 0.8); backdrop-filter: blur(10px); }
        .product-card:hover { transform: translateY(-10px); transition: all 0.3s ease; }
        .green-gradient { background: linear-gradient(135deg, #10b981 0%, #059669 100%); }
    </style>
</head>
<body class="bg-gray-50 text-gray-900">

    <nav class="fixed w-full z-50 glass-nav border-b border-gray-100">
        <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
            <div class="text-2xl font-bold text-emerald-600 tracking-tight">COOL<span class="text-gray-800">POINT</span></div>
            <div class="hidden md:flex space-x-8 font-medium">
                <a href="#home" class="hover:text-emerald-600 transition">Home</a>
                <a href="#products" class="hover:text-emerald-600 transition">Products</a>
                <a href="#services" class="hover:text-emerald-600 transition">Services</a>
                <a href="#contact" class="hover:text-emerald-600 transition">Contact</a>
            </div>
            <button class="bg-emerald-600 text-white px-5 py-2 rounded-full font-semibold hover:bg-emerald-700 transition">Shop Now</button>
        </div>
    </nav>

    <section id="home" class="pt-32 pb-20 px-6 green-gradient text-white">
        <div class="max-w-7xl mx-auto text-center">
            <h1 class="text-5xl md:text-7xl font-bold mb-6">Elevate Your Lifestyle.</h1>
            <p class="text-xl opacity-90 mb-10 max-w-2xl mx-auto">Premium products and professional services tailored for the modern consumer. Experience the Cool Point difference.</p>
            <div class="flex justify-center gap-4">
                <a href="#products" class="bg-white text-emerald-700 px-8 py-3 rounded-lg font-bold shadow-lg">View Products</a>
                <a href="#services" class="border-2 border-white px-8 py-3 rounded-lg font-bold hover:bg-white hover:text-emerald-700 transition">Our Services</a>
            </div>
        </div>
    </section>

    <section id="products" class="py-20 px-6 max-w-7xl mx-auto">
        <div class="flex justify-between items-end mb-12">
            <div>
                <h2 class="text-3xl font-bold text-gray-800">Premium Collection</h2>
                <p class="text-gray-500">Explore our top 25 featured products</p>
            </div>
            <button class="text-emerald-600 font-semibold border-b-2 border-emerald-600">View All 50+</button>
        </div>
        
        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-6">
            <script>
                for(let i=1; i<=10; i++) {
                    document.write(`
                        <div class="product-card bg-white p-4 rounded-2xl shadow-sm border border-gray-100 cursor-pointer">
                            <div class="bg-gray-100 h-48 rounded-xl mb-4 flex items-center justify-center text-gray-400">
                                <i class="fa-regular fa-image text-3xl"></i>
                            </div>
                            <h3 class="font-bold text-gray-800">Cool Product #${i}</h3>
                            <p class="text-sm text-gray-500 mb-3">Premium Quality Item</p>
                            <div class="flex justify-between items-center">
                                <span class="text-emerald-600 font-bold">$199.00</span>
                                <button class="p-2 bg-gray-900 text-white rounded-lg hover:bg-emerald-600 transition">
                                    <i class="fa-solid fa-plus text-xs"></i>
                                </button>
                            </div>
                        </div>
                    `);
                }
            </script>
        </div>
    </section>

    <section id="services" class="py-20 bg-gray-900 text-white px-6">
        <div class="max-w-7xl mx-auto">
            <h2 class="text-3xl font-bold mb-2">Our Specialized Services</h2>
            <p class="text-gray-400 mb-12">Expert solutions for every need</p>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-5 gap-8">
                <script>
                    const icons = ['gear', 'shield-halved', 'truck-fast', 'headset', 'wand-magic-sparkles'];
                    for(let i=1; i<=5; i++) {
                        document.write(`
                            <div class="group border-l border-emerald-500/30 pl-6 py-4 hover:border-emerald-500 transition">
                                <i class="fa-solid fa-${icons[i-1]} text-3xl text-emerald-500 mb-4"></i>
                                <h3 class="text-xl font-bold mb-2">Service Line ${i}</h3>
                                <p class="text-gray-400 text-sm">Description of premium service providing top-tier results for clients.</p>
                            </div>
                        `);
                    }
                </script>
            </div>
        </div>
    </section>

    <footer id="contact" class="bg-white pt-20 pb-10 border-t border-gray-100">
        <div class="max-w-7xl mx-auto px-6 grid grid-cols-1 md:grid-cols-3 gap-12 mb-16">
            <div>
                <h3 class="text-xl font-bold mb-6">Cool Point</h3>
                <p class="text-gray-500 mb-6">The ultimate destination for professional products and reliable services.</p>
                <div class="flex gap-4">
                    <a href="#" class="w-10 h-10 rounded-full bg-gray-100 flex items-center justify-center hover:bg-emerald-600 hover:text-white transition"><i class="fa-brands fa-instagram"></i></a>
                    <a href="#" class="w-10 h-10 rounded-full bg-gray-100 flex items-center justify-center hover:bg-emerald-600 hover:text-white transition"><i class="fa-brands fa-facebook-f"></i></a>
                    <a href="#" class="w-10 h-10 rounded-full bg-emerald-100 text-emerald-600 flex items-center justify-center hover:bg-emerald-600 hover:text-white transition"><i class="fa-brands fa-whatsapp"></i></a>
                </div>
            </div>
            <div>
                <h3 class="text-lg font-bold mb-6">Quick Contact</h3>
                <p class="text-gray-600 mb-2 font-medium">WhatsApp: <span class="text-emerald-600">+1 234 567 890</span></p>
                <p class="text-gray-600 mb-2 font-medium">Email: <span class="text-emerald-600">hello@coolpoint.com</span></p>
                <p class="text-gray-600 font-medium">Instagram: <span class="text-emerald-600">@coolpoint_shop</span></p>
            </div>
            <form class="space-y-4">
                <input type="text" placeholder="Your Name" class="w-full p-3 bg-gray-50 border border-gray-200 rounded-lg outline-none focus:border-emerald-500">
                <textarea placeholder="How can we help?" class="w-full p-3 bg-gray-50 border border-gray-200 rounded-lg outline-none focus:border-emerald-500 h-24"></textarea>
                <button class="w-full bg-emerald-600 text-white py-3 rounded-lg font-bold shadow-lg hover:bg-emerald-700 transition">Send Message</button>
            </form>
        </div>
        <div class="text-center text-gray-400 text-sm border-t border-gray-50 pt-8">
            &copy; 2026 Cool Point Official. Built for Excellence.
        </div>
    </footer>

</body>
</html>
