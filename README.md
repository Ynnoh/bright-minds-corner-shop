<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bright Minds Corner | Printable Worksheets & Resources</title>
    <!-- Load Tailwind CSS via CDN --><script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom font import and fallback */
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            /* Using a very light, almost white background */
            background-color: #fcfcfc;
        }
    </style>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        // New Pastel Color Scheme based on the logo
                        'pastel-blue': '#B3D9FF', // Soft blue for backgrounds/accents
                        'pastel-green': '#C2F0C2', // Soft green for accents
                        'pastel-yellow': '#FFECB3', // Soft yellow for highlights
                        'pastel-pink': '#FFC2E0',  // Soft pink accent
                        'pastel-purple': '#D4B3FF', // Soft purple accent
                        'dark-text': '#4A5568', // Darker text for readability
                        'light-text': '#718096', // Lighter text for secondary info
                        'surface-bg': '#FFFFFF', // Pure white for cards and main content areas
                    },
                }
            }
        }

        // --- Mobile Menu Toggle Functionality ---
        function toggleMobileMenu() {
            const menu = document.getElementById('mobile-menu');
            const button = document.getElementById('menu-button');
            const isHidden = menu.classList.toggle('hidden');

            if (isHidden) {
                button.setAttribute('aria-expanded', 'false');
            } else {
                button.setAttribute('aria-expanded', 'true');
            }
        }
    </script>
</head>
<body>

    <!-- Header & Navigation --><header class="bg-surface-bg shadow-md sticky top-0 z-10">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- Logo --><a href="#" class="flex-shrink-0">
                    <img src="https://i.imgur.com/uRj0yI7.png" alt="Bright Minds Corner Logo" class="h-12 w-auto">
                </a>

                <!-- Desktop Navigation --><nav class="hidden md:flex space-x-8 items-center">
                    <a href="#featured" class="text-dark-text hover:text-pastel-blue font-medium transition duration-150">Worksheets</a>
                    <a href="#how-it-works" class="text-dark-text hover:text-pastel-blue font-medium transition duration-150">How It Works</a>
                    <a href="#" class="text-dark-text hover:text-pastel-blue font-medium transition duration-150">About Us</a>
                    <a href="#" class="px-5 py-2 bg-pastel-green text-dark-text font-semibold rounded-full shadow-md hover:bg-green-300 transition duration-150 transform hover:scale-105">
                        View Cart (0)
                    </a>
                </nav>

                <!-- Mobile Menu Button --><button id="menu-button" type="button" class="md:hidden p-2 rounded-lg text-dark-text hover:text-pastel-blue focus:outline-none focus:ring-2 focus:ring-inset focus:ring-pastel-blue" aria-controls="mobile-menu" aria-expanded="false" onclick="toggleMobileMenu()">
                    <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                    </svg>
                </button>
            </div>
        </div>

        <!-- Mobile Menu (Hidden by default) --><div class="hidden md:hidden" id="mobile-menu">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3 border-t border-gray-100">
                <a href="#featured" class="block px-3 py-2 rounded-md text-base font-medium text-dark-text hover:bg-gray-50">Worksheets</a>
                <a href="#how-it-works" class="block px-3 py-2 rounded-md text-base font-medium text-dark-text hover:bg-gray-50">How It Works</a>
                <a href="#" class="block px-3 py-2 rounded-md text-base font-medium text-dark-text hover:bg-gray-50">About Us</a>
                <a href="#" class="block w-full text-center mt-2 px-3 py-2 bg-pastel-green text-dark-text font-semibold rounded-full hover:bg-green-300 transition duration-150">View Cart (0)</a>
            </div>
        </div>
    </header>

    <main>
        <!-- Hero Section --><section class="bg-pastel-blue text-dark-text py-16 sm:py-24 text-center">
            <div class="max-w-4xl mx-auto px-4">
                <h1 class="text-4xl sm:text-6xl font-extrabold mb-4 leading-tight">
                    Learning for All Kids. Instantly Printable Resources.
                </h1>
                <p class="text-xl sm:text-2xl font-light mb-8 opacity-90">
                    High-quality, teacher-designed educational materials focused on making learning fun and accessible.
                </p>
                <a href="#featured" class="inline-block px-10 py-4 bg-pastel-yellow text-dark-text font-bold text-lg rounded-full shadow-lg hover:bg-yellow-300 transform hover:scale-105 transition duration-300 ease-in-out">
                    Start Exploring Now
                </a>
            </div>
        </section>

        <!-- Featured Products Section --><section id="featured" class="py-16 sm:py-24 bg-gray-50">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl sm:text-4xl font-bold text-dark-text mb-12 text-center">Our Most Popular Resources</h2>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">

                    <!-- Product Card 1: Math (Blue Accent) --><div class="bg-surface-bg rounded-xl shadow-lg overflow-hidden transform hover:scale-[1.02] transition duration-300 ease-in-out border-t-4 border-pastel-blue">
                        <!-- Placeholder Image --><img src="https://placehold.co/400x300/B3D9FF/4A5568?text=Math+Worksheets" onerror="this.onerror=null; this.src='https://via.placeholder.com/400x300.png?text=Math';" alt="Math Worksheets" class="w-full h-48 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-semibold text-dark-text mb-2">Fundamental Math</h3>
                            <p class="text-light-text text-sm mb-4">Grade K-5. Algebra basics, fractions, and counting sets.</p>
                            <span class="text-2xl font-bold text-pastel-green">$5.99</span>
                            <button class="mt-4 w-full py-3 bg-pastel-green text-dark-text font-semibold rounded-full hover:bg-green-300 transition duration-150 shadow-md">
                                Add to Cart
                            </button>
                        </div>
                    </div>

                    <!-- Product Card 2: Literacy (Green Accent) --><div class="bg-surface-bg rounded-xl shadow-lg overflow-hidden transform hover:scale-[1.02] transition duration-300 ease-in-out border-t-4 border-pastel-green">
                        <!-- Placeholder Image --><img src="https://placehold.co/400x300/C2F0C2/4A5568?text=Literacy+Packs" onerror="this.onerror=null; this.src='https://via.placeholder.com/400x300.png?text=Literacy';" alt="Literacy Worksheets" class="w-full h-48 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-semibold text-dark-text mb-2">Reading & Phonics</h3>
                            <p class="text-light-text text-sm mb-4">Build strong reading skills with targeted phonics worksheets.</p>
                            <span class="text-2xl font-bold text-pastel-green">$7.50</span>
                            <button class="mt-4 w-full py-3 bg-pastel-green text-dark-text font-semibold rounded-full hover:bg-green-300 transition duration-150 shadow-md">
                                Add to Cart
                            </button>
                        </div>
                    </div>

                    <!-- Product Card 3: Science (Yellow Accent) --><div class="bg-surface-bg rounded-xl shadow-lg overflow-hidden transform hover:scale-[1.02] transition duration-300 ease-in-out border-t-4 border-pastel-yellow">
                        <!-- Placeholder Image --><img src="https://placehold.co/400x300/FFECB3/4A5568?text=Science+Topics" onerror="this.onerror=null; this.src='https://via.placeholder.com/400x300.png?text=Science';" alt="Science Worksheets" class="w-full h-48 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-semibold text-dark-text mb-2">Elementary Science</h3>
                            <p class="text-light-text text-sm mb-4">Topics covering nature, space, and simple experiments.</p>
                            <span class="text-2xl font-bold text-pastel-green">$6.25</span>
                            <button class="mt-4 w-full py-3 bg-pastel-green text-dark-text font-semibold rounded-full hover:bg-green-300 transition duration-150 shadow-md">
                                Add to Cart
                            </button>
                        </div>
                    </div>

                    <!-- Product Card 4: Fine Motor (Pink Accent) --><div class="bg-surface-bg rounded-xl shadow-lg overflow-hidden transform hover:scale-[1.02] transition duration-300 ease-in-out border-t-4 border-pastel-pink">
                        <!-- Placeholder Image --><img src="https://placehold.co/400x300/FFC2E0/4A5568?text=Fine+Motor+Skills" onerror="this.onerror=null; this.src='https://via.placeholder.com/400x300.png?text=Fine+Motor';" alt="Fine Motor Worksheets" class="w-full h-48 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-semibold text-dark-text mb-2">Fine Motor Skills</h3>
                            <p class="text-light-text text-sm mb-4">Engaging printable activities for handwriting and cutting practice.</p>
                            <span class="text-2xl font-bold text-pastel-green">$3.99</span>
                            <button class="mt-4 w-full py-3 bg-pastel-green text-dark-text font-semibold rounded-full hover:bg-green-300 transition duration-150 shadow-md">
                                Add to Cart
                            </button>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- How It Works Section --><section id="how-it-works" class="py-16 sm:py-24 bg-surface-bg">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl sm:text-4xl font-bold text-dark-text mb-12 text-center">Simple Steps to Start Learning</h2>

                <div class="grid grid-cols-1 md:grid-cols-3 gap-10 text-center">

                    <!-- Step 1 --><div class="p-6 bg-gray-50 rounded-xl shadow-lg border-b-4 border-pastel-blue">
                        <div class="text-5xl mb-4 text-pastel-blue font-black">1</div>
                        <h3 class="text-xl font-semibold text-dark-text mb-3">Find Your Resource</h3>
                        <p class="text-light-text">Browse hundreds of worksheets organized by grade level and subject, finding exactly what your child needs.</p>
                    </div>

                    <!-- Step 2 --><div class="p-6 bg-gray-50 rounded-xl shadow-lg border-b-4 border-pastel-green">
                        <div class="text-5xl mb-4 text-pastel-green font-black">2</div>
                        <h3 class="text-xl font-semibold text-dark-text mb-3">Download Instantly</h3>
                        <p class="text-light-text">Complete your secure checkout and your high-resolution PDF files are available for immediate download.</p>
                    </div>

                    <!-- Step 3 --><div class="p-6 bg-gray-50 rounded-xl shadow-lg border-b-4 border-pastel-yellow">
                        <div class="text-5xl mb-4 text-pastel-yellow font-black">3</div>
                        <h3 class="text-xl font-semibold text-dark-text mb-3">Print & Educate</h3>
                        <p class="text-light-text">Print as many copies as you need, and start using them for class, tutoring, or homeschooling!</p>
                    </div>

                </div>
            </div>
        </section>

    </main>

    <!-- Footer --><footer class="bg-gray-800 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8 mb-8">
                <div>
                    <h4 class="font-bold text-lg mb-4 text-pastel-blue">Shop</h4>
                    <ul class="space-y-2 text-sm">
                        <li><a href="#featured" class="hover:text-pastel-green transition duration-150">All Worksheets</a></li>
                        <li><a href="#" class="hover:text-pastel-green transition duration-150">Bundles</a></li>
                        <li><a href="#" class="hover:text-pastel-green transition duration-150">New Releases</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold text-lg mb-4 text-pastel-blue">Customer Service</h4>
                    <ul class="space-y-2 text-sm">
                        <li><a href="#" class="hover:text-pastel-green transition duration-150">FAQ</a></li>
                        <li><a href="#" class="hover:text-pastel-green transition duration-150">Download Help</a></li>
                        <li><a href="#" class="hover:text-pastel-green transition duration-150">Refund Policy</a></li>
                    </ul>
                </div>
                <div class="col-span-2 md:col-span-2">
                    <h4 class="font-bold text-lg mb-4 text-pastel-blue">Stay Connected</h4>
                    <p class="text-sm mb-4">Sign up for our newsletter to get the latest deals and new worksheet alerts.</p>
                    <form onsubmit="event.preventDefault(); alert('Thanks for signing up for Bright Minds Corner newsletter!');" class="flex">
                        <input type="email" placeholder="Your Email Address" required class="p-3 w-full rounded-l-lg text-gray-800 focus:ring-pastel-blue focus:border-pastel-blue border-transparent">
                        <button type="submit" class="p-3 bg-pastel-green text-dark-text rounded-r-lg hover:bg-green-300 transition duration-150 font-semibold">
                            Sign Up
                        </button>
                    </form>
                </div>
            </div>

            <div class="border-t border-gray-700 pt-6 text-center text-sm">
                <img src="https://i.imgur.com/uRj0yI7.png" alt="Bright Minds Corner Logo" class="h-10 w-auto mx-auto mb-4 opacity-80">
                &copy; 2025 Bright Minds Corner. Learning for All Kids.
            </div>
        </div>
    </footer>

</body>
</html>

