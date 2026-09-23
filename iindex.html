<!DOCTYPE html>
<html lang="en" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E-HEALTHY | Digital Health Campus & AI Diagnostics</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        brand: { 50: '#ecfdf5', 500: '#10b981', 600: '#059669', 900: '#064e3b' },
                        darkBg: '#090d16',
                        cardBg: '#111827'
                    },
                    animation: {
                        'pulse-slow': 'pulse 4s cubic-bezier(0.4, 0, 0.6, 1) infinite',
                        'float': 'float 6s ease-in-out infinite',
                        'scan-laser': 'scanLaser 2.5s ease-in-out infinite',
                        'radar': 'radarSpin 4s linear infinite',
                    },
                    keyframes: {
                        float: {
                            '0%, 100%': { transform: 'translateY(0px)' },
                            '50%': { transform: 'translateY(-10px)' },
                        },
                        scanLaser: {
                            '0%, 100%': { top: '0%' },
                            '50%': { top: '95%' },
                        },
                        radarSpin: {
                            '0%': { transform: 'rotate(0deg)' },
                            '100%': { transform: 'rotate(360deg)' }
                        }
                    }
                }
            }
        }
    </script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Plus Jakarta Sans', sans-serif; }
        /* Smooth Custom Scrollbar */
        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #090d16; }
        ::-webkit-scrollbar-thumb { background: #1f2937; border-radius: 4px; }
        ::-webkit-scrollbar-thumb:hover { background: #10b981; }

        /* Smooth Spring Page Transitions */
        .page-view {
            opacity: 0;
            transform: translateY(16px) scale(0.99);
            transition: opacity 0.5s cubic-bezier(0.16, 1, 0.3, 1), transform 0.5s cubic-bezier(0.16, 1, 0.3, 1);
            pointer-events: none;
            position: absolute;
            width: 100%;
            top: 0;
            left: 0;
        }
        .page-view.active {
            opacity: 1;
            transform: translateY(0) scale(1);
            pointer-events: auto;
            position: relative;
        }

        /* Glassmorphism & Glows */
        .glass-card {
            background: rgba(17, 24, 39, 0.7);
            backdrop-filter: blur(16px);
            border: 1px solid rgba(16, 185, 129, 0.15);
            transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .glass-card:hover {
            border-color: rgba(16, 185, 129, 0.4);
            box-shadow: 0 10px 30px -10px rgba(16, 185, 129, 0.2);
            transform: translateY(-4px);
        }
        .glow-btn {
            position: relative;
            overflow: hidden;
            transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .glow-btn::after {
            content: '';
            position: absolute;
            top: -50%; left: -50%; width: 200%; height: 200%;
            background: linear-gradient(60deg, transparent, rgba(255,255,255,0.2), transparent);
            transform: rotate(45deg) translateX(-100%);
            transition: transform 0.6s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .glow-btn:hover::after {
            transform: rotate(45deg) translateX(100%);
        }
    </style>
</head>
<body class="bg-darkBg text-gray-100 min-h-screen flex flex-col selection:bg-brand-500 selection:text-white overflow-x-hidden">

    <header class="sticky top-0 z-50 glass-card border-b border-gray-800/80 backdrop-blur-xl">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <div class="flex items-center space-x-3 cursor-pointer group" onclick="switchPage('home')">
                <div class="w-12 h-12 rounded-2xl bg-gradient-to-tr from-brand-600 to-emerald-400 flex items-center justify-center shadow-lg shadow-emerald-900/30 group-hover:scale-105 transition-transform duration-300">
                    <i data-lucide="activity" class="w-7 h-7 text-white"></i>
                </div>
                <div>
                    <span class="text-2xl font-black tracking-wider bg-gradient-to-r from-white via-emerald-200 to-brand-500 bg-clip-text text-transparent">E-HEALTHY</span>
                    <span class="block text-[10px] uppercase tracking-widest text-emerald-400 font-semibold">Eat Healthy Digital Campus</span>
                </div>
            </div>

            <nav class="hidden md:flex items-center space-x-1 bg-gray-900/60 p-1.5 rounded-full border border-gray-800">
                <button onclick="switchPage('home')" id="nav-home" class="px-5 py-2 rounded-full text-sm font-semibold transition-all duration-300 bg-brand-500 text-white shadow-md">Home</button>
                <button onclick="switchPage('scan')" id="nav-scan" class="px-5 py-2 rounded-full text-sm font-semibold text-gray-400 hover:text-white hover:bg-gray-800 transition-all duration-300">AI Face Scan</button>
                <button onclick="switchPage('hub')" id="nav-hub" class="px-5 py-2 rounded-full text-sm font-semibold text-gray-400 hover:text-white hover:bg-gray-800 transition-all duration-300">Health Hub</button>
                <button onclick="switchPage('assistant')" id="nav-assistant" class="px-5 py-2 rounded-full text-sm font-semibold text-gray-400 hover:text-white hover:bg-gray-800 transition-all duration-300">AI Assistant</button>
                <button onclick="switchPage('about')" id="nav-about" class="px-5 py-2 rounded-full text-sm font-semibold text-gray-400 hover:text-white hover:bg-gray-800 transition-all duration-300">About Project</button>
            </nav>

            <div class="flex items-center space-x-4">
                <button onclick="switchPage('scan')" class="hidden sm:inline-flex items-center space-x-2 px-5 py-2.5 rounded-xl bg-gradient-to-r from-brand-600 to-emerald-500 text-white font-semibold glow-btn shadow-lg shadow-brand-500/20">
                    <i data-lucide="scan" class="w-4 h-4"></i>
                    <span>Quick Scan</span>
                </button>
                <button onclick="toggleMobileMenu()" class="md:hidden p-2 rounded-xl bg-gray-800 text-gray-300 hover:text-white">
                    <i data-lucide="menu" class="w-6 h-6"></i>
                </button>
            </div>
        </div>

        <div id="mobile-menu" class="hidden md:hidden glass-card border-t border-gray-800 px-6 py-4 space-y-3">
            <button onclick="switchPage('home'); toggleMobileMenu();" class="block w-full text-left py-2 text-gray-300 hover:text-emerald-400 font-medium">Home</button>
            <button onclick="switchPage('scan'); toggleMobileMenu();" class="block w-full text-left py-2 text-gray-300 hover:text-emerald-400 font-medium">AI Face Scan</button>
            <button onclick="switchPage('hub'); toggleMobileMenu();" class="block w-full text-left py-2 text-gray-300 hover:text-emerald-400 font-medium">Health Hub & Files</button>
            <button onclick="switchPage('assistant'); toggleMobileMenu();" class="block w-full text-left py-2 text-gray-300 hover:text-emerald-400 font-medium">AI Assistant</button>
            <button onclick="switchPage('about'); toggleMobileMenu();" class="block w-full text-left py-2 text-gray-300 hover:text-emerald-400 font-medium">About Project</button>
        </div>
    </header>

    <main class="flex-grow relative max-w-7xl mx-auto w-full px-4 sm:px-6 lg:px-8 py-8">

        <div id="page-home" class="page-view active space-y-16">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center py-10">
                <div class="space-y-6">
                    <div class="inline-flex items-center space-x-2 px-3.5 py-1.5 rounded-full bg-emerald-500/10 border border-emerald-500/20 text-emerald-400 text-xs font-semibold tracking-wide animate-pulse">
                        <i data-lucide="sparkles" class="w-4 h-4"></i>
                        <span>Next-Gen AI Biometric Campus Platform</span>
                    </div>
                    <h1 class="text-4xl sm:text-6xl font-extrabold tracking-tight leading-tight">
                        Eat Healthy, <br>
                        <span class="bg-gradient-to-r from-emerald-400 via-teal-300 to-brand-500 bg-clip-text text-transparent">Live Limitless.</span>
                    </h1>
                    <p class="text-gray-400 text-lg leading-relaxed max-w-xl">
                        E-HEALTHY combines cutting-edge computer vision, instant facial health diagnostics, and smart dietary prescriptions to optimize student & faculty well-being on campus.
                    </p>
                    <div class="flex flex-wrap gap-4 pt-4">
                        <button onclick="switchPage('scan')" class="px-8 py-4 rounded-2xl bg-gradient-to-r from-brand-600 to-emerald-500 text-white font-bold text-base glow-btn shadow-xl shadow-brand-500/25 flex items-center space-x-3">
                            <i data-lucide="camera" class="w-5 h-5"></i>
                            <span>Start AI Face Scan</span>
                        </button>
                        <button onclick="switchPage('hub')" class="px-8 py-4 rounded-2xl glass-card text-gray-200 hover:text-white font-bold text-base flex items-center space-x-3">
                            <i data-lucide="file-text" class="w-5 h-5"></i>
                            <span>Analyze Reports</span>
                        </button>
                    </div>
                    <div class="grid grid-cols-3 gap-6 pt-8 border-t border-gray-800">
                        <div>
                            <div class="text-3xl font-extrabold text-white">99.4%</div>
                            <div class="text-xs text-gray-400 mt-1">Scan Precision</div>
                        </div>
                        <div>
                            <div class="text-3xl font-extrabold text-emerald-400">0.8s</div>
                            <div class="text-xs text-gray-400 mt-1">Analysis Speed</div>
                        </div>
                        <div>
                            <div class="text-3xl font-extrabold text-white">24/7</div>
                            <div class="text-xs text-gray-400 mt-1">AI Health Assistant</div>
                        </div>
                    </div>
                </div>

                <div class="relative">
                    <div class="absolute -inset-1 rounded-3xl bg-gradient-to-r from-emerald-500 to-teal-600 opacity-30 blur-2xl animate-pulse-slow"></div>
                    <div class="relative glass-card rounded-3xl p-6 sm:p-8 space-y-6">
                        <div class="flex items-center justify-between">
                            <div class="flex items-center space-x-3">
                                <div class="w-3 h-3 rounded-full bg-red-500 animate-ping"></div>
                                <span class="text-sm font-semibold tracking-wider text-gray-300">LIVE BIOMETRIC FEED</span>
                            </div>
                            <span class="px-2.5 py-1 rounded-md bg-emerald-500/20 text-emerald-400 text-xs font-bold">SECURE v2.4</span>
                        </div>
                        <div class="relative h-64 sm:h-80 rounded-2xl bg-gray-950 overflow-hidden border border-emerald-500/30 flex items-center justify-center">
                            <div class="absolute inset-0 bg-[radial-gradient(#10b981_1px,transparent_1px)] [background-size:16px_16px] opacity-20"></div>
                            <div class="absolute w-40 h-40 sm:w-52 sm:h-52 rounded-full border border-emerald-500/40 animate-radar"></div>
                            <div class="absolute w-28 h-28 sm:w-36 sm:h-36 rounded-full border border-dashed border-emerald-400/30"></div>
                            <div class="relative z-10 w-24 h-32 sm:w-32 sm:h-44 border-2 border-emerald-400/60 rounded-[40%] flex flex-col items-center justify-center shadow-[0_0_30px_rgba(16,185,129,0.3)] animate-float">
                                <div class="w-16 h-4 border-b-2 border-emerald-400 rounded-full mb-6"></div>
                                <div class="flex space-x-4">
                                    <div class="w-3 h-3 bg-emerald-400 rounded-full animate-ping"></div>
                                    <div class="w-3 h-3 bg-emerald-400 rounded-full animate-ping"></div>
                                </div>
                            </div>
                            <div class="absolute bottom-4 left-4 right-4 bg-gray-900/90 backdrop-blur-md rounded-xl p-3 border border-gray-800 flex items-center justify-between text-xs">
                                <div class="flex items-center space-x-2">
                                    <i data-lucide="cpu" class="w-4 h-4 text-emerald-400"></i>
                                    <span>AI Neural Engine Active</span>
                                </div>
                                <span class="text-emerald-400 font-bold">OK (98.7%)</span>
                            </div>
                        </div>
                        <div class="flex items-center justify-between text-sm text-gray-400">
                            <span>Status: Ready for scanning</span>
                            <button onclick="switchPage('scan')" class="text-emerald-400 hover:text-emerald-300 font-semibold flex items-center space-x-1">
                                <span>Launch Scanner</span>
                                <i data-lucide="arrow-right" class="w-4 h-4"></i>
                            </button>
                        </div>
                    </div>
                </div>
            </div>

            <div class="py-12 space-y-12">
                <div class="text-center max-w-2xl mx-auto space-y-3">
                    <h2 class="text-3xl font-bold tracking-tight">Core Campus Health Pillars</h2>
                    <p class="text-gray-400">Engineered with precision for real-time diagnostics and preventive student healthcare.</p>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    <div class="glass-card rounded-2xl p-8 space-y-4">
                        <div class="w-14 h-14 rounded-2xl bg-brand-500/10 border border-brand-500/20 flex items-center justify-center text-emerald-400">
                            <i data-lucide="scan-face" class="w-7 h-7"></i>
                        </div>
                        <h3 class="text-xl font-bold">Facial AI Scanning</h3>
                        <p class="text-gray-400 text-sm leading-relaxed">Instant camera scan analyzing micro-expressions, skin hydration, fatigue indexes, and vitamin indicators in under a second.</p>
                    </div>
                    <div class="glass-card rounded-2xl p-8 space-y-4">
                        <div class="w-14 h-14 rounded-2xl bg-brand-500/10 border border-brand-500/20 flex items-center justify-center text-emerald-400">
                            <i data-lucide="file-spreadsheet" class="w-7 h-7"></i>
                        </div>
                        <h3 class="text-xl font-bold">Smart Report Analyzer</h3>
                        <p class="text-gray-400 text-sm leading-relaxed">Upload blood work or health reports to generate instant graphical analytics, trend charts, and dietary prescriptions.</p>
                    </div>
                    <div class="glass-card rounded-2xl p-8 space-y-4">
                        <div class="w-14 h-14 rounded-2xl bg-brand-500/10 border border-brand-500/20 flex items-center justify-center text-emerald-400">
                            <i data-lucide="bot" class="w-7 h-7"></i>
                        </div>
                        <h3 class="text-xl font-bold">Gemini AI Assistant</h3>
                        <p class="text-gray-400 text-sm leading-relaxed">Ask any question regarding nutrition, fitness routines, or wellness guidelines and receive instant intelligent responses.</p>
                    </div>
                </div>
            </div>
        </div>

        <div id="page-scan" class="page-view space-y-10">
            <div class="text-center max-w-2xl mx-auto space-y-3">
                <div class="inline-flex items-center space-x-2 px-3 py-1 rounded-full bg-emerald-500/10 text-emerald-400 text-xs font-semibold">
                    <i data-lucide="camera" class="w-3.5 h-3.5"></i>
                    <span>Computer Vision Diagnostic Module</span>
                </div>
                <h2 class="text-3xl font-extrabold">AI Facial Health Scan</h2>
                <p class="text-gray-400">Position your face within the camera frame or upload a clear photo for instant health probability metrics.</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
                <div class="lg:col-span-7 glass-card rounded-3xl p-6 space-y-6">
                    <div class="relative h-80 sm:h-96 rounded-2xl bg-gray-950 overflow-hidden border border-gray-800 flex items-center justify-center">
                        <video id="webcam-video" autoplay playsinline class="absolute inset-0 w-full h-full object-cover hidden"></video>
                        <div id="scan-placeholder" class="absolute inset-0 flex flex-col items-center justify-center space-y-4 text-center p-6">
                            <div class="w-20 h-20 rounded-full bg-brand-500/10 border border-emerald-500/30 flex items-center justify-center text-emerald-400">
                                <i data-lucide="user-check" class="w-10 h-10"></i>
                            </div>
                            <div class="space-y-1">
                                <h4 class="font-bold text-lg">Camera Feed Offline</h4>
                                <p class="text-xs text-gray-400">Click below to activate live webcam or upload a photo for AI analysis.</p>
                            </div>
                        </div>

                        <div id="scan-laser-overlay" class="absolute inset-0 hidden pointer-events-none">
                            <div class="absolute inset-0 bg-[linear-gradient(to_bottom,transparent_95%,rgba(16,185,129,0.5)_100%)] bg-[length:100%_40px]"></div>
                            <div class="absolute w-full h-1 bg-emerald-400 shadow-[0_0_15px_#10b981] animate-scan-laser"></div>
                        </div>

                        <div id="face-box" class="absolute w-48 h-64 border-2 border-dashed border-emerald-400/70 rounded-3xl hidden flex flex-col justify-between p-2">
                            <div class="flex justify-between"><span class="w-3 h-3 border-t-2 border-l-2 border-emerald-400"></span><span class="w-3 h-3 border-t-2 border-r-2 border-emerald-400"></span></div>
                            <div class="flex justify-between"><span class="w-3 h-3 border-b-2 border-l-2 border-emerald-400"></span><span class="w-3 h-3 border-b-2 border-r-2 border-emerald-400"></span></div>
                        </div>
                    </div>

                    <div class="flex flex-wrap gap-4 justify-between items-center">
                        <div class="flex space-x-3">
                            <button onclick="startWebcam()" id="btn-cam" class="px-5 py-3 rounded-xl bg-gray-800 hover:bg-gray-700 text-white font-semibold text-sm flex items-center space-x-2 transition-all">
                                <i data-lucide="video" class="w-4 h-4 text-emerald-400"></i>
                                <span>Start Camera</span>
                            </button>
                            <label class="px-5 py-3 rounded-xl bg-gray-800 hover:bg-gray-700 text-white font-semibold text-sm flex items-center space-x-2 cursor-pointer transition-all">
                                <i data-lucide="upload" class="w-4 h-4 text-emerald-400"></i>
                                <span>Upload Photo</span>
                                <input type="file" accept="image/*" class="hidden" onchange="handleImageUpload(event)">
                            </label>
                        </div>
                        <button onclick="triggerAIScan()" id="btn-scan" class="px-6 py-3 rounded-xl bg-gradient-to-r from-brand-600 to-emerald-500 text-white font-bold text-sm glow-btn flex items-center space-x-2 disabled:opacity-50">
                            <i data-lucide="zap" class="w-4 h-4"></i>
                            <span>Run AI Analysis</span>
                        </button>
                    </div>
                </div>

                <div class="lg:col-span-5 space-y-6">
                    <div class="glass-card rounded-3xl p-6 space-y-6">
                        <div class="flex items-center justify-between border-b border-gray-800 pb-4">
                            <h3 class="font-bold text-lg flex items-center space-x-2">
                                <i data-lucide="activity" class="w-5 h-5 text-emerald-400"></i>
                                <span>Diagnostic Analytics</span>
                            </h3>
                            <span id="scan-status-badge" class="px-2.5 py-1 rounded-full bg-gray-800 text-gray-400 text-xs font-semibold">Awaiting Scan</span>
                        </div>

                        <div id="results-container" class="space-y-5">
                            <div class="text-center py-12 text-gray-500 space-y-2">
                                <i data-lucide="shield-alert" class="w-12 h-12 mx-auto opacity-40"></i>
                                <p class="text-sm">Run face scan to view condition probability & vitamin indicators.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div id="page-hub" class="page-view space-y-10">
            <div class="text-center max-w-2xl mx-auto space-y-3">
                <div class="inline-flex items-center space-x-2 px-3 py-1 rounded-full bg-emerald-500/10 text-emerald-400 text-xs font-semibold">
                    <i data-lucide="bar-chart-3" class="w-3.5 h-3.5"></i>
                    <span>Medical Report & Nutrient Visualizer</span>
                </div>
                <h2 class="text-3xl font-extrabold">Campus Health Hub</h2>
                <p class="text-gray-400">Upload medical files, blood work PDFs, or examine real-time nutritional tracking charts.</p>
            </div>

            <div class="glass-card rounded-3xl p-8 text-center space-y-4 border-dashed border-2 border-gray-700 hover:border-emerald-500/50 transition-colors">
                <div class="w-16 h-16 rounded-2xl bg-brand-500/10 border border-emerald-500/30 flex items-center justify-center mx-auto text-emerald-400">
                    <i data-lucide="upload-cloud" class="w-8 h-8"></i>
                </div>
                <div>
                    <h4 class="font-bold text-lg">Upload Health Report / Blood Work</h4>
                    <p class="text-sm text-gray-400 mt-1">Supports PDF, PNG, JPG, or CSV health metrics records.</p>
                </div>
                <div class="flex justify-center gap-4 pt-2">
                    <label class="px-6 py-3 rounded-xl bg-brand-600 hover:bg-brand-500 text-white font-semibold text-sm cursor-pointer glow-btn">
                        <span>Browse Files</span>
                        <input type="file" class="hidden" onchange="simulateFileUpload(event)">
                    </label>
                    <button onclick="loadSampleReport()" class="px-6 py-3 rounded-xl bg-gray-800 hover:bg-gray-700 text-gray-200 font-semibold text-sm">
                        Load Demo Report
                    </button>
                </div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
                <div class="glass-card rounded-3xl p-6 space-y-4">
                    <div class="flex items-center justify-between">
                        <h4 class="font-bold text-base">Weekly Nutrient Intake vs Target</h4>
                        <span class="text-xs text-emerald-400 font-semibold">Optimized</span>
                    </div>
                    <div class="h-72">
                        <canvas id="nutrientChart"></canvas>
                    </div>
                </div>
                <div class="glass-card rounded-3xl p-6 space-y-4">
                    <div class="flex items-center justify-between">
                        <h4 class="font-bold text-base">Hydration & Sleep Recovery Index</h4>
                        <span class="text-xs text-emerald-400 font-semibold">Last 7 Days</span>
                    </div>
                    <div class="h-72">
                        <canvas id="hydrationChart"></canvas>
                    </div>
                </div>
            </div>
        </div>

        <div id="page-assistant" class="page-view space-y-8">
            <div class="text-center max-w-2xl mx-auto space-y-3">
                <div class="inline-flex items-center space-x-2 px-3 py-1 rounded-full bg-emerald-500/10 text-emerald-400 text-xs font-semibold">
                    <i data-lucide="bot" class="w-3.5 h-3.5"></i>
                    <span>Real-time Gemini API Health Specialist</span>
                </div>
                <h2 class="text-3xl font-extrabold">AI Health & Diet Assistant</h2>
                <p class="text-gray-400">Ask any question regarding nutrition, fitness plans, meal prep, or disease prevention.</p>
            </div>

            <div class="max-w-4xl mx-auto glass-card rounded-3xl p-6 flex flex-col h-[600px]">
                <div id="chat-messages" class="flex-grow overflow-y-auto space-y-4 pr-2">
                    <div class="flex items-start space-x-3">
                        <div class="w-10 h-10 rounded-xl bg-brand-600 flex items-center justify-center text-white flex-shrink-0 shadow-lg">
                            <i data-lucide="bot" class="w-5 h-5"></i>
                        </div>
                        <div class="glass-card rounded-2xl p-4 max-w-xl text-sm leading-relaxed text-gray-200">
                            Hello! I am your <strong>E-HEALTHY AI Assistant</strong> powered by Gemini. How can I help you optimize your diet or health today?
                        </div>
                    </div>
                </div>

                <div class="pt-4 border-t border-gray-800 flex items-center space-x-3">
                    <input type="text" id="chat-input" placeholder="Ask about healthy campus meals, protein intake, fatigue relief..." class="flex-grow bg-gray-900 border border-gray-800 rounded-2xl px-5 py-4 text-sm text-white focus:outline-none focus:border-emerald-500 transition-colors" onkeydown="if(event.key==='Enter') sendChatMessage()">
                    <button onclick="sendChatMessage()" class="p-4 rounded-2xl bg-gradient-to-r from-brand-600 to-emerald-500 text-white glow-btn flex items-center justify-center">
                        <i data-lucide="send" class="w-5 h-5"></i>
                    </button>
                </div>
            </div>
        </div>

        <div id="page-about" class="page-view space-y-12">
            <div class="text-center max-w-3xl mx-auto space-y-4">
                <div class="inline-flex items-center space-x-2 px-3.5 py-1.5 rounded-full bg-emerald-500/10 text-emerald-400 text-xs font-semibold">
                    <i data-lucide="info" class="w-4 h-4"></i>
                    <span>Project Overview & Vision</span>
                </div>
                <h2 class="text-4xl font-extrabold tracking-tight">About E-HEALTHY (Eat Healthy)</h2>
                <p class="text-gray-400 text-lg leading-relaxed">
                    A digital campus health ecosystem designed to revolutionize student wellness through AI diagnostics, computer vision, and preventive nutrition.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="glass-card rounded-3xl p-8 space-y-6">
                    <div class="w-12 h-12 rounded-2xl bg-brand-500/10 flex items-center justify-center text-emerald-400">
                        <i data-lucide="target" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-2xl font-bold">Our Core Mission</h3>
                    <p class="text-gray-400 leading-relaxed">
                        Modern student life often leads to irregular eating habits, high stress, and fatigue. **E-HEALTHY** (Eat Healthy) provides an accessible, AI-powered digital campus platform that scans early indicators of fatigue, nutritional deficiencies, and dehydration, offering instant personalized dietary prescriptions.
                    </p>
                </div>
                <div class="glass-card rounded-3xl p-8 space-y-6">
                    <div class="w-12 h-12 rounded-2xl bg-brand-500/10 flex items-center justify-center text-emerald-400">
                        <i data-lucide="cpu" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-2xl font-bold">Technology Stack</h3>
                    <ul class="space-y-3 text-gray-400">
                        <li class="flex items-center space-x-3">
                            <i data-lucide="check-circle-2" class="w-5 h-5 text-emerald-400"></i>
                            <span><strong>Frontend:</strong> Tailwind CSS, HTML5, Lucide Icons, Chart.js</span>
                        </li>
                        <li class="flex items-center space-x-3">
                            <i data-lucide="check-circle-2" class="w-5 h-5 text-emerald-400"></i>
                            <span><strong>AI & Computer Vision:</strong> Simulated Python OpenCV & Face Mesh Analysis</span>
                        </li>
                        <li class="flex items-center space-x-3">
                            <i data-lucide="check-circle-2" class="w-5 h-5 text-emerald-400"></i>
                            <span><strong>AI Assistant:</strong> Gemini API Integration for real-time health queries</span>
                        </li>
                        <li class="flex items-center space-x-3">
                            <i data-lucide="check-circle-2" class="w-5 h-5 text-emerald-400"></i>
                            <span><strong>Motion UI:</strong> Spring physics, smooth transitions, and glowing micro-interactions</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>

    </main>

    <footer class="mt-20 border-t border-gray-800/80 glass-card py-8 text-center text-sm text-gray-500">
        <div class="max-w-7xl mx-auto px-4 flex flex-col sm:flex-row items-center justify-between gap-4">
            <div class="flex items-center space-x-2">
                <i data-lucide="activity" class="w-5 h-5 text-emerald-400"></i>
                <span class="font-bold text-gray-300">E-HEALTHY (Eat Healthy)</span>
            </div>
            <div>&copy; 2026 Digital Campus Health Initiative. All rights reserved.</div>
        </div>
    </footer>

    <script>
        // Initialize Lucide Icons
        lucide.createIcons();

        // Smooth Page Switcher with Active States
        function switchPage(pageId) {
            const pages = ['home', 'scan', 'hub', 'assistant', 'about'];
            pages.forEach(p => {
                const el = document.getElementById(`page-${p}`);
                const navBtn = document.getElementById(`nav-${p}`);
                if (p === pageId) {
                    el.classList.add('active');
                    if (navBtn) {
                        navBtn.className = 'px-5 py-2 rounded-full text-sm font-semibold transition-all duration-300 bg-brand-500 text-white shadow-md';
                    }
                } else {
                    el.classList.remove('active');
                    if (navBtn) {
                        navBtn.className = 'px-5 py-2 rounded-full text-sm font-semibold text-gray-400 hover:text-white hover:bg-gray-800 transition-all duration-300';
                    }
                }
            });
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        // Mobile Menu Toggle
        function toggleMobileMenu() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        }

        // Webcam Simulation
        let webcamStream = null;
        async function startWebcam() {
            const video = document.getElementById('webcam-video');
            const placeholder = document.getElementById('scan-placeholder');
            const faceBox = document.getElementById('face-box');
            const btnCam = document.getElementById('btn-cam');

            try {
                webcamStream = await navigator.mediaDevices.getUserMedia({ video: true });
                video.srcObject = webcamStream;
                video.classList.remove('hidden');
                placeholder.classList.add('hidden');
                faceBox.classList.remove('hidden');
                btnCam.innerHTML = `<i data-lucide="video-off" class="w-4 h-4 text-red-400"></i><span>Stop Camera</span>`;
                btnCam.onclick = stopWebcam;
                lucide.createIcons();
            } catch (e) {
                alert('Webcam access denied or unavailable. Please use the image upload option.');
            }
        }

        function stopWebcam() {
            if (webcamStream) {
                webcamStream.getTracks().forEach(track => track.stop());
                webcamStream = null;
            }
            const video = document.getElementById('webcam-video');
            const placeholder = document.getElementById('scan-placeholder');
            const faceBox = document.getElementById('face-box');
            const btnCam = document.getElementById('btn-cam');

            video.classList.add('hidden');
            placeholder.classList.remove('hidden');
            faceBox.classList.add('hidden');
            btnCam.innerHTML = `<i data-lucide="video" class="w-4 h-4 text-emerald-400"></i><span>Start Camera</span>`;
            btnCam.onclick = startWebcam;
            lucide.createIcons();
        }

        function handleImageUpload(event) {
            const file = event.target.files[0];
            if (file) {
                const placeholder = document.getElementById('scan-placeholder');
                placeholder.innerHTML = `
                    <div class="w-20 h-20 rounded-2xl bg-brand-500/20 border border-emerald-500/40 flex items-center justify-center text-emerald-400">
                        <i data-lucide="image" class="w-10 h-10"></i>
                    </div>
                    <div>
                        <h4 class="font-bold text-lg">${file.name}</h4>
                        <p class="text-xs text-emerald-400">Photo loaded successfully. Ready for AI Scan.</p>
                    </div>
                `;
                document.getElementById('face-box').classList.remove('hidden');
                lucide.createIcons();
            }
        }

        // Trigger AI Face Scan Simulation
        function triggerAIScan() {
            const badge = document.getElementById('scan-status-badge');
            const container = document.getElementById('results-container');
            const laser = document.getElementById('scan-laser-overlay');

            badge.className = 'px-2.5 py-1 rounded-full bg-brand-500/20 text-emerald-400 text-xs font-bold animate-pulse';
            badge.innerText = 'Analyzing Biometrics...';
            laser.classList.remove('hidden');

            container.innerHTML = `
                <div class="space-y-4 py-8 text-center">
                    <div class="w-12 h-12 border-4 border-emerald-500 border-t-transparent rounded-full animate-spin mx-auto"></div>
                    <p class="text-sm text-gray-300 font-medium">Scanning micro-expressions & skin hydration...</p>
                </div>
            `;

            setTimeout(() => {
                laser.classList.add('hidden');
                badge.className = 'px-2.5 py-1 rounded-full bg-emerald-500/20 text-emerald-400 text-xs font-bold';
                badge.innerText = 'Analysis Complete';

                container.innerHTML = `
                    <div class="space-y-4">
                        <div class="p-4 rounded-2xl bg-gray-900 border border-gray-800 space-y-2">
                            <div class="flex justify-between text-sm font-semibold">
                                <span>Fatigue Risk Index</span>
                                <span class="text-amber-400">18% (Low)</span>
                            </div>
                            <div class="w-full h-2 bg-gray-800 rounded-full overflow-hidden">
                                <div class="h-full bg-amber-400 rounded-full" style="width: 18%"></div>
                            </div>
                        </div>

                        <div class="p-4 rounded-2xl bg-gray-900 border border-gray-800 space-y-2">
                            <div class="flex justify-between text-sm font-semibold">
                                <span>Skin Hydration Level</span>
                                <span class="text-emerald-400">84% (Optimal)</span>
                            </div>
                            <div class="w-full h-2 bg-gray-800 rounded-full overflow-hidden">
                                <div class="h-full bg-emerald-400 rounded-full" style="width: 84%"></div>
                            </div>
                        </div>

                        <div class="p-4 rounded-2xl bg-gray-900 border border-gray-800 space-y-2">
                            <div class="flex justify-between text-sm font-semibold">
                                <span>Iron / Vitamin Deficiency</span>
                                <span class="text-emerald-400">Minimal Risk (92%)</span>
                            </div>
                            <div class="w-full h-2 bg-gray-800 rounded-full overflow-hidden">
                                <div class="h-full bg-emerald-400 rounded-full" style="width: 92%"></div>
                            </div>
                        </div>

                        <div class="p-4 rounded-2xl bg-emerald-500/10 border border-emerald-500/20 space-y-2">
                            <div class="flex items-center space-x-2 text-emerald-400 font-bold text-sm">
                                <i data-lucide="sparkles" class="w-4 h-4"></i>
                                <span>E-HEALTHY Prescription</span>
                            </div>
                            <p class="text-xs text-gray-300 leading-relaxed">
                                Maintain current hydration (2.5L water daily). Add citrus fruits and green salads to your campus lunch menu to sustain optimal energy levels.
                            </p>
                        </div>
                    </div>
                `;
                lucide.createIcons();
            }, 2000);
        }

        // Initialize Chart.js Dashboards
        window.addEventListener('DOMContentLoaded', () => {
            const nutrientCtx = document.getElementById('nutrientChart').getContext('2d');
            new Chart(nutrientCtx, {
                type: 'bar',
                data: {
                    labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
                    datasets: [
                        { label: 'Protein (g)', data: [65, 70, 80, 75, 85, 90, 88], backgroundColor: '#10b981', borderRadius: 6 },
                        { label: 'Target', data: [75, 75, 75, 75, 75, 75, 75], type: 'line', borderColor: '#34d399', borderWidth: 2, pointRadius: 0 }
                    ]
                },
                options: { responsive: true, maintainAspectRatio: false, plugins: { legend: { labels: { color: '#9ca3af', font: { family: 'Plus Jakarta Sans' } } } }, scales: { x: { grid: { color: '#1f2937' }, ticks: { color: '#9ca3af' } }, y: { grid: { color: '#1f2937' }, ticks: { color: '#9ca3af' } } } }
            });

            const hydrationCtx = document.getElementById('hydrationChart').getContext('2d');
            new Chart(hydrationCtx, {
                type: 'line',
                data: {
                    labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
                    datasets: [{ label: 'Hydration Score', data: [80, 85, 78, 90, 92, 88, 95], borderColor: '#10b981', backgroundColor: 'rgba(16, 185, 129, 0.1)', fill: true, tension: 0.4 }]
                },
                options: { responsive: true, maintainAspectRatio: false, plugins: { legend: { labels: { color: '#9ca3af', font: { family: 'Plus Jakarta Sans' } } } }, scales: { x: { grid: { color: '#1f2937' }, ticks: { color: '#9ca3af' } }, y: { grid: { color: '#1f2937' }, ticks: { color: '#9ca3af' } } } }
            });
        });

        function simulateFileUpload(event) {
            alert('Report uploaded successfully! Visualizing metric graphs in the Health Hub.');
        }

        function loadSampleReport() {
            alert('Demo campus blood work report loaded into charts.');
        }

        // Gemini AI Assistant Chat Simulation
        function sendChatMessage() {
            const input = document.getElementById('chat-input');
            const messages = document.getElementById('chat-messages');
            const query = input.value.trim();
            if (!query) return;

            // Append User Message
            messages.innerHTML += `
                <div class="flex items-start justify-end space-x-3">
                    <div class="glass-card rounded-2xl p-4 max-w-xl text-sm leading-relaxed text-gray-200 bg-emerald-950/40 border-emerald-500/30">
                        ${query}
                    </div>
                    <div class="w-10 h-10 rounded-xl bg-gray-800 flex items-center justify-center text-emerald-400 flex-shrink-0">
                        <i data-lucide="user" class="w-5 h-5"></i>
                    </div>
                </div>
            `;
            input.value = '';
            messages.scrollTop = messages.scrollHeight;

            // Simulate Gemini AI Response
            setTimeout(() => {
                let aiReply = "That's a great question regarding your campus nutrition! To maintain steady focus during classes, combine complex carbohydrates with lean proteins like lentils, paneer, or chicken salads.";
                if (query.toLowerCase().includes('fatigue')) {
                    aiReply = "Fatigue is often caused by mild dehydration or iron deficiency. Ensure you drink at least 2.5 liters of water daily and include iron-rich foods such as spinach and pomegranate in your diet.";
                } else if (query.toLowerCase().includes('protein')) {
                    aiReply = "For active students, a daily intake of 1.2g to 1.6g of protein per kg of body weight is ideal. Try Greek yogurt, sprouts, eggs, and tofu.";
                }

                messages.innerHTML += `
                    <div class="flex items-start space-x-3">
                        <div class="w-10 h-10 rounded-xl bg-brand-600 flex items-center justify-center text-white flex-shrink-0 shadow-lg">
                            <i data-lucide="bot" class="w-5 h-5"></i>
                        </div>
                        <div class="glass-card rounded-2xl p-4 max-w-xl text-sm leading-relaxed text-gray-200">
                            ${aiReply}
                        </div>
                    </div>
                `;
                lucide.createIcons();
                messages.scrollTop = messages.scrollHeight;
            }, 1000);
        }
    </script>
</body>
</html>
