<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AL_HOSTING</title>
    <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>👨‍💻</text></svg>">
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        electric: '#00f0ff',
                        neonPurple: '#a855f7',
                        dark: '#0f172a',
                        darker: '#020617'
                    },
                    fontFamily: {
                        orbitron: ['Orbitron', 'sans-serif'],
                        poppins: ['Poppins', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <script src="https://unpkg.com/feather-icons"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.11.4/gsap.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.11.4/ScrollTrigger.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r134/three.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/vanta@latest/dist/vanta.net.min.js"></script>
    
    <style>
        .glass-card {
            background: rgba(15, 23, 42, 0.7);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .neon-text {
            text-shadow: 0 0 10px #00f0ff, 0 0 20px #00f0ff;
        }
        
        .neon-border {
            box-shadow: 0 0 10px #00f0ff, 0 0 20px #00f0ff;
        }
        
        .skill-bar {
            height: 8px;
            background: linear-gradient(90deg, #00f0ff 0%, #a855f7 100%);
            border-radius: 4px;
        }
        
        .typing-text {
            border-right: 3px solid #00f0ff;
            white-space: nowrap;
            overflow: hidden;
            animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
        }
        
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #00f0ff }
        }
        
        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0, 240, 255, 0.3);
        }
    </style>
</head>
<body class="bg-darker text-white font-poppins relative overflow-x-hidden"></body>
    <div id="vanta-bg" class="fixed top-0 left-0 w-full h-full z-0"></div>
    <div class="relative z-10">
        <header class="container mx-auto px-6 py-8">
            <div class="flex justify-between items-center">
                <div class="text-2xl font-bold font-orbitron text-electric neon-text">
                    AL_HOSTING
                </div>
<nav class="hidden md:block">
                    <ul class="flex space-x-8">
                        <li><a href="#home" class="hover:text-electric transition">Home</a></li>
                        <li><a href="#projects" class="hover:text-electric transition">Projects</a></li>
                        <li><a href="#skills" class="hover:text-electric transition">Skills</a></li>
                        <li><a href="#contact" class="hover:text-electric transition">Contact</a></li>
                    </ul>
                </nav>
                <button class="md:hidden">
                    <i data-feather="menu" class="text-electric"></i>
                </button>
            </div>
        </header>
        <section id="home" class="container mx-auto px-6 py-20 md:py-32 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-12 md:mb-0">
                <h1 class="text-4xl md:text-6xl font-bold font-orbitron text-white mb-4">
                    Halo, Saya <span class="text-electric neon-text">AL_HOSTING</span>
                </h1>
                <h2 class="text-2xl md:text-4xl font-orbitron text-white mb-6 typing-text">
                    Full Stack Developer
                </h2>
                <p class="text-lg mb-8 max-w-lg">
                    Saya membangun sebuah bisnis yaitu di bidang hosting dan developer nexa id
                </p>
<div class="flex space-x-4">
                    <a href="#projects" class="px-8 py-3 bg-gradient-to-r from-electric to-neonPurple rounded-full font-bold text-dark hover:scale-105 transition transform">
                        Lihat Projek
                    </a>
                    <a href="https://github.com/SIsuryaOfficial" target="_blank" class="px-8 py-3 border-2 border-electric rounded-full font-bold text-electric hover:bg-electric hover:text-dark transition">
                        GitHub Saya
                    </a>
</div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <div class="relative">
                    <div class="w-64 h-64 md:w-80 md:h-80 rounded-full bg-gradient-to-br from-electric to-neonPurple opacity-20 absolute -z-10 top-0 left-0"></div>
                    <img src="http://static.photos/technology/640x360/42" alt="Developer" class="w-64 h-64 md:w-80 md:h-80 rounded-full object-cover border-4 border-electric neon-border">
                </div>
            </div>
        </section>
        <section id="projects" class="container mx-auto px-6 py-20">
            <h2 class="text-3xl md:text-5xl font-bold font-orbitron text-white mb-12 text-center">
                My <span class="text-electric neon-text">Projects</span>
            </h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="glass-card rounded-xl p-6 project-card transition duration-500">
                    <div class="h-48 bg-gradient-to-br from-electric/20 to-neonPurple/20 rounded-lg mb-4 overflow-hidden">
                        <img src="http://static.photos/technology/640x360/1" alt="Project 1" class="w-full h-full object-cover">
                    </div>
                    <h3 class="text-xl font-bold font-orbitron text-white mb-2">Quantum Dashboard</h3>
                    <p class="text-gray-400 mb-4">A futuristic admin dashboard with real-time analytics and AI predictions.</p>
                    <div class="flex flex-wrap gap-2 mb-4">
                        <span class="px-3 py-1 bg-dark text-electric text-xs rounded-full">React</span>
                        <span class="px-3 py-1 bg-dark text-electric text-xs rounded-full">Node.js</span>
                        <span class="px-3 py-1 bg-dark text-electric text-xs rounded-full">Three.js</span>
                    </div>
                    <a href="#" class="text-electric hover:underline inline-flex items-center">
                        View Project <i data-feather="arrow-right" class="ml-2 w-4 h-4"></i>
                    </a>
                </div>
                <div class="glass-card rounded-xl p-6 project-card transition duration-500">
                    <div class="h-48 bg-gradient-to-br from-electric/20 to-neonPurple/20 rounded-lg mb-4 overflow-hidden">
                        <img src="http://static.photos/technology/640x360/2" alt="Project 2" class="w-full h-full object-cover">
                    </div>
                    <h3 class="text-xl font-bold font-orbitron text-white mb-2">Neon Social</h3>
                    <p class="text-gray-400 mb-4">A next-gen social media platform with Web3 integration and NFT support.</p>
                    <div class="flex flex-wrap gap-2 mb-4">
                        <span class="px-3 py-1 bg-dark text-electric text-xs rounded-full">Next.js</span>
                        <span class="px-3 py-1 bg-dark text-electric text-xs rounded-full">Solidity</span>
                        <span class="px-3 py-1 bg-dark text-electric text-xs rounded-full">GraphQL</span>
                    </div>
                    <a href="#" class="text-electric hover:underline inline-flex items-center">
                        View Project <i data-feather="arrow-right" class="ml-2 w-4 h-4"></i>
                    </a>
                </div>
                <div class="glass-card rounded-xl p-6 project-card transition duration-500">
                    <div class="h-48 bg-gradient-to-br from-electric/20 to-neonPurple/20 rounded-lg mb-4 overflow-hidden">
                        <img src="http://static.photos/technology/640x360/3" alt="Project 3" class="w-full h-full object-cover">
                    </div>
                    <h3 class="text-xl font-bold font-orbitron text-white mb-2">AR Shopping</h3>
                    <p class="text-gray-400 mb-4">Augmented reality e-commerce app for virtual product try-ons.</p>
                    <div class="flex flex-wrap gap-2 mb-4">
                        <span class="px-3 py-1 bg-dark text-electric text-xs rounded-full">AR.js</span>
                        <span class="px-3 py-1 bg-dark text-electric text-xs rounded-full">Vue.js</span>
                        <span class="px-3 py-1 bg-dark text-electric text-xs rounded-full">Firebase</span>
                    </div>
                    <a href="#" class="text-electric hover:underline inline-flex items-center">
                        View Project <i data-feather="arrow-right" class="ml-2 w-4 h-4"></i>
                    </a>
                </div>
            </div>
            
            <div class="text-center mt-12">
                    <a href="https://github.com/SIsuryaOfficial?tab=repositories" target="_blank" class="px-8 py-3 border-2 border-electric rounded-full font-bold text-electric hover:bg-electric hover:text-dark transition">
                        Lihat Semua Projek
                    </a>
</div>
        </section>

        <section id="skills" class="container mx-auto px-6 py-20">
            <h2 class="text-3xl md:text-5xl font-bold font-orbitron text-white mb-12 text-center">
                My <span class="text-electric neon-text">Skills</span>
            </h2>
            
            <div class="max-w-4xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-8">
                <div>
                    <div class="mb-8">
                        <div class="flex justify-between mb-2">
                            <span class="font-medium">JavaScript</span>
                            <span>95%</span>
                        </div>
                        <div class="w-full bg-gray-800 rounded-full h-2">
                            <div class="skill-bar rounded-full h-2" style="width: 95%"></div>
                        </div>
                    </div>
                    
                    <div class="mb-8">
                        <div class="flex justify-between mb-2">
                            <span class="font-medium">React</span>
                            <span>90%</span>
                        </div>
                        <div class="w-full bg-gray-800 rounded-full h-2">
                            <div class="skill-bar rounded-full h-2" style="width: 90%"></div>
                        </div>
                    </div>
                    
                    <div class="mb-8">
                        <div class="flex justify-between mb-2">
                            <span class="font-medium">Node.js</span>
                            <span>85%</span>
                        </div>
                        <div class="w-full bg-gray-800 rounded-full h-2">
                            <div class="skill-bar rounded-full h-2" style="width: 85%"></div>
                        </div>
                    </div>
                </div>
                
                <div>
                    <div class="mb-8">
                        <div class="flex justify-between mb-2">
                            <span class="font-medium">TypeScript</span>
                            <span>80%</span>
                        </div>
                        <div class="w-full bg-gray-800 rounded-full h-2">
                            <div class="skill-bar rounded-full h-2" style="width: 80%"></div>
                        </div>
                    </div>
                    
                    <div class="mb-8">
                        <div class="flex justify-between mb-2">
                            <span class="font-medium">GraphQL</span>
                            <span>75%</span>
                        </div>
                        <div class="w-full bg-gray-800 rounded-full h-2">
                            <div class="skill-bar rounded-full h-2" style="width: 75%"></div>
                        </div>
                    </div>
                    
                    <div class="mb-8">
                        <div class="flex justify-between mb-2">
                            <span class="font-medium">Three.js</span>
                            <span>70%</span>
                        </div>
                        <div class="w-full bg-gray-800 rounded-full h-2">
                            <div class="skill-bar rounded-full h-2" style="width: 70%"></div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="max-w-4xl mx-auto mt-12">
                <h3 class="text-xl font-bold font-orbitron text-white mb-6 text-center">
                    Other Technologies
                </h3>
                <div class="flex flex-wrap justify-center gap-4">
                    <div class="px-6 py-3 bg-dark rounded-full flex items-center">
                        <i data-feather="code" class="text-electric mr-2"></i>
                        <span>HTML/CSS</span>
                    </div>
                    <div class="px-6 py-3 bg-dark rounded-full flex items-center">
                        <i data-feather="database" class="text-electric mr-2"></i>
                        <span>MongoDB</span>
                    </div>
                    <div class="px-6 py-3 bg-dark rounded-full flex items-center">
                        <i data-feather="git-branch" class="text-electric mr-2"></i>
                        <span>Git</span>
                    </div>
                    <div class="px-6 py-3 bg-dark rounded-full flex items-center">
                        <i data-feather="cpu" class="text-electric mr-2"></i>
                        <span>Docker</span>
                    </div>
                    <div class="px-6 py-3 bg-dark rounded-full flex items-center">
                        <i data-feather="cloud" class="text-electric mr-2"></i>
                        <span>AWS</span>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact" class="container mx-auto px-6 py-20">
            <div class="max-w-4xl mx-auto glass-card rounded-xl p-8 md:p-12">
                <h2 class="text-3xl md:text-5xl font-bold font-orbitron text-white mb-6 text-center">
                    Get In <span class="text-electric neon-text">Touch</span>
                </h2>
                <p class="text-center mb-12 max-w-2xl mx-auto">
                    Have a project in mind or want to discuss potential opportunities? Feel free to reach out!
                </p>
                
                <form class="space-y-6">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        <div>
                            <label for="name" class="block mb-2">Your Name</label>
                            <input type="text" id="name" class="w-full px-4 py-3 bg-dark border border-gray-700 rounded-lg focus:outline-none focus:border-electric">
                        </div>
                        <div>
                            <label for="email" class="block mb-2">Your Email</label>
                            <input type="email" id="email" class="w-full px-4 py-3 bg-dark border border-gray-700 rounded-lg focus:outline-none focus:border-electric">
                        </div>
                    </div>
                    <div>
                        <label for="subject" class="block mb-2">Subject</label>
                        <input type="text" id="subject" class="w-full px-4 py-3 bg-dark border border-gray-700 rounded-lg focus:outline-none focus:border-electric">
                    </div>
                    <div>
                        <label for="message" class="block mb-2">Message</label>
                        <textarea id="message" rows="5" class="w-full px-4 py-3 bg-dark border border-gray-700 rounded-lg focus:outline-none focus:border-electric"></textarea>
                    </div>
                    <button type="submit" class="w-full px-8 py-4 bg-gradient-to-r from-electric to-neonPurple rounded-full font-bold text-dark hover:scale-105 transition transform">
                        Send Message
                    </button>
                </form>
            </div>
        </section>

        <footer class="container mx-auto px-6 py-12">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="text-xl font-bold font-orbitron text-electric neon-text mb-4 md:mb-0">
                   
                </div>
                <div class="flex space-x-6 mb-4 md:mb-0">
                    <a href="https://github.com/SIsuryaOfficial" target="_blank" class="text-gray-400 hover:text-electric transition">
                        <i data-feather="github"></i>
                    </a>
                    <a href="https://twitter.com/SIsuryaOfficial" target="_blank" class="text-gray-400 hover:text-electric transition">
                        <i data-feather="twitter"></i>
                    </a>
                    <a href="https://linkedin.com/in/SIsuryaOfficial" target="_blank" class="text-gray-400 hover:text-electric transition">
                        <i data-feather="linkedin"></i>
                    </a>
                    <a href="https://instagram.com/SIsuryaOfficial" target="_blank" class="text-gray-400 hover:text-electric transition">
                        <i data-feather="instagram"></i>
                    </a>
</div>
            </div>
        </footer>
    </div>

    <script>
        VANTA.NET({
            el: "#vanta-bg",
            mouseControls: true,
            touchControls: true,
            gyroControls: false,
            minHeight: 200.00,
            minWidth: 200.00,
            scale: 1.00,
            scaleMobile: 1.00,
            color: 0x00f0ff,
            backgroundColor: 0x020617,
            points: 12.00,
            maxDistance: 22.00,
            spacing: 18.00
        });
        
        document.addEventListener('DOMContentLoaded', () => {
            gsap.registerPlugin(ScrollTrigger);
            gsap.utils.toArray('section').forEach(section => {
                gsap.from(section, {
                    scrollTrigger: {
                        trigger: section,
                        start: "top 80%",
                        toggleActions: "play none none none"
                    },
                    opacity: 0,
                    y: 50,
                    duration: 1
                });
            });
            gsap.utils.toArray('.project-card').forEach(card => {
                card.addEventListener('mouseenter', () => {
                    gsap.to(card, {
                        scale: 1.05,
                        duration: 0.3
                    });
                });
                card.addEventListener('mouseleave', () => {
                    gsap.to(card, {
                        scale: 1,
                        duration: 0.3
                    });
                });
            });

            gsap.utils.toArray('button').forEach(button => {
                button.addEventListener('mouseenter', () => {
                    gsap.to(button, {
                        scale: 1.05,
                        duration: 0.2
                    });
                });
                button.addEventListener('mouseleave', () => {
                    gsap.to(button, {
                        scale: 1,
                        duration: 0.2
                    });
                });
            });
        });
        feather.replace();
    </script>
</body>
</html>
