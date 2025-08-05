<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sarah Johnson - Virtual Assistant</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        body { font-family: 'Inter', sans-serif; }
        .gradient-bg { background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); }
        .card-hover { transition: transform 0.3s ease, box-shadow 0.3s ease; }
        .card-hover:hover { transform: translateY(-5px); box-shadow: 0 20px 40px rgba(0,0,0,0.1); }
        .skill-bar { transition: width 1s ease-in-out; }
        .fade-in { opacity: 0; transform: translateY(20px); transition: opacity 0.6s ease, transform 0.6s ease; }
        .fade-in.visible { opacity: 1; transform: translateY(0); }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Navigation -->
    <nav class="bg-white shadow-lg fixed w-full top-0 z-50">
        <div class="max-w-6xl mx-auto px-4">
            <div class="flex justify-between items-center py-4">
                <div class="text-2xl font-bold text-gray-800">Sarah Johnson</div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="text-gray-600 hover:text-purple-600 transition duration-300">Home</a>
                    <a href="#about" class="text-gray-600 hover:text-purple-600 transition duration-300">About</a>
                    <a href="#services" class="text-gray-600 hover:text-purple-600 transition duration-300">Services</a>
                    <a href="#portfolio" class="text-gray-600 hover:text-purple-600 transition duration-300">Portfolio</a>
                    <a href="#contact" class="text-gray-600 hover:text-purple-600 transition duration-300">Contact</a>
                </div>
                <button id="mobile-menu-btn" class="md:hidden text-gray-600">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
            <div id="mobile-menu" class="hidden md:hidden pb-4">
                <a href="#home" class="block py-2 text-gray-600 hover:text-purple-600">Home</a>
                <a href="#about" class="block py-2 text-gray-600 hover:text-purple-600">About</a>
                <a href="#services" class="block py-2 text-gray-600 hover:text-purple-600">Services</a>
                <a href="#portfolio" class="block py-2 text-gray-600 hover:text-purple-600">Portfolio</a>
                <a href="#contact" class="block py-2 text-gray-600 hover:text-purple-600">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="gradient-bg min-h-screen flex items-center pt-16">
        <div class="max-w-6xl mx-auto px-4 text-center text-white">
            <div class="fade-in">
                <div class="w-32 h-32 mx-auto mb-8 bg-white rounded-full flex items-center justify-center text-6xl">
                    👩‍💼
                </div>
                <h1 class="text-5xl md:text-6xl font-bold mb-6">Sarah Johnson</h1>
                <p class="text-xl md:text-2xl mb-8 opacity-90">Professional Virtual Assistant</p>
                <p class="text-lg mb-12 max-w-2xl mx-auto opacity-80">
                    Helping businesses streamline operations, manage tasks, and achieve their goals with reliable virtual assistance services.
                </p>
                <div class="space-x-4">
                    <a href="#services" class="bg-white text-purple-600 px-8 py-3 rounded-full font-semibold hover:bg-gray-100 transition duration-300">
                        View Services
                    </a>
                    <a href="#contact" class="border-2 border-white text-white px-8 py-3 rounded-full font-semibold hover:bg-white hover:text-purple-600 transition duration-300">
                        Get In Touch
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">About Me</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">
                    With over 5 years of experience in virtual assistance, I help businesses and entrepreneurs focus on what they do best while I handle the rest.
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div class="fade-in">
                    <div class="bg-gradient-to-br from-purple-100 to-blue-100 rounded-2xl p-8 text-center">
                        <div class="text-8xl mb-4">🎯</div>
                        <h3 class="text-2xl font-semibold text-gray-800 mb-4">Mission Focused</h3>
                        <p class="text-gray-600">Dedicated to helping you achieve your business goals through efficient and reliable virtual support.</p>
                    </div>
                </div>
                
                <div class="fade-in">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-6">Skills & Expertise</h3>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Administrative Tasks</span>
                                <span class="text-gray-500">95%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar bg-purple-600 h-2 rounded-full" style="width: 95%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Customer Support</span>
                                <span class="text-gray-500">90%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar bg-blue-600 h-2 rounded-full" style="width: 90%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Social Media Management</span>
                                <span class="text-gray-500">85%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar bg-green-600 h-2 rounded-full" style="width: 85%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Data Entry & Research</span>
                                <span class="text-gray-500">92%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar bg-indigo-600 h-2 rounded-full" style="width: 92%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-gray-50">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">My Services</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">
                    Comprehensive virtual assistance services tailored to meet your business needs and help you succeed.
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white rounded-xl p-8 shadow-lg card-hover fade-in">
                    <div class="text-4xl mb-4">📋</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Administrative Support</h3>
                    <p class="text-gray-600 mb-6">Email management, scheduling, document preparation, and general administrative tasks.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Email management</li>
                        <li>• Calendar scheduling</li>
                        <li>• Document creation</li>
                        <li>• Travel planning</li>
                    </ul>
                </div>
                
                <div class="bg-white rounded-xl p-8 shadow-lg card-hover fade-in">
                    <div class="text-4xl mb-4">💬</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Customer Support</h3>
                    <p class="text-gray-600 mb-6">Professional customer service, live chat support, and client communication management.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Live chat support</li>
                        <li>• Email responses</li>
                        <li>• Order processing</li>
                        <li>• Customer inquiries</li>
                    </ul>
                </div>
                
                <div class="bg-white rounded-xl p-8 shadow-lg card-hover fade-in">
                    <div class="text-4xl mb-4">📱</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Social Media Management</h3>
                    <p class="text-gray-600 mb-6">Content creation, posting schedules, engagement, and social media strategy implementation.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Content creation</li>
                        <li>• Post scheduling</li>
                        <li>• Community engagement</li>
                        <li>• Analytics reporting</li>
                    </ul>
                </div>
                
                <div class="bg-white rounded-xl p-8 shadow-lg card-hover fade-in">
                    <div class="text-4xl mb-4">🔍</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Research & Data Entry</h3>
                    <p class="text-gray-600 mb-6">Market research, lead generation, data collection, and accurate data entry services.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Market research</li>
                        <li>• Lead generation</li>
                        <li>• Data entry</li>
                        <li>• Database management</li>
                    </ul>
                </div>
                
                <div class="bg-white rounded-xl p-8 shadow-lg card-hover fade-in">
                    <div class="text-4xl mb-4">✍️</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Content Writing</h3>
                    <p class="text-gray-600 mb-6">Blog posts, website content, product descriptions, and marketing copy creation.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Blog writing</li>
                        <li>• Website content</li>
                        <li>• Product descriptions</li>
                        <li>• Marketing copy</li>
                    </ul>
                </div>
                
                <div class="bg-white rounded-xl p-8 shadow-lg card-hover fade-in">
                    <div class="text-4xl mb-4">📊</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Project Management</h3>
                    <p class="text-gray-600 mb-6">Task coordination, timeline management, team communication, and project tracking.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Task coordination</li>
                        <li>• Timeline management</li>
                        <li>• Team communication</li>
                        <li>• Progress tracking</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Success Stories</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">
                    Here are some examples of how I've helped businesses streamline their operations and achieve their goals.
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-gradient-to-br from-blue-50 to-indigo-50 rounded-xl p-6 card-hover fade-in">
                    <div class="text-3xl mb-4">🏢</div>
                    <h3 class="text-lg font-semibold text-gray-800 mb-3">E-commerce Business</h3>
                    <p class="text-gray-600 text-sm mb-4">Managed customer support and order processing for an online store, increasing customer satisfaction by 40%.</p>
                    <div class="text-xs text-gray-500">
                        <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded">Customer Support</span>
                        <span class="bg-green-100 text-green-800 px-2 py-1 rounded ml-2">Order Management</span>
                    </div>
                </div>
                
                <div class="bg-gradient-to-br from-purple-50 to-pink-50 rounded-xl p-6 card-hover fade-in">
                    <div class="text-3xl mb-4">📈</div>
                    <h3 class="text-lg font-semibold text-gray-800 mb-3">Marketing Agency</h3>
                    <p class="text-gray-600 text-sm mb-4">Provided social media management and content creation, helping increase client engagement by 60%.</p>
                    <div class="text-xs text-gray-500">
                        <span class="bg-purple-100 text-purple-800 px-2 py-1 rounded">Social Media</span>
                        <span class="bg-pink-100 text-pink-800 px-2 py-1 rounded ml-2">Content Creation</span>
                    </div>
                </div>
                
                <div class="bg-gradient-to-br from-green-50 to-teal-50 rounded-xl p-6 card-hover fade-in">
                    <div class="text-3xl mb-4">💼</div>
                    <h3 class="text-lg font-semibold text-gray-800 mb-3">Consulting Firm</h3>
                    <p class="text-gray-600 text-sm mb-4">Streamlined administrative processes and managed client communications, saving 20 hours per week.</p>
                    <div class="text-xs text-gray-500">
                        <span class="bg-green-100 text-green-800 px-2 py-1 rounded">Admin Support</span>
                        <span class="bg-teal-100 text-teal-800 px-2 py-1 rounded ml-2">Client Management</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="py-20 bg-gray-50">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">What Clients Say</h2>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white rounded-xl p-6 shadow-lg fade-in">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 bg-blue-500 rounded-full flex items-center justify-center text-white font-bold">MJ</div>
                        <div class="ml-4">
                            <h4 class="font-semibold text-gray-800">Michael Johnson</h4>
                            <p class="text-sm text-gray-500">CEO, TechStart Inc.</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"Sarah has been instrumental in helping us scale our operations. Her attention to detail and proactive approach saved us countless hours."</p>
                    <div class="flex text-yellow-400 mt-4">
                        ⭐⭐⭐⭐⭐
                    </div>
                </div>
                
                <div class="bg-white rounded-xl p-6 shadow-lg fade-in">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 bg-purple-500 rounded-full flex items-center justify-center text-white font-bold">ER</div>
                        <div class="ml-4">
                            <h4 class="font-semibold text-gray-800">Emily Rodriguez</h4>
                            <p class="text-sm text-gray-500">Founder, Creative Studio</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"Working with Sarah has been a game-changer. She manages our social media perfectly and our engagement has never been higher."</p>
                    <div class="flex text-yellow-400 mt-4">
                        ⭐⭐⭐⭐⭐
                    </div>
                </div>
                
                <div class="bg-white rounded-xl p-6 shadow-lg fade-in">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 bg-green-500 rounded-full flex items-center justify-center text-white font-bold">DL</div>
                        <div class="ml-4">
                            <h4 class="font-semibold text-gray-800">David Lee</h4>
                            <p class="text-sm text-gray-500">Owner, Online Boutique</p>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"Sarah's customer support skills are exceptional. Our customers love the quick and professional responses she provides."</p>
                    <div class="flex text-yellow-400 mt-4">
                        ⭐⭐⭐⭐⭐
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-white">
        <div class="max-w-4xl mx-auto px-4">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Let's Work Together</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">
                    Ready to streamline your business operations? Get in touch and let's discuss how I can help you achieve your goals.
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 gap-12">
                <div class="fade-in">
                    <h3 class="text-2xl font-semibold text-gray-800 mb-6">Get In Touch</h3>
                    <div class="space-y-4">
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-purple-100 rounded-lg flex items-center justify-center mr-4">
                                📧
                            </div>
                            <div>
                                <p class="font-semibold text-gray-800">Email</p>
                                <p class="text-gray-600">sarah@virtualassistant.com</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <d
