# Eu-Sou-Você-
meu tcc
!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eu Sou Você</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');
        body { font-family: 'Inter', sans-serif; }
        
        .gradient-bg { 
            background: linear-gradient(135deg, #e385c8 0%, #5632f3 100%);
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }
        
        .fade-in {
            animation: fadeIn 0.6s ease-out;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .pulse-gentle {
            animation: pulseGentle 3s ease-in-out infinite;
        }
        
        @keyframes pulseGentle {
            0%, 100% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.05); opacity: 0.8; }
        }
        
        .breathing-circle {
            transition: all 1s ease-in-out;
        }
        
        .glassmorphism {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .progress-bar {
            transition: width 0.3s ease;
        }
        
        .mood-emoji {
            font-size: 2.5rem;
            transition: all 0.2s ease;
        }
        
        .mood-emoji:hover {
            transform: scale(1.2);
        }
        
        .feature-icon {
            transition: all 0.3s ease;
        }
        
        .feature-icon:hover {
            transform: rotate(5deg) scale(1.1);
        }
    </style>
</head>
<body class="bg-gradient-to-br from-blue-50 to-purple-50 min-h-screen">
    <!-- navegação -->
    <nav class="bg-white/50 backdrop-blur-md shadow-lg sticky top-0 z-50">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <div class="flex-shrink-0 flex items-center">
                        <div class= rounded-xl flex items-center justify-center mr-3 pulse-gentle>
                            <div class="w-10 h-10 flex items-center justify-center mr-3 pulse-gentle" aria-label="Logo MindWell">
                                <!-- Borboleta lavanda realista, adaptada ao tamanho da logo -->
                                <svg width="36" height="30" viewBox="0 0 140 120" fill="none" xmlns="http://www.w3.org/2000/svg">
                                  <!-- Cabeça -->
                                  <ellipse cx="70" cy="35" rx="3" ry="4" fill="url(#headGradient)"/>
                                  <circle cx="68" cy="33" r="0.8" fill="#1F2937" opacity="0.8"/>
                                  <circle cx="72" cy="33" r="0.8" fill="#1F2937" opacity="0.8"/>
                  
                                  <!-- Tórax -->
                                  <ellipse cx="70" cy="45" rx="2.5" ry="8" fill="url(#thoraxGradient)"/>
                  
                                  <!-- Abdômen -->
                                  <ellipse cx="70" cy="65" rx="2" ry="18" fill="url(#abdomenGradient)"/>
                  
                                  <!-- Antenas -->
                                  <path d="M67,32 Q62,25 58,18" stroke="#374151" stroke-width="1.5" fill="none" stroke-linecap="round"/>
                                  <path d="M73,32 Q78,25 82,18" stroke="#374151" stroke-width="1.5" fill="none" stroke-linecap="round"/>
                                  <ellipse cx="58" cy="18" rx="1.5" ry="2" fill="#8B5CF6"/>
                                  <ellipse cx="82" cy="18" rx="1.5" ry="2" fill="#8B5CF6"/>
                  
                                  <!-- Asa superior esquerda -->
                                  <path d="M67,42 Q35,15 15,25 Q8,35 12,55 Q18,75 45,70 Q60,65 67,50 Z" fill="url(#leftUpperWing)" stroke="#7C3AED" stroke-width="0.8" opacity="0.95"/>
                                  <!-- Asa inferior esquerda -->
                                  <path d="M67,52 Q45,48 35,65 Q32,75 38,85 Q45,90 55,85 Q65,78 67,65 Z" fill="url(#leftLowerWing)" stroke="#7C3AED" stroke-width="0.8" opacity="0.95"/>
                  
                                  <!-- Asa superior direita -->
                                  <path d="M73,42 Q105,15 125,25 Q132,35 128,55 Q122,75 95,70 Q80,65 73,50 Z" fill="url(#rightUpperWing)" stroke="#7C3AED" stroke-width="0.8" opacity="0.95"/>
                                  <!-- Asa inferior direita -->
                                  <path d="M73,52 Q95,48 105,65 Q108,75 102,85 Q95,90 85,85 Q75,78 73,65 Z" fill="url(#rightLowerWing)" stroke="#7C3AED" stroke-width="0.8" opacity="0.95"/>
                  
                                  <!-- Nervuras -->
                                  <path d="M67,42 L45,35 M67,42 L40,50 M67,42 L35,65" stroke="#8B5CF6" stroke-width="0.5" opacity="0.6"/>
                                  <path d="M73,42 L95,35 M73,42 L100,50 M73,42 L105,65" stroke="#8B5CF6" stroke-width="0.5" opacity="0.6"/>
                                  <path d="M67,52 L50,60 M67,52 L45,75" stroke="#8B5CF6" stroke-width="0.5" opacity="0.6"/>
                                  <path d="M73,52 L90,60 M73,52 L95,75" stroke="#8B5CF6" stroke-width="0.5" opacity="0.6"/>
                  
                                  <!-- Ocelos maiores -->
                                  <circle cx="35" cy="45" r="6" fill="url(#eyespot1)" opacity="0.8"/>
                                  <circle cx="35" cy="45" r="3" fill="#1F2937" opacity="0.6"/>
                                  <circle cx="35" cy="45" r="1.5" fill="#FFFFFF" opacity="0.9"/>
                                  <circle cx="105" cy="45" r="6" fill="url(#eyespot2)" opacity="0.8"/>
                                  <circle cx="105" cy="45" r="3" fill="#1F2937" opacity="0.6"/>
                                  <circle cx="105" cy="45" r="1.5" fill="#FFFFFF" opacity="0.9"/>
                  
                                  <!-- Ocelos menores -->
                                  <circle cx="45" cy="70" r="4" fill="url(#smallEyespot1)" opacity="0.7"/>
                                  <circle cx="45" cy="70" r="2" fill="#374151" opacity="0.5"/>
                                  <circle cx="45" cy="70" r="1" fill="#FFFFFF" opacity="0.8"/>
                                  <circle cx="95" cy="70" r="4" fill="url(#smallEyespot2)" opacity="0.7"/>
                                  <circle cx="95" cy="70" r="2" fill="#374151" opacity="0.5"/>
                                  <circle cx="95" cy="70" r="1" fill="#FFFFFF" opacity="0.8"/>
                  
                                  <!-- Pontos de brilho -->
                                  <circle cx="25" cy="35" r="2" fill="#DDD6FE" opacity="0.7"/>
                                  <circle cx="30" cy="60" r="1.5" fill="#C4B5FD" opacity="0.8"/>
                                  <circle cx="115" cy="35" r="2" fill="#DDD6FE" opacity="0.7"/>
                                  <circle cx="110" cy="60" r="1.5" fill="#C4B5FD" opacity="0.8"/>
                  
                                  <!-- Gradientes -->
                                  <defs>
                                    <linearGradient id="headGradient" x1="0%" y1="0%" x2="0%" y2="100%">
                                      <stop offset="0%" stop-color="#4B5563"/><stop offset="100%" stop-color="#374151"/>
                                    </linearGradient>
                                    <linearGradient id="thoraxGradient" x1="0%" y1="0%" x2="0%" y2="100%">
                                      <stop offset="0%" stop-color="#6B7280"/><stop offset="50%" stop-color="#4B5563"/><stop offset="100%" stop-color="#374151"/>
                                    </linearGradient>
                                    <linearGradient id="abdomenGradient" x1="0%" y1="0%" x2="0%" y2="100%">
                                      <stop offset="0%" stop-color="#6B7280"/><stop offset="100%" stop-color="#4B5563"/>
                                    </linearGradient>
                                    <radialGradient id="leftUpperWing" cx="0.4" cy="0.3" r="0.8">
                                      <stop offset="0%" stop-color="#FFFFFF" stop-opacity="0.95"/>
                                      <stop offset="20%" stop-color="#FAF5FF" stop-opacity="0.9"/>
                                      <stop offset="40%" stop-color="#F3E8FF" stop-opacity="0.85"/>
                                      <stop offset="60%" stop-color="#E9D5FF" stop-opacity="0.8"/>
                                      <stop offset="80%" stop-color="#C4B5FD" stop-opacity="0.75"/>
                                      <stop offset="100%" stop-color="#8B5CF6" stop-opacity="0.8"/>
                                    </radialGradient>
                                    <radialGradient id="leftLowerWing" cx="0.4" cy="0.3" r="0.8">
                                      <stop offset="0%" stop-color="#F8FAFC" stop-opacity="0.9"/>
                                      <stop offset="30%" stop-color="#F1F5F9" stop-opacity="0.85"/>
                                      <stop offset="60%" stop-color="#DDD6FE" stop-opacity="0.8"/>
                                      <stop offset="100%" stop-color="#A855F7" stop-opacity="0.85"/>
                                    </radialGradient>
                                    <radialGradient id="rightUpperWing" cx="0.6" cy="0.3" r="0.8">
                                      <stop offset="0%" stop-color="#FFFFFF" stop-opacity="0.95"/>
                                      <stop offset="20%" stop-color="#FAF5FF" stop-opacity="0.9"/>
                                      <stop offset="40%" stop-color="#F3E8FF" stop-opacity="0.85"/>
                                      <stop offset="60%" stop-color="#E9D5FF" stop-opacity="0.8"/>
                                      <stop offset="80%" stop-color="#C4B5FD" stop-opacity="0.75"/>
                                      <stop offset="100%" stop-color="#8B5CF6" stop-opacity="0.8"/>
                                    </radialGradient>
                                    <radialGradient id="rightLowerWing" cx="0.6" cy="0.3" r="0.8">
                                      <stop offset="0%" stop-color="#F8FAFC" stop-opacity="0.9"/>
                                      <stop offset="30%" stop-color="#F1F5F9" stop-opacity="0.85"/>
                                      <stop offset="60%" stop-color="#DDD6FE" stop-opacity="0.8"/>
                                      <stop offset="100%" stop-color="#A855F7" stop-opacity="0.85"/>
                                    </radialGradient>
                                    <radialGradient id="eyespot1" cx="0.5" cy="0.5" r="0.8">
                                      <stop offset="0%" stop-color="#7C3AED" stop-opacity="0.9"/>
                                      <stop offset="50%" stop-color="#A855F7" stop-opacity="0.7"/>
                                      <stop offset="100%" stop-color="#C4B5FD" stop-opacity="0.5"/>
                                    </radialGradient>
                                    <radialGradient id="eyespot2" cx="0.5" cy="0.5" r="0.8">
                                      <stop offset="0%" stop-color="#7C3AED" stop-opacity="0.9"/>
                                      <stop offset="50%" stop-color="#A855F7" stop-opacity="0.7"/>
                                      <stop offset="100%" stop-color="#C4B5FD" stop-opacity="0.5"/>
                                    </radialGradient>
                                    <radialGradient id="smallEyespot1" cx="0.5" cy="0.5" r="0.8">
                                      <stop offset="0%" stop-color="#8B5CF6" stop-opacity="0.8"/>
                                      <stop offset="70%" stop-color="#C4B5FD" stop-opacity="0.6"/>
                                      <stop offset="100%" stop-color="#DDD6FE" stop-opacity="0.4"/>
                                    </radialGradient>
                                    <radialGradient id="smallEyespot2" cx="0.5" cy="0.5" r="0.8">
                                      <stop offset="0%" stop-color="#8B5CF6" stop-opacity="0.8"/>
                                      <stop offset="70%" stop-color="#C4B5FD" stop-opacity="0.6"/>
                                      <stop offset="100%" stop-color="#DDD6FE" stop-opacity="0.4"/>
                                    </radialGradient>
                                  </defs>
                                </svg>
                              </div>
                              <span class="text-2xl font-bold bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent"></span>
                        </div>
                        <span class="text-3xl font-bold bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">Eu Sou Você</span>
                    </div>
                </div>
                <div class="hidden md:flex items-center space-x-8">
                    <button onclick="showPage('home')" class="nav-btn text-gray-700 hover:text-blue-600 px-3 py-2 font-medium transition-colors">🏠 Início</button>
                    <button onclick="showPage('assessment')" class="nav-btn text-gray-700 hover:text-blue-600 px-3 py-2 font-medium transition-colors">📋 Avaliação</button>
                    <button onclick="showPage('resources')" class="nav-btn text-gray-700 hover:text-blue-600 px-3 py-2 font-medium transition-colors">📚 Recursos</button>
                    <button onclick="showPage('tools')" class="nav-btn text-gray-700 hover:text-blue-600 px-3 py-2 font-medium transition-colors">🛠️ Ferramentas</button>
                    <button onclick="showPage('about')" class="nav-btn text-gray-700 hover:text-blue-600 px-3 py-2 font-medium transition-colors">ℹ️ Sobre</button>
                </div>
                <div class="md:hidden">
                    <button onclick="toggleMobileMenu()" class="text-gray-700 hover:text-blue-600">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
    </nav>

    <!-- página inicial -->
    <div id="home-page" class="page">
        <!-- Seção de herói-->
        <section class="gradient-bg text-white py-20 relative overflow-hidden">
            <div class="absolute inset-0 bg-black/10"></div>
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative">
                <div class="text-center fade-in">
                    <h1 class="text-4xl md:text-6xl font-bold mb-6">Cuidando da Sua Saúde Mental</h1>
                    <p class="text-xl md:text-2xl mb-8 max-w-3xl mx-auto opacity-90">
                        Uma plataforma acolhedora e profissional com ferramentas baseadas em ciência para promover seu bem-estar mental
                    </p>
                    <div class="flex flex-col sm:flex-row gap-4 justify-center">
                        <button onclick="showPage('assessment')" class="bg-white text-blue-600 px-8 py-4 rounded-xl font-semibold hover:bg-gray-100 transition duration-300 shadow-lg">
                            ✨ Fazer Avaliação
                        </button>
                        <button onclick="document.getElementById('features').scrollIntoView({behavior: 'smooth'})" class="border-2 border-white text-white px-8 py-4 rounded-xl font-semibold hover:bg-white hover:text-blue-600 transition duration-300">
                            🔍 Explorar Recursos
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Estatísticas rápidas-->
        <section class="py-12 bg-white/80 backdrop-blur-sm">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="grid md:grid-cols-4 gap-8 text-center">
                    <div class="p-6">
                        <div class="text-4xl mb-2">💙</div>
                        <div class="text-2xl font-bold text-blue-600 mb-1">1 em 4</div>
                        <p class="text-gray-600 text-sm">pessoas será afetada por transtornos mentais</p>
                    </div>
                    <div class="p-6">
                        <div class="text-4xl mb-2">🌱</div>
                        <div class="text-2xl font-bold text-green-600 mb-1">70%</div>
                        <p class="text-gray-600 text-sm">melhora com tratamento adequado</p>
                    </div>
                    <div class="p-6">
                        <div class="text-4xl mb-2">🤝</div>
                        <div class="text-2xl font-bold text-purple-600 mb-1">24/7</div>
                        <p class="text-gray-600 text-sm">suporte disponível (CVV 188)</p>
                    </div>
                    <div class="p-6">
                        <div class="text-4xl mb-2">🎯</div>
                        <div class="text-2xl font-bold text-orange-600 mb-1">100%</div>
                        <p class="text-gray-600 text-sm">baseado em evidências científicas</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seção de recursos -->
        <section id="features" class="py-16 bg-white">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-12">
                    <div class="text-5xl mb-4">🛠️</div>
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">Suas Ferramentas de Bem-Estar</h2>
                    <p class="text-xl text-gray-600 max-w-3xl mx-auto">
                        Recursos desenvolvidos com carinho e baseados em pesquisas científicas para cuidar da sua saúde mental
                    </p>
                </div>
                
                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Monitor de Humor -->
                    <div class="card-hover bg-gradient-to-br from-blue-50 to-blue-100 rounded-2xl shadow-lg p-8 border border-blue-200">
                        <div class="feature-icon text-5xl mb-4">📊</div>
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Monitor de Humor</h3>
                        <p class="text-gray-600 mb-4">Acompanhe seus sentimentos diários de forma simples e visual. Descubra padrões e celebre suas conquistas!</p>
                        <button onclick="showMoodTracker()" class="text-blue-600 font-medium hover:text-blue-800 transition-colors flex items-center">
                            Começar a monitorar 📈
                        </button>
                    </div>

                    <!-- Exercícios respiratórios -->
                    <div class="card-hover bg-gradient-to-br from-green-50 to-green-100 rounded-2xl shadow-lg p-8 border border-green-200">
                        <div class="feature-icon text-5xl mb-4">🌬️</div>
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Respiração Guiada</h3>
                        <p class="text-gray-600 mb-4">Exercícios de respiração relaxantes para acalmar a mente e reduzir a ansiedade. Respire e se sinta melhor!</p>
                        <button onclick="showBreathingExercise()" class="text-green-600 font-medium hover:text-green-800 transition-colors flex items-center">
                            Respirar comigo 😮‍💨
                        </button>
                    </div>

                    <!-- Ferramentas de avaliação -->
                    <div class="card-hover bg-gradient-to-br from-purple-50 to-purple-100 rounded-2xl shadow-lg p-8 border border-purple-200">
                        <div class="feature-icon text-5xl mb-4">🔍</div>
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Autoavaliação</h3>
                        <p class="text-gray-600 mb-4">Questionários científicos para entender melhor como você está se sentindo. Conhecimento é poder!</p>
                        <button onclick="showPage('assessment')" class="text-purple-600 font-medium hover:text-purple-800 transition-colors flex items-center">
                            Fazer avaliação ✨
                        </button>
                    </div>

                    <!-- Recursos Educacionais -->
                    <div class="card-hover bg-gradient-to-br from-yellow-50 to-yellow-100 rounded-2xl shadow-lg p-8 border border-yellow-200">
                        <div class="feature-icon text-5xl mb-4">📖</div>
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Aprenda Mais</h3>
                        <p class="text-gray-600 mb-4">Conteúdo educativo sobre saúde mental, dicas práticas e estratégias para o dia a dia. Conhecimento que transforma!</p>
                        <button onclick="showPage('resources')" class="text-yellow-600 font-medium hover:text-yellow-800 transition-colors flex items-center">
                            Explorar conteúdo 🎓
                        </button>
                    </div>

                    <!-- Diário de Gratidão -->
                    <div class="card-hover bg-gradient-to-br from-pink-50 to-pink-100 rounded-2xl shadow-lg p-8 border border-pink-200">
                        <div class="feature-icon text-5xl mb-4">💝</div>
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Diário de Gratidão</h3>
                        <p class="text-gray-600 mb-4">Registre momentos especiais e coisas pelas quais você é grato. A gratidão transforma perspectivas!</p>
                        <button onclick="showGratitudeJournal()" class="text-pink-600 font-medium hover:text-pink-800 transition-colors flex items-center">
                            Começar diário 📝
                        </button>
                    </div>

                    <!-- Suporte Profissional -->
                    <div class="card-hover bg-gradient-to-br from-red-50 to-red-100 rounded-2xl shadow-lg p-8 border border-red-200">
                        <div class="feature-icon text-5xl mb-4">🤝</div>
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Buscar Ajuda</h3>
                        <p class="text-gray-600 mb-4">Informações sobre como encontrar profissionais qualificados e recursos de emergência. Você não está sozinho!</p>
                        <button onclick="showProfessionalSupport()" class="text-red-600 font-medium hover:text-red-800 transition-colors flex items-center">
                            Ver recursos 🆘
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seção de Depoimentos -->
        <section class="py-16 bg-gradient-to-r from-blue-50 to-purple-50">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-12">
                    <div class="text-5xl mb-4">💬</div>
                    <h2 class="text-3xl font-bold text-gray-800 mb-4">O que as pessoas dizem</h2>
                    <p class="text-lg text-gray-600">Depoimentos de quem já começou a cuidar da saúde mental</p>
                </div>
                
                <div class="grid md:grid-cols-3 gap-8">
                    <div class="bg-white rounded-2xl p-6 shadow-lg">
                        <div class="text-3xl mb-4">😊</div>
                        <p class="text-gray-600 mb-4">"O monitor de humor me ajudou a perceber padrões que eu não via antes. Agora consigo me cuidar melhor!"</p>
                        <div class="font-semibold text-gray-800">- Alunos Pedro Do Mazza</div>
                    </div>
                    <div class="bg-white rounded-2xl p-6 shadow-lg">
                        <div class="text-3xl mb-4">🌬️</div>
                        <p class="text-gray-600 mb-4">"Os exercícios de respiração são incríveis! Uso sempre que me sinto ansioso e realmente funciona."</p>
                        <div class="font-semibold text-gray-800">- Ronielly, 19 anos</div>
                    </div>
                    <div class="bg-white rounded-2xl p-6 shadow-lg">
                        <div class="text-3xl mb-4">💙</div>
                        <p class="text-gray-600 mb-4">"A avaliação me deu insights importantes sobre minha saúde mental. Me senti acolhida e compreendida."</p>
                        <div class="font-semibold text-gray-800">- Ana, 18 anos</div>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!--Página de avaliação -->
    <div id="assessment-page" class="page hidden py-12">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <button onclick="showPage('home')" class="mb-8 text-blue-600 hover:text-blue-800 flex items-center font-medium">
                ← Voltar ao início
            </button>
            
            <div class="bg-white rounded-2xl shadow-xl p-8">
                <div class="text-center mb-8">
                    <div class="text-6xl mb-4">🔍</div>
                    <h1 class="text-3xl font-bold text-gray-800 mb-4">Como Você Está Se Sentindo?</h1>
                    <p class="text-lg text-gray-600">Um questionário carinhoso baseado em ciência para entender melhor seu bem-estar emocional</p>
                </div>
                
                <div id="assessment-container">
                    <div id="assessment-intro" class="text-center">
                        <div class="bg-blue-50 border-2 border-blue-200 rounded-2xl p-6 mb-8">
                            <div class="text-3xl mb-2">💙</div>
                            <h3 class="text-lg font-semibold text-blue-800 mb-2">Um momento importante</h3>
                            <p class="text-blue-700">Esta avaliação é um primeiro passo para conhecer melhor seus sentimentos. Lembre-se: buscar ajuda profissional é sempre uma opção válida e corajosa.</p>
                        </div>
                        
                        <div class="mb-8">
                            <h3 class="text-xl font-semibold text-gray-800 mb-6">O que vamos descobrir juntos:</h3>
                            <div class="grid md:grid-cols-2 gap-6">
                                <div class="bg-gradient-to-br from-blue-50 to-blue-100 p-6 rounded-2xl">
                                    <div class="text-3xl mb-2">😰</div>
                                    <h4 class="font-medium text-gray-800 mb-2">Níveis de Ansiedade</h4>
                                    <p class="text-gray-600 text-sm">Usando a escala GAD-7, reconhecida mundialmente</p>
                                </div>
                                <div class="bg-gradient-to-br from-green-50 to-green-100 p-6 rounded-2xl">
                                    <div class="text-3xl mb-2">😔</div>
                                    <h4 class="font-medium text-gray-800 mb-2">Sinais de Depressão</h4>
                                    <p class="text-gray-600 text-sm">Através do questionário PHQ-9, usado por profissionais</p>
                                </div>
                            </div>
                        </div>
                        
                        <button onclick="startAssessment()" class="bg-gradient-to-r from-blue-600 to-purple-600 text-white px-8 py-4 rounded-xl font-semibold hover:from-blue-700 hover:to-purple-700 transition duration-300 shadow-lg">
                            ✨ Vamos começar juntos
                        </button>
                    </div>
                    
                    <div id="assessment-questions" class="hidden">
                        <div class="mb-8">
                            <div class="flex justify-between items-center mb-4">
                                <span class="text-sm font-medium text-gray-600">Seu progresso</span>
                                <span class="text-sm font-medium text-gray-600"><span id="current-question">1</span> de <span id="total-questions">14</span></span>
                            </div>
                            <div class="w-full bg-gray-200 rounded-full h-3">
                                <div id="progress-bar" class="progress-bar bg-gradient-to-r from-blue-500 to-purple-500 h-3 rounded-full" style="width: 7%"></div>
                            </div>
                        </div>
                        
                        <div class="mb-8">
                            <h3 id="question-title" class="text-xl font-semibold text-gray-800 mb-6">Nas últimas 2 semanas, com que frequência você foi incomodado por nervosismo, ansiedade ou tensão?</h3>
                            
                            <div id="question-options" class="space-y-3">
                                <label class="flex items-center p-4 border-2 border-gray-200 rounded-xl hover:bg-blue-50 hover:border-blue-300 cursor-pointer transition-all">
                                    <input type="radio" name="question" value="0" class="mr-4 text-blue-600">
                                    <span class="text-lg">😌 Nenhuma vez</span>
                                </label>
                                <label class="flex items-center p-4 border-2 border-gray-200 rounded-xl hover:bg-blue-50 hover:border-blue-300 cursor-pointer transition-all">
                                    <input type="radio" name="question" value="1" class="mr-4 text-blue-600">
                                    <span class="text-lg">😐 Vários dias</span>
                                </label>
                                <label class="flex items-center p-4 border-2 border-gray-200 rounded-xl hover:bg-blue-50 hover:border-blue-300 cursor-pointer transition-all">
                                    <input type="radio" name="question" value="2" class="mr-4 text-blue-600">
                                    <span class="text-lg">😟 Mais da metade dos dias</span>
                                </label>
                                <label class="flex items-center p-4 border-2 border-gray-200 rounded-xl hover:bg-blue-50 hover:border-blue-300 cursor-pointer transition-all">
                                    <input type="radio" name="question" value="3" class="mr-4 text-blue-600">
                                    <span class="text-lg">😰 Quase todos os dias</span>
                                </label>
                            </div>
                        </div>
                        
                        <div class="flex justify-between">
                            <button id="prev-btn" onclick="previousQuestion()" class="bg-gray-300 text-gray-700 px-6 py-3 rounded-xl hover:bg-gray-400 transition duration-300 disabled:opacity-50" disabled>
                                ← Anterior
                            </button>
                            <button id="next-btn" onclick="nextQuestion()" class="bg-gradient-to-r from-blue-600 to-purple-600 text-white px-6 py-3 rounded-xl hover:from-blue-700 hover:to-purple-700 transition duration-300 disabled:opacity-50" disabled>
                                Próxima →
                            </button>
                        </div>
                    </div>
                    
                    <div id="assessment-results" class="hidden text-center">
                        <div class="text-5xl mb-6">📊</div>
                        <h2 class="text-2xl font-bold text-gray-800 mb-8">Seus Resultados</h2>
                        
                        <div class="grid md:grid-cols-2 gap-8 mb-8">
                            <div class="bg-gradient-to-br from-blue-50 to-blue-100 rounded-2xl p-6 border-2 border-blue-200">
                                <div class="text-3xl mb-2">😰</div>
                                <h3 class="text-lg font-semibold text-blue-800 mb-2">Ansiedade</h3>
                                <div class="text-4xl font-bold text-blue-600 mb-2" id="anxiety-score">0</div>
                                <p class="text-blue-700" id="anxiety-level">Nível mínimo</p>
                            </div>
                            
                            <div class="bg-gradient-to-br from-green-50 to-green-100 rounded-2xl p-6 border-2 border-green-200">
                                <div class="text-3xl mb-2">😔</div>
                                <h3 class="text-lg font-semibold text-green-800 mb-2">Humor Deprimido</h3>
                                <div class="text-4xl font-bold text-green-600 mb-2" id="depression-score">0</div>
                                <p class="text-green-700" id="depression-level">Nível mínimo</p>
                            </div>
                        </div>
                        
                        <div class="bg-gradient-to-br from-yellow-50 to-orange-50 border-2 border-yellow-200 rounded-2xl p-6 mb-8">
                            <div class="text-3xl mb-2">💡</div>
                            <h3 class="text-lg font-semibold text-yellow-800 mb-4">Suas Próximas Ações</h3>
                            <div id="recommendations" class="text-yellow-700">
                                <p>Com base nos seus resultados, aqui estão algumas sugestões carinhosas para cuidar do seu bem-estar.</p>
                            </div>
                        </div>
                        
                        <div class="flex flex-col sm:flex-row gap-4 justify-center">
                            <button onclick="restartAssessment()" class="bg-gradient-to-r from-blue-600 to-purple-600 text-white px-6 py-3 rounded-xl hover:from-blue-700 hover:to-purple-700 transition duration-300">
                                🔄 Refazer Avaliação
                            </button>
                            <button onclick="showPage('resources')" class="bg-gradient-to-r from-green-600 to-teal-600 text-white px-6 py-3 rounded-xl hover:from-green-700 hover:to-teal-700 transition duration-300">
                                📚 Ver Recursos
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Página de recursos -->
    <div id="resources-page" class="page hidden py-12">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <button onclick="showPage('home')" class="mb-8 text-blue-600 hover:text-blue-800 flex items-center font-medium">
                ← Voltar ao início
            </button>
            
            <div class="text-center mb-12">
                <div class="text-6xl mb-4">📚</div>
                <h1 class="text-4xl font-bold text-gray-800 mb-4">Aprenda e Cresça</h1>
                <p class="text-xl text-gray-600">Conhecimento que transforma e empodera sua jornada de bem-estar</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Recursos para ansiedade -->
                <div class="card-hover bg-gradient-to-br from-blue-50 to-blue-100 rounded-2xl shadow-lg p-6 border-2 border-blue-200">
                    <div class="text-5xl mb-4">😰</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-3">Entendendo a Ansiedade</h3>
                    <p class="text-gray-600 mb-4">Descubra o que é ansiedade, seus tipos e estratégias práticas para lidar com ela no dia a dia.</p>
                    <button onclick="showResourceContent('anxiety')" class="text-blue-600 font-medium hover:text-blue-800 transition-colors flex items-center">
                        Ler mais 📖
                    </button>
                </div>

                <!-- Recursos para depressão -->
                <div class="card-hover bg-gradient-to-br from-green-50 to-green-100 rounded-2xl shadow-lg p-6 border-2 border-green-200">
                    <div class="text-5xl mb-4">😔</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-3">Compreendendo a Depressão</h3>
                    <p class="text-gray-600 mb-4">Informações científicas sobre depressão, sinais de alerta e caminhos para a recuperação.</p>
                    <button onclick="showResourceContent('depression')" class="text-green-600 font-medium hover:text-green-800 transition-colors flex items-center">
                        Explorar 🌱
                    </button>
                </div>

                <!--Gerenciamento de estresse -->
                <div class="card-hover bg-gradient-to-br from-yellow-50 to-yellow-100 rounded-2xl shadow-lg p-6 border-2 border-yellow-200">
                    <div class="text-5xl mb-4">⚡</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-3">Gerenciando o Estresse</h3>
                    <p class="text-gray-600 mb-4">Técnicas comprovadas para identificar, compreender e transformar o estresse em energia positiva.</p>
                    <button onclick="showResourceContent('stress')" class="text-yellow-600 font-medium hover:text-yellow-800 transition-colors flex items-center">
                        Descobrir 💪
                    </button>
                </div>

                <!-- meditação -->
                <div class="card-hover bg-gradient-to-br from-purple-50 to-purple-100 rounded-2xl shadow-lg p-6 border-2 border-purple-200">
                    <div class="text-5xl mb-4">🧘</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-3">Mindfulness e Meditação</h3>
                    <p class="text-gray-600 mb-4">Práticas de atenção plena para cultivar paz interior e reduzir o estresse do cotidiano.</p>
                    <button onclick="showResourceContent('mindfulness')" class="text-purple-600 font-medium hover:text-purple-800 transition-colors flex items-center">
                        Praticar 🕯️
                    </button>
                </div>

                <!-- Higiene do Sono -->
                <div class="card-hover bg-gradient-to-br from-indigo-50 to-indigo-100 rounded-2xl shadow-lg p-6 border-2 border-indigo-200">
                    <div class="text-5xl mb-4">😴</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-3">Sono Reparador</h3>
                    <p class="text-gray-600 mb-4">Estratégias científicas para melhorar a qualidade do sono e seu impacto na saúde mental.</p>
                    <button onclick="showResourceContent('sleep')" class="text-indigo-600 font-medium hover:text-indigo-800 transition-colors flex items-center">
                        Aprender 🌙
                    </button>
                </div>

                <!-- Ajuda profissional  -->
                <div class="card-hover bg-gradient-to-br from-red-50 to-red-100 rounded-2xl shadow-lg p-6 border-2 border-red-200">
                    <div class="text-5xl mb-4">🤝</div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-3">Buscar Ajuda Profissional</h3>
                    <p class="text-gray-600 mb-4">Guia completo sobre quando e como procurar ajuda de psicólogos e outros profissionais.</p>
                    <button onclick="showResourceContent('professional')" class="text-red-600 font-medium hover:text-red-800 transition-colors flex items-center">
                        Ver guia 🆘
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- Página de ferramentas -->
    <div id="tools-page" class="page hidden py-12">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <button onclick="showPage('home')" class="mb-8 text-blue-600 hover:text-blue-800 flex items-center font-medium">
                ← Voltar ao início
            </button>
            
            <div class="text-center mb-12">
                <div class="text-6xl mb-4">🛠️</div>
                <h1 class="text-4xl font-bold text-gray-800 mb-4">Suas Ferramentas Interativas</h1>
                <p class="text-xl text-gray-600">Práticas diárias para cultivar bem-estar e autoconhecimento</p>
            </div>
            
            <div class="space-y-8">
                <!-- Mood Tracker Tool -->
                <div class="bg-white rounded-2xl shadow-xl p-8 border border-gray-100">
                    <div class="text-center mb-6">
                        <div class="text-5xl mb-4">📊</div>
                        <h2 class="text-2xl font-semibold text-gray-800 mb-2">Como Você Está Hoje?</h2>
                        <p class="text-gray-600">Registre seu humor e descubra padrões que podem ajudar no seu autocuidado</p>
                    </div>
                    
                    <div class="grid grid-cols-5 gap-4 mb-8">
                        <button onclick="recordMood(1, '😢')" class="mood-btn p-6 border-2 border-gray-200 rounded-2xl hover:border-blue-500 hover:bg-blue-50 transition-all text-center">
                            <div class="mood-emoji">😢</div>
                            <div class="text-sm text-gray-600 mt-2">Muito Baixo</div>
                        </button>
                        <button onclick="recordMood(2, '😔')" class="mood-btn p-6 border-2 border-gray-200 rounded-2xl hover:border-blue-500 hover:bg-blue-50 transition-all text-center">
                            <div class="mood-emoji">😔</div>
                            <div class="text-sm text-gray-600 mt-2">Baixo</div>
                        </button>
                        <button onclick="recordMood(3, '😐')" class="mood-btn p-6 border-2 border-gray-200 rounded-2xl hover:border-blue-500 hover:bg-blue-50 transition-all text-center">
                            <div class="mood-emoji">😐</div>
                            <div class="text-sm text-gray-600 mt-2">Neutro</div>
                        </button>
                        <button onclick="recordMood(4, '😊')" class="mood-btn p-6 border-2 border-gray-200 rounded-2xl hover:border-blue-500 hover:bg-blue-50 transition-all text-center">
                            <div class="mood-emoji">😊</div>
                            <div class="text-sm text-gray-600 mt-2">Bom</div>
                        </button>
                        <button onclick="recordMood(5, '😄')" class="mood-btn p-6 border-2 border-gray-200 rounded-2xl hover:border-blue-500 hover:bg-blue-50 transition-all text-center">
                            <div class="mood-emoji">😄</div>
                            <div class="text-sm text-gray-600 mt-2">Muito Bom</div>
                        </button>
                    </div>
                    
                    <div id="mood-history" class="bg-gradient-to-r from-blue-50 to-purple-50 rounded-2xl p-6">
                        <h3 class="font-semibold text-gray-800 mb-4 flex items-center">
                            📈 Seu Histórico dos Últimos 7 Dias
                        </h3>
                        <div id="mood-chart" class="text-center text-gray-500">
                            Registre seu primeiro humor para ver o histórico
                        </div>
                    </div>
                </div>

                <!-- Breathing Exercise Tool -->
                <div class="bg-white rounded-2xl shadow-xl p-8 border border-gray-100">
                    <div class="text-center mb-6">
                        <h2 class="text-2xl font-semibold text-gray-800 mb-2">Respiração Relaxante</h2>
                        <p class="text-gray-600">Técnica 4-7-8 para acalmar a mente e reduzir a ansiedade</p>
                    </div>
                    
                    <div class="text-center">
                        <div id="breathing-circle" class="breathing-circle w-40 h-40 mx-auto mb-8 rounded-full bg-gradient-to-r from-blue-400 to-purple-600 flex items-center justify-center text-white text-2xl font-bold shadow-lg">
                            🌬️
                        </div>
                        
                        <div id="breathing-instruction" class="text-xl text-gray-700 mb-8 h-8">
                            Clique no círculo para começar sua sessão de relaxamento
                        </div>
                        
                        <button id="breathing-start-btn" onclick="startBreathingExercise()" class="bg-gradient-to-r from-blue-600 to-purple-600 text-white px-8 py-4 rounded-xl font-semibold hover:from-blue-700 hover:to-purple-700 transition duration-300 shadow-lg">
                            ✨ Começar Respiração
                        </button>
                    </div>
                </div>

                <!-- Gratitude Journal -->
                <div class="bg-white rounded-2xl shadow-xl p-8 border border-gray-100">
                    <div class="text-center mb-6">
                        <div class="text-5xl mb-4">💝</div>
                        <h2 class="text-2xl font-semibold text-gray-800 mb-2">Diário de Gratidão</h2>
                        <p class="text-gray-600">Registre três coisas especiais do seu dia. A gratidão transforma perspectivas!</p>
                    </div>
                    
                    <div class="space-y-6 mb-8">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-3 flex items-center">
                                🌟 1. Hoje sou grato por...
                            </label>
                            <input type="text" id="gratitude-1" class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-blue-500" placeholder="Ex: Ter saúde para mais um dia">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-3 flex items-center">
                                💙 2. Também sou grato por...
                            </label>
                            <input type="text" id="gratitude-2" class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-blue-500" placeholder="Ex: O apoio da minha família">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-3 flex items-center">
                                ✨ 3. E ainda sou grato por...
                            </label>
                            <input type="text" id="gratitude-3" class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-blue-500" placeholder="Ex: A oportunidade de aprender algo novo">
                        </div>
                    </div>
                    
                    <div class="text-center">
                        <button onclick="saveGratitude()" class="bg-gradient-to-r from-pink-600 to-purple-600 text-white px-8 py-4 rounded-xl font-semibold hover:from-pink-700 hover:to-purple-700 transition duration-300 shadow-lg">
                            💝 Salvar Minha Gratidão
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- About Page -->
    <div id="about-page" class="page hidden py-12">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <button onclick="showPage('home')" class="mb-8 text-blue-600 hover:text-blue-800 flex items-center font-medium">
                ← Voltar ao início
            </button>
            
            <div class="bg-white rounded-2xl shadow-xl p-8">
                <div class="text-center mb-8">
                    <div class="text-6xl mb-4">🌸</div>
                    <h1 class="text-3xl font-bold text-gray-800 mb-4">Sobre o Eu Sou Você</h1>
                    <p class="text-lg text-gray-600">Uma plataforma feita com carinho para cuidar da sua saúde mental</p>
                </div>
                
                <div class="prose max-w-none">
                    <div class="bg-gradient-to-r from-blue-50 to-purple-50 p-6 rounded-2xl mb-8">
                        <h2 class="text-2xl font-semibold text-gray-800 mb-4 flex items-center">
                            💙 Nossa Missão
                        </h2>
                        <p class="text-gray-600 mb-4">O Eu Sou Você tem o objetivo de ajudar as pessoas a cuidarem da saúde mental e do bem-estar. Ele ensina maneiras simples de sentir melhor, como relaxar, ter hábitos saudáveis e entender quando é hora de procurar um médico, todo mundo pode aprender a se cuidar e viver melhor consigo mesmo.</h1>
                        </p>
                        <p class="text-gray-600">
                         Queremos democratizar o acesso ao conhecimento sobre bem-estar mental, oferecendo recursos baseados em evidências científicas de forma acessível e carinhosa.
                        </p>
                    </div>

                    <h2 class="text-2xl font-semibold text-gray-800 mb-4 flex items-center">
                        🔬 Nossa Abordagem Científica
                    </h2>
                    <p class="text-gray-600 mb-6">
                        Utilizamos instrumentos validados cientificamente, como o GAD-7 para ansiedade e PHQ-9 para depressão, garantindo que nossas avaliações sejam confiáveis e baseadas em padrões clínicos reconhecidos mundialmente.
                    </p>

                    <h2 class="text-2xl font-semibold text-gray-800 mb-4 flex items-center">
                        📚 Nossas Fontes
                    </h2>
                    <div class="grid md:grid-cols-2 gap-6 mb-8">
                        <div class="bg-blue-50 p-4 rounded-xl">
                            <div class="text-2xl mb-2">🌍</div>
                            <h3 class="font-semibold text-blue-800 mb-2">Organização Mundial da Saúde</h3>
                            <p class="text-blue-700 text-sm">Diretrizes globais sobre saúde mental e bem-estar</p>
                        </div>
                        <div class="bg-green-50 p-4 rounded-xl">
                            <div class="text-2xl mb-2">🏥</div>
                            <h3 class="font-semibold text-green-800 mb-2">American Psychological Association</h3>
                            <p class="text-green-700 text-sm">Práticas baseadas em evidências e instrumentos validados</p>
                        </div>
                        <div class="bg-yellow-50 p-4 rounded-xl">
                            <div class="text-2xl mb-2">🇧🇷</div>
                            <h3 class="font-semibold text-yellow-800 mb-2">Ministério da Saúde do Brasil</h3>
                            <p class="text-yellow-700 text-sm">Políticas nacionais de saúde mental e diretrizes do SUS</p>
                        </div>
                        <div class="bg-purple-50 p-4 rounded-xl">
                            <div class="text-2xl mb-2">🧠</div>
                            <h3 class="font-semibold text-purple-800 mb-2">Conselho Federal de Psicologia</h3>
                            <p class="text-purple-700 text-sm">Regulamentações e práticas profissionais em psicologia</p>
                        </div>
                    </div>

                    <div class="bg-gradient-to-r from-yellow-50 to-orange-50 border-l-4 border-yellow-400 p-6 rounded-r-2xl mb-8">
                        <div class="flex items-start">
                            <div class="text-2xl mr-3">⚠️</div>
                            <div>
                                <h3 class="font-semibold text-yellow-800 mb-2">Importante Lembrar</h3>
                                <p class="text-yellow-700">
                                    Esta plataforma tem caráter informativo e educacional. Não substitui o acompanhamento profissional. Em caso de crise ou pensamentos suicidas, procure ajuda imediatamente.
                                </p>
                            </div>
                        </div>
                    </div>

                    <h2 class="text-2xl font-semibold text-gray-800 mb-6 flex items-center">
                        🆘 Contatos de Emergência
                    </h2>
                    <div class="grid md:grid-cols-2 gap-6">
                        <div class="bg-gradient-to-br from-red-50 to-red-100 p-6 rounded-2xl border-2 border-red-200">
                            <div class="text-3xl mb-2">💙</div>
                            <h3 class="text-lg font-semibold text-red-800 mb-2">CVV - Centro de Valorização da Vida</h3>
                            <p class="text-3xl font-bold text-red-600 mb-2">188</p>
                            <p class="text-red-700">24 horas, gratuito e sigiloso</p>
                        </div>
                        <div class="bg-gradient-to-br from-blue-50 to-blue-100 p-6 rounded-2xl border-2 border-blue-200">
                            <div class="text-3xl mb-2">🚑</div>
                            <h3 class="text-lg font-semibold text-blue-800 mb-2">SAMU</h3>
                            <p class="text-3xl font-bold text-blue-600 mb-2">192</p>
                            <p class="text-blue-700">Emergências médicas</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Overlay -->
    <div id="modal-overlay" class="fixed inset-0 bg-black bg-opacity-50 hidden items-center justify-center z-50 p-4">
        <div class="bg-white rounded-2xl shadow-2xl p-8 max-w-md mx-auto max-h-96 overflow-y-auto">
            <div id="modal-content">
                <!-- Modal content will be inserted here -->
            </div>
        </div>
    </div>

    <script>
        // Global variables
        let currentAssessmentQuestion = 0;
        let assessmentAnswers = [];
        let breathingActive = false;
        let moodHistory = JSON.parse(localStorage.getItem('moodHistory') || '[]');
        
        // Assessment questions (GAD-7 + PHQ-9)
        const assessmentQuestions = [
            // GAD-7 Questions
            { type: 'anxiety', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por nervosismo, ansiedade ou tensão?' },
            { type: 'anxiety', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por não conseguir parar ou controlar as preocupações?' },
            { type: 'anxiety', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por preocupar-se muito com coisas diferentes?' },
            { type: 'anxiety', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por dificuldade para relaxar?' },
            { type: 'anxiety', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por ficar tão inquieto que se torna difícil permanecer sentado?' },
            { type: 'anxiety', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por ficar facilmente aborrecido ou irritado?' },
            { type: 'anxiety', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por sentir medo como se algo terrível fosse acontecer?' },
            
            // PHQ-9 Questions
            { type: 'depression', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por pouco interesse ou prazer em fazer as coisas?' },
            { type: 'depression', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por se sentir desanimado, deprimido ou sem esperança?' },
            { type: 'depression', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por dificuldade para adormecer, continuar dormindo ou dormir demais?' },
            { type: 'depression', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por se sentir cansado ou com pouca energia?' },
            { type: 'depression', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por falta de apetite ou comer demais?' },
            { type: 'depression', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por se sentir mal consigo mesmo ou sentir que é um fracasso?' },
            { type: 'depression', text: 'Nas últimas 2 semanas, com que frequência você foi incomodado por dificuldade para se concentrar em coisas como ler ou assistir televisão?' }
        ];
        
        // Page navigation
        function showPage(pageId) {
            document.querySelectorAll('.page').forEach(page => {
                page.classList.add('hidden');
            });
            document.getElementById(pageId + '-page').classList.remove('hidden');
            window.scrollTo(0, 0);
        }
        
        // Assessment functions
        function startAssessment() {
            document.getElementById('assessment-intro').classList.add('hidden');
            document.getElementById('assessment-questions').classList.remove('hidden');
            currentAssessmentQuestion = 0;
            assessmentAnswers = [];
            updateAssessmentQuestion();
        }
        
        function updateAssessmentQuestion() {
            const question = assessmentQuestions[currentAssessmentQuestion];
            document.getElementById('question-title').textContent = question.text;
            document.getElementById('current-question').textContent = currentAssessmentQuestion + 1;
            document.getElementById('total-questions').textContent = assessmentQuestions.length;
            
            const progress = ((currentAssessmentQuestion + 1) / assessmentQuestions.length) * 100;
            document.getElementById('progress-bar').style.width = progress + '%';
            
            // Clear previous selection
            document.querySelectorAll('input[name="question"]').forEach(input => {
                input.checked = false;
            });
            
            // Update button states
            document.getElementById('prev-btn').disabled = currentAssessmentQuestion === 0;
            document.getElementById('next-btn').disabled = true;
            
            // Add event listeners to radio buttons
            document.querySelectorAll('input[name="question"]').forEach(input => {
                input.addEventListener('change', function() {
                    document.getElementById('next-btn').disabled = false;
                });
            });
        }
        
        function nextQuestion() {
            const selectedAnswer = document.querySelector('input[name="question"]:checked');
            if (!selectedAnswer) return;
            
            assessmentAnswers[currentAssessmentQuestion] = parseInt(selectedAnswer.value);
            currentAssessmentQuestion++;
            
            if (currentAssessmentQuestion < assessmentQuestions.length) {
                updateAssessmentQuestion();
            } else {
                showAssessmentResults();
            }
        }
        
        function previousQuestion() {
            if (currentAssessmentQuestion > 0) {
                currentAssessmentQuestion--;
                updateAssessmentQuestion();
                
                // Restore previous answer
                if (assessmentAnswers[currentAssessmentQuestion] !== undefined) {
                    const value = assessmentAnswers[currentAssessmentQuestion];
                    document.querySelector(`input[name="question"][value="${value}"]`).checked = true;
                    document.getElementById('next-btn').disabled = false;
                }
            }
        }
        
        function showAssessmentResults() {
            document.getElementById('assessment-questions').classList.add('hidden');
            document.getElementById('assessment-results').classList.remove('hidden');
            
            // Calculate scores
            const anxietyScore = assessmentAnswers.slice(0, 7).reduce((sum, score) => sum + score, 0);
            const depressionScore = assessmentAnswers.slice(7, 14).reduce((sum, score) => sum + score, 0);
            
            // Update display
            document.getElementById('anxiety-score').textContent = anxietyScore;
            document.getElementById('depression-score').textContent = depressionScore;
            
            // Determine levels and recommendations
            const anxietyLevel = getAnxietyLevel(anxietyScore);
            const depressionLevel = getDepressionLevel(depressionScore);
            
            document.getElementById('anxiety-level').textContent = anxietyLevel;
            document.getElementById('depression-level').textContent = depressionLevel;
            
            // Generate recommendations
            const recommendations = generateRecommendations(anxietyScore, depressionScore);
            document.getElementById('recommendations').innerHTML = recommendations;
        }
        
        function getAnxietyLevel(score) {
            if (score <= 4) return 'Ansiedade mínima 😌';
            if (score <= 9) return 'Ansiedade leve 😐';
            if (score <= 14) return 'Ansiedade moderada 😟';
            return 'Ansiedade severa 😰';
        }
        
        function getDepressionLevel(score) {
            if (score <= 4) return 'Humor normal 😊';
            if (score <= 9) return 'Humor levemente baixo 😔';
            if (score <= 14) return 'Humor moderadamente baixo 😞';
            if (score <= 19) return 'Humor consideravelmente baixo 😢';
            return 'Humor muito baixo 😭';
        }
        
        function generateRecommendations(anxietyScore, depressionScore) {
            let recommendations = '<ul class="text-left space-y-3">';
            
            if (anxietyScore <= 4 && depressionScore <= 4) {
                recommendations += '<li class="flex items-start"><span class="mr-2">🌟</span> Continue mantendo suas práticas de autocuidado</li>';
                recommendations += '<li class="flex items-start"><span class="mr-2">💪</span> Pratique exercícios regulares e técnicas de relaxamento</li>';
                recommendations += '<li class="flex items-start"><span class="mr-2">📊</span> Continue monitorando seu bem-estar regularmente</li>';
            } else if (anxietyScore <= 9 || depressionScore <= 9) {
                recommendations += '<li class="flex items-start"><span class="mr-2">🧘</span> Considere técnicas de manejo do estresse e mindfulness</li>';
                recommendations += '<li class="flex items-start"><span class="mr-2">🌬️</span> Pratique exercícios de respiração diariamente</li>';
                recommendations += '<li class="flex items-start"><span class="mr-2">😴</span> Mantenha uma rotina saudável de sono e exercícios</li>';
                recommendations += '<li class="flex items-start"><span class="mr-2">💬</span> Considere conversar com um profissional de saúde mental</li>';
            } else {
                recommendations += '<li class="flex items-start"><span class="mr-2 text-red-600">🚨</span> <strong>Recomendamos buscar ajuda profissional</strong></li>';
                recommendations += '<li class="flex items-start"><span class="mr-2">🤝</span> Considere terapia psicológica ou acompanhamento médico</li>';
                recommendations += '<li class="flex items-start"><span class="mr-2">💙</span> Pratique técnicas de autocuidado diariamente</li>';
                recommendations += '<li class="flex items-start"><span class="mr-2">👥</span> Mantenha uma rede de apoio social</li>';
            }
            
            if (anxietyScore >= 15 || depressionScore >= 15) {
                recommendations += '<li class="flex items-start text-red-600"><span class="mr-2">🆘</span> <strong>Se você está tendo pensamentos de autolesão, procure ajuda imediatamente (CVV: 188)</strong></li>';
            }
            
            recommendations += '</ul>';
            return recommendations;
        }
        
        function restartAssessment() {
            document.getElementById('assessment-results').classList.add('hidden');
            document.getElementById('assessment-intro').classList.remove('hidden');
            currentAssessmentQuestion = 0;
            assessmentAnswers = [];
        }
        
        // Mood tracking functions
        function recordMood(level, emoji) {
            const today = new Date().toISOString().split('T')[0];
            
            // Remove existing entry for today
            moodHistory = moodHistory.filter(entry => entry.date !== today);
            
            // Add new entry
            moodHistory.push({ date: today, level: level, emoji: emoji });
            
            // Keep only last 30 days
            moodHistory = moodHistory.slice(-30);
            
            // Save to localStorage
            localStorage.setItem('moodHistory', JSON.stringify(moodHistory));
            
            // Update display
            updateMoodChart();
            
            // Visual feedback
            showModal('Humor Registrado! 🎉', `Seu humor de hoje foi registrado como ${emoji}. Continue monitorando para identificar padrões e celebrar suas conquistas!`);
        }
        
        function updateMoodChart() {
            const chartContainer = document.getElementById('mood-chart');
            
            if (moodHistory.length === 0) {
                chartContainer.innerHTML = '<p class="text-gray-500">Registre seu primeiro humor para ver o histórico 📊</p>';
                return;
            }
            
            // Get last 7 days
            const last7Days = moodHistory.slice(-7);
            
            let chartHTML = '<div class="flex justify-between items-end h-24 mb-4 bg-white rounded-xl p-4">';
            
            last7Days.forEach(entry => {
                const height = (entry.level / 5) * 100;
                const colors = ['bg-red-400', 'bg-orange-400', 'bg-yellow-400', 'bg-green-400', 'bg-blue-400'];
                const colorClass = colors[entry.level - 1];
                
                chartHTML += `
                    <div class="flex flex-col items-center">
                        <div class="${colorClass} rounded-t-lg transition-all hover:opacity-80" style="height: ${height}%; width: 24px; min-height: 12px;"></div>
                        <div class="text-lg mt-2">${entry.emoji}</div>
                        <div class="text-xs text-gray-500 mt-1">${new Date(entry.date).getDate()}</div>
                    </div>
                `;
            });
            
            chartHTML += '</div>';
            chartHTML += '<p class="text-sm text-gray-600 text-center">📅 Últimos 7 registros de humor</p>';
            
            chartContainer.innerHTML = chartHTML;
        }
        
        // Breathing exercise functions
        function startBreathingExercise() {
            if (breathingActive) return;
            
            breathingActive = true;
            const circle = document.getElementById('breathing-circle');
            const instruction = document.getElementById('breathing-instruction');
            const btn = document.getElementById('breathing-start-btn');
            
            btn.textContent = '⏳ Exercício em andamento...';
            btn.disabled = true;
            
            let phase = 'prepare';
            let count = 3;
            
            // Preparation phase
            const prepareInterval = setInterval(() => {
                circle.textContent = count;
                instruction.textContent = `Preparando sua sessão... ${count}`;
                count--;
                
                if (count < 0) {
                    clearInterval(prepareInterval);
                    startBreathingCycle();
                }
            }, 1000);
        }
        
        function startBreathingCycle() {
            const circle = document.getElementById('breathing-circle');
            const instruction = document.getElementById('breathing-instruction');
            
            let cycles = 0;
            const maxCycles = 4;
            
            function runCycle() {
                if (cycles >= maxCycles) {
                    finishBreathingExercise();
                    return;
                }
                
                // Inhale phase (4 seconds)
                let count = 4;
                instruction.textContent = '🌬️ Inspire lentamente pelo nariz...';
                circle.style.transform = 'scale(1.3)';
                circle.style.background = 'linear-gradient(45deg, #3B82F6, #8B5CF6)';
                
                const inhaleInterval = setInterval(() => {
                    circle.textContent = count;
                    count--;
                    
                    if (count < 0) {
                        clearInterval(inhaleInterval);
                        holdPhase();
                    }
                }, 1000);
                
                function holdPhase() {
                    // Hold phase (7 seconds)
                    let count = 7;
                    instruction.textContent = '⏸️ Segure a respiração suavemente...';
                    circle.style.background = 'linear-gradient(45deg, #10B981, #059669)';
                    
                    const holdInterval = setInterval(() => {
                        circle.textContent = count;
                        count--;
                        
                        if (count < 0) {
                            clearInterval(holdInterval);
                            exhalePhase();
                        }
                    }, 1000);
                }
                
                function exhalePhase() {
                    // Exhale phase (8 seconds)
                    let count = 8;
                    instruction.textContent = '💨 Expire lentamente pela boca...';
                    circle.style.transform = 'scale(1)';
                    circle.style.background = 'linear-gradient(45deg, #8B5CF6, #EC4899)';
                    
                    const exhaleInterval = setInterval(() => {
                        circle.textContent = count;
                        count--;
                        
                        if (count < 0) {
                            clearInterval(exhaleInterval);
                            cycles++;
                            setTimeout(runCycle, 1000);
                        }
                    }, 1000);
                }
            }
            
            runCycle();
        }
        
        function finishBreathingExercise() {
            const circle = document.getElementById('breathing-circle');
            const instruction = document.getElementById('breathing-instruction');
            const btn = document.getElementById('breathing-start-btn');
            
            circle.textContent = '✨';
            circle.style.transform = 'scale(1)';
            circle.style.background = 'linear-gradient(45deg, #10B981, #059669)';
            instruction.textContent = '🎉 Exercício concluído! Como se sente agora?';
            
            btn.textContent = '🔄 Respirar Novamente';
            btn.disabled = false;
            breathingActive = false;
            
            setTimeout(() => {
                circle.textContent = '🌬️';
                circle.style.background = 'linear-gradient(45deg, #3B82F6, #8B5CF6)';
                instruction.textContent = 'Clique no círculo para começar sua sessão de relaxamento';
            }, 4000);
        }
        
        // Gratitude journal functions
        function saveGratitude() {
            const gratitude1 = document.getElementById('gratitude-1').value.trim();
            const gratitude2 = document.getElementById('gratitude-2').value.trim();
            const gratitude3 = document.getElementById('gratitude-3').value.trim();
            
            if (!gratitude1 || !gratitude2 || !gratitude3) {
                showModal('Campos Incompletos 📝', 'Por favor, preencha todos os três campos de gratidão. Cada pequena coisa conta!');
                return;
            }
            
            const today = new Date().toISOString().split('T')[0];
            const gratitudeEntry = {
                date: today,
                items: [gratitude1, gratitude2, gratitude3]
            };
            
            // Save to localStorage
            let gratitudeHistory = JSON.parse(localStorage.getItem('gratitudeHistory') || '[]');
            gratitudeHistory = gratitudeHistory.filter(entry => entry.date !== today);
            gratitudeHistory.push(gratitudeEntry);
            localStorage.setItem('gratitudeHistory', JSON.stringify(gratitudeHistory));
            
            // Clear form
            document.getElementById('gratitude-1').value = '';
            document.getElementById('gratitude-2').value = '';
            document.getElementById('gratitude-3').value = '';
            
            showModal('Gratidão Registrada! 💝', 'Seu registro de gratidão foi salvo com carinho! A prática regular de gratidão está associada a maior bem-estar e felicidade. Continue assim! ✨');
        }
        
        // Modal functions
        function showModal(title, content) {
            document.getElementById('modal-content').innerHTML = `
                <div class="text-center">
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">${title}</h3>
                    <p class="text-gray-600 mb-6">${content}</p>
                    <button onclick="closeModal()" class="bg-gradient-to-r from-blue-600 to-purple-600 text-white px-6 py-3 rounded-xl hover:from-blue-700 hover:to-purple-700 transition duration-300">
                        ✨ Fechar
                    </button>
                </div>
            `;
            document.getElementById('modal-overlay').classList.remove('hidden');
            document.getElementById('modal-overlay').classList.add('flex');
        }
        
        function closeModal() {
            document.getElementById('modal-overlay').classList.add('hidden');
            document.getElementById('modal-overlay').classList.remove('flex');
        }
        
        // Resource content functions
        function showResourceContent(type) {
            const content = {
                anxiety: {
                    title: '😰 Entendendo a Ansiedade',
                    content: `
                        <div class="text-left">
                            <h4 class="font-semibold mb-3 flex items-center">🤔 O que é Ansiedade?</h4>
                            <p class="mb-4">A ansiedade é uma resposta natural do nosso corpo a situações de perigo ou estresse. Ela se torna um problema quando é excessiva, persistente e interfere na nossa vida diária.</p>
                            
                            <h4 class="font-semibold mb-3 flex items-center">🎭 Tipos Principais:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>😰 Transtorno de Ansiedade Generalizada (TAG)</li>
                                <li>😱 Transtorno do Pânico</li>
                                <li>😨 Fobias Específicas</li>
                                <li>😳 Transtorno de Ansiedade Social</li>
                            </ul>
                            
                            <h4 class="font-semibold mb-3 flex items-center">💪 Estratégias que Ajudam:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>🫁 Técnicas de respiração e relaxamento</li>
                                <li>🏃‍♀️ Exercícios físicos regulares</li>
                                <li>🧠 Terapia Cognitivo-Comportamental</li>
                                <li>🧘 Mindfulness e meditação</li>
                                <li>💤 Higiene do sono adequada</li>
                            </ul>
                        </div>
                    `
                },
                depression: {
                    title: '😔 Compreendendo a Depressão',
                    content: `
                        <div class="text-left">
                            <h4 class="font-semibold mb-3 flex items-center">💙 O que é Depressão?</h4>
                            <p class="mb-4">A depressão é mais que tristeza passageira. É um transtorno mental caracterizado por sentimentos persistentes de tristeza, desesperança e perda de interesse em atividades que antes traziam prazer.</p>
                            
                            <h4 class="font-semibold mb-3 flex items-center">🚨 Sinais Importantes:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>😞 Humor deprimido na maior parte do dia</li>
                                <li>😴 Perda de interesse em atividades prazerosas</li>
                                <li>🛏️ Alterações no sono e apetite</li>
                                <li>⚡ Fadiga e perda de energia</li>
                                <li>💭 Sentimentos de inutilidade ou culpa excessiva</li>
                                <li>🧠 Dificuldade de concentração</li>
                            </ul>
                            
                            <h4 class="font-semibold mb-3 flex items-center">🌱 Caminhos para Recuperação:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>💬 Psicoterapia (especialmente TCC)</li>
                                <li>💊 Medicação quando indicada por profissional</li>
                                <li>🏃‍♂️ Exercícios físicos regulares</li>
                                <li>👥 Apoio social e familiar</li>
                                <li>🎯 Estabelecimento de rotinas saudáveis</li>
                            </ul>
                        </div>
                    `
                },
                stress: {
                    title: '⚡ Gerenciando o Estresse',
                    content: `
                        <div class="text-left">
                            <h4 class="font-semibold mb-3 flex items-center">🤯 O que é Estresse?</h4>
                            <p class="mb-4">O estresse é uma resposta natural do organismo a situações desafiadoras. Em pequenas doses, pode ser motivador. Porém, quando crônico, pode prejudicar nossa saúde física e mental.</p>
                            
                            <h4 class="font-semibold mb-3 flex items-center">⚠️ Sinais de Estresse Crônico:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>💪 Tensão muscular constante</li>
                                <li>🧠 Dificuldades de concentração</li>
                                <li>😤 Irritabilidade frequente</li>
                                <li>😴 Problemas de sono</li>
                                <li>🤕 Sintomas físicos (dores de cabeça, problemas digestivos)</li>
                                <li>😰 Ansiedade e preocupação excessiva</li>
                            </ul>
                            
                            <h4 class="font-semibold mb-3 flex items-center">🛠️ Técnicas de Manejo:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>🧘 Técnicas de relaxamento progressivo</li>
                                <li>⏰ Gestão eficaz do tempo</li>
                                <li>🚫 Estabelecimento de limites saudáveis</li>
                                <li>🏃‍♀️ Atividade física regular</li>
                                <li>🌱 Práticas de mindfulness</li>
                                <li>😴 Priorização do descanso</li>
                            </ul>
                        </div>
                    `
                },
                mindfulness: {
                    title: '🧘 Mindfulness e Meditação',
                    content: `
                        <div class="text-left">
                            <h4 class="font-semibold mb-3 flex items-center">🌟 O que é Mindfulness?</h4>
                            <p class="mb-4">Mindfulness é a prática de estar presente no momento atual, observando pensamentos e sentimentos sem julgamento. É uma ferramenta poderosa para reduzir estresse e ansiedade.</p>
                            
                            <h4 class="font-semibold mb-3 flex items-center">💙 Benefícios Comprovados:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>😌 Redução do estresse e ansiedade</li>
                                <li>🧠 Melhora da concentração</li>
                                <li>😴 Melhor qualidade do sono</li>
                                <li>💪 Fortalecimento da resiliência emocional</li>
                                <li>❤️ Aumento da autocompaixão</li>
                            </ul>
                            
                            <h4 class="font-semibold mb-3 flex items-center">🎯 Práticas Simples:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>🫁 Respiração consciente (5-10 minutos diários)</li>
                                <li>🚶‍♀️ Caminhada mindful</li>
                                <li>🍽️ Alimentação consciente</li>
                                <li>📱 Meditações guiadas por apps</li>
                                <li>🌅 Momentos de pausa durante o dia</li>
                            </ul>
                        </div>
                    `
                },
                sleep: {
                    title: '😴 Sono Reparador',
                    content: `
                        <div class="text-left">
                            <h4 class="font-semibold mb-3 flex items-center">💤 Por que o Sono é Importante?</h4>
                            <p class="mb-4">O sono de qualidade é fundamental para a saúde mental. Durante o sono, nosso cérebro processa emoções, consolida memórias e se prepara para um novo dia.</p>
                            
                            <h4 class="font-semibold mb-3 flex items-center">🚨 Sinais de Sono Inadequado:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>😴 Sonolência durante o dia</li>
                                <li>😤 Irritabilidade e mudanças de humor</li>
                                <li>🧠 Dificuldade de concentração</li>
                                <li>🤒 Maior suscetibilidade a doenças</li>
                                <li>⚡ Baixa energia e motivação</li>
                            </ul>
                            
                            <h4 class="font-semibold mb-3 flex items-center">🌙 Dicas para Melhor Sono:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>⏰ Mantenha horários regulares para dormir e acordar</li>
                                <li>📱 Evite telas 1 hora antes de dormir</li>
                                <li>🛏️ Crie um ambiente confortável e escuro</li>
                                <li>☕ Evite cafeína após 14h</li>
                                <li>🧘 Pratique relaxamento antes de dormir</li>
                                <li>🏃‍♀️ Exercite-se regularmente (mas não antes de dormir)</li>
                            </ul>
                        </div>
                    `
                },
                professional: {
                    title: '🤝 Buscar Ajuda Profissional',
                    content: `
                        <div class="text-left">
                            <h4 class="font-semibold mb-3 flex items-center">🚨 Quando Buscar Ajuda:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>⏰ Sintomas persistem por mais de 2 semanas</li>
                                <li>🏠 Interferem significativamente na vida diária</li>
                                <li>💭 Pensamentos de autolesão ou suicídio</li>
                                <li>🍺 Uso de substâncias para lidar com emoções</li>
                                <li>😰 Ataques de pânico frequentes</li>
                                <li>😔 Perda de interesse em tudo</li>
                            </ul>
                            
                            <h4 class="font-semibold mb-3 flex items-center">🏥 Onde Encontrar Ajuda:</h4>
                            <ul class="list-disc list-inside mb-4 space-y-2">
                                <li>🏥 CAPS - Centros de Atenção Psicossocial (SUS)</li>
                                <li>👨‍⚕️ Psicólogos e psiquiatras particulares</li>
                                <li>🏥 Unidades Básicas de Saúde</li>
                                <li>🏥 Hospitais com serviços de psiquiatria</li>
                                <li>📞 Linhas de apoio emocional</li>
                            </ul>
                            
                            <div class="bg-red-50 p-4 rounded-xl mt-4 border-2 border-red-200">
                                <h4 class="font-semibold text-red-800 mb-2 flex items-center">🆘 Emergência:</h4>
                                <p class="text-red-700 font-semibold">CVV: 188 (24h, gratuito e sigiloso)</p>
                                <p class="text-red-700">SAMU: 192 (emergências médicas)</p>
                            </div>
                        </div>
                    `
                }
            };
            
            if (content[type]) {
                showModal(content[type].title, content[type].content);
            }
        }
        
        // Helper functions for features
        function showMoodTracker() {
            showModal('Monitor de Humor 📊', 'O monitoramento regular do humor ajuda a identificar padrões e gatilhos emocionais. Acesse a página de Ferramentas para usar o monitor completo e começar sua jornada de autoconhecimento! ✨');
        }
        
        function showBreathingExercise() {
            showModal('Exercício de Respiração 🫁', 'Os exercícios de respiração são técnicas comprovadas para redução da ansiedade e promoção do relaxamento. Acesse a página de Ferramentas para praticar o exercício guiado e sentir a diferença! 🌬️');
        }
        
        function showGratitudeJournal() {
            showModal('Diário de Gratidão 💝', 'A prática da gratidão está cientificamente associada a maior bem-estar e felicidade. Acesse a página de Ferramentas para começar seu diário e transformar sua perspectiva! ✨');
        }
        
        function showProfessionalSupport() {
            showModal('Suporte Profissional 🤝', `
                <div class="text-left">
                    <h4 class="font-semibold mb-3 flex items-center">🚨 Quando Buscar Ajuda:</h4>
                    <ul class="list-disc list-inside mb-4 space-y-2">
                        <li>Sintomas persistem por mais de 2 semanas</li>
                        <li>Interferem significativamente na vida diária</li>
                        <li>Pensamentos de autolesão ou suicídio</li>
                        <li>Uso de substâncias para lidar com emoções</li>
                    </ul>
                    
                    <h4 class="font-semibold mb-3 flex items-center">🏥 Onde Encontrar Ajuda:</h4>
                    <ul class="list-disc list-inside mb-4 space-y-2">
                        <li>CAPS - Centros de Atenção Psicossocial (SUS)</li>
                        <li>Psicólogos e psiquiatras particulares</li>
                        <li>Unidades Básicas de Saúde</li>
                        <li>Hospitais com serviços de psiquiatria</li>
                    </ul>
                    
                    <div class="bg-red-50 p-3 rounded-lg mt-4 border border-red-200">
                        <div style="display: flex; gap: 20px;">

</div>

                    </div>
                </div>
            `);
        }
        
        // Initialize page
        document.addEventListener('DOMContentLoaded', function() {
            showPage('home');
            updateMoodChart();
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'969e1d2966f780fe',t:'MTc1NDMxMTEyOC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
