<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Origens - Centro de Fonoaudiologia | Dr. Fernando Manoel Macedo</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Fontes -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&display=swap" rel="stylesheet">
    
    <!-- Ícones -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- Three.js -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>

    <script>
        // ==========================================
        // ESQUEMA DE CORES: AZUL PETRÓLEO + PRATA
        // ==========================================
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'origem-dark': '#0A192F',
                        'origem-light': '#F4F7F6',
                        'origem-gold': '#C0C0C0', // Prata
                        'origem-teal': '#112240',
                    },
                    fontFamily: {
                        'sans': ['Montserrat', 'sans-serif'],
                        'serif': ['Playfair Display', 'serif'],
                    }
                }
            }
        }
    </script>
    <style>
        body { background-color: #0A192F; color: #F4F7F6; overflow-x: hidden; margin: 0; }
        #canvas-container { position: fixed; top: 0; left: 0; width: 100vw; height: 100vh; z-index: 0; }
        
        .glass-panel {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.3);
        }
        .glass-panel-dark {
            background: rgba(10, 25, 47, 0.85);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(192, 192, 192, 0.2);
        }

        /* Card Informativo Moderno */
        .info-card {
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
            border-left: 4px solid #C0C0C0;
        }
        .info-card:hover {
            transform: translateX(5px);
            background: rgba(255, 255, 255, 0.05);
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }

        /* Timeline */
        .timeline-item::before {
            content: '';
            position: absolute;
            left: -24px;
            top: 0;
            bottom: 0;
            width: 2px;
            background: rgba(192, 192, 192, 0.2);
        }
        .timeline-item.active::before { background: #C0C0C0; }

        /* Admin Panel */
        .admin-panel { 
            transform: translateX(100%); transition: transform 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: fixed; top: 0; right: 0; width: 100%; max-width: 450px; height: 100vh; 
            background: rgba(10, 25, 47, 0.98); backdrop-filter: blur(20px);
            border-left: 1px solid rgba(192, 192, 192, 0.3); z-index: 9999; 
            overflow-y: auto; padding: 30px; 
        }
        .admin-panel.active { transform: translateX(0); }
        .admin-input { width: 100%; padding: 10px; margin-bottom: 15px; background: rgba(255,255,255,0.05); border: 1px solid rgba(255,255,255,0.1); border-radius: 6px; color: white; font-family: 'Montserrat', sans-serif; font-size: 0.9rem; }
        .admin-input:focus { outline: none; border-color: #C0C0C0; }
        .admin-label { font-weight: 500; font-size: 0.75rem; color: #C0C0C0; margin-bottom: 5px; display: block; text-transform: uppercase; letter-spacing: 1px;}

        .fade-in-up { animation: fadeInUp 1s ease-out forwards; opacity: 0; transform: translateY(30px); }
        .delay-1 { animation-delay: 0.2s; }
        .delay-2 { animation-delay: 0.4s; }
        @keyframes fadeInUp { to { opacity: 1; transform: translateY(0); } }

        .logo-svg { height: 40px; width: auto; }
        @media (min-width: 768px) { .logo-svg { height: 50px; } }

        /* Header Styles */
        .top-bar { background: rgba(0,0,0,0.3); border-bottom: 1px solid rgba(255,255,255,0.05); }
        .navbar { background: rgba(10, 25, 47, 0.9); backdrop-filter: blur(20px); border-bottom: 1px solid rgba(192, 192, 192, 0.1); }
        .nav-link { position: relative; transition: color 0.3s; }
        .nav-link::after { content: ''; position: absolute; width: 0; height: 2px; bottom: -4px; left: 0; background-color: #C0C0C0; transition: width 0.3s; }
        .nav-link:hover::after { width: 100%; }
    </style>
</head>
<body class="font-sans antialiased">

    <!-- Fundo 3D Temático -->
    <div id="canvas-container"></div>

    <!-- Botão Admin -->
    <button onclick="toggleAdmin()" class="fixed bottom-6 right-6 glass-panel p-4 rounded-full shadow-lg z-50 hover:bg-white/10 transition group">
        <i class="fas fa-cog text-origem-gold text-xl group-hover:rotate-90 transition-transform duration-500"></i>
    </button>

    <!-- PAINEL ADMINISTRATIVO -->
    <div id="adminPanel" class="admin-panel">
        <div class="flex justify-between items-center mb-6 border-b border-white/10 pb-4">
            <h2 class="font-serif text-xl text-origem-gold">Painel Comercial</h2>
            <button onclick="toggleAdmin()" class="text-gray-400 hover:text-white"><i class="fas fa-times text-xl"></i></button>
        </div>
        
        <form id="adminForm" onsubmit="saveData(event)">
            <h3 class="text-white font-bold mb-3 border-b border-white/10 pb-1">Topo (Hero)</h3>
            <label class="admin-label">Título Principal</label>
            <input type="text" id="edit_hero_title" class="admin-input">
            <label class="admin-label">Subtítulo</label>
            <textarea id="edit_hero_subtitle" class="admin-input" rows="2"></textarea>

            <h3 class="text-white font-bold mb-3 mt-6 border-b border-white/10 pb-1">Depoimentos</h3>
            <label class="admin-label">Depoimento 1</label>
            <textarea id="edit_test1" class="admin-input" rows="2"></textarea>
            <label class="admin-label">Depoimento 2</label>
            <textarea id="edit_test2" class="admin-input" rows="2"></textarea>

            <h3 class="text-white font-bold mb-3 mt-6 border-b border-white/10 pb-1">Rodapé</h3>
            <label class="admin-label">Endereço</label>
            <input type="text" id="edit_footer_address" class="admin-input">
            <label class="admin-label">Telefone/WhatsApp</label>
            <input type="text" id="edit_footer_phone" class="admin-input">

            <button type="submit" class="w-full bg-origem-gold text-origem-dark py-3 rounded-lg font-bold hover:bg-yellow-500 transition mt-4">
                Salvar Alterações
            </button>
        </form>
    </div>

    <!-- LANDING PAGE -->
    <div class="relative z-10">
        
        <!-- CABEÇALHO RICO EM INFORMAÇÕES -->
        <header class="fixed top-0 left-0 right-0 z-50">
            <!-- Top Bar (Informações de Contato) -->
            <div class="top-bar py-2 px-4 md:px-6 hidden md:block">
                <div class="container mx-auto flex justify-between items-center text-xs text-gray-400">
                    <div class="flex items-center gap-6">
                        <span class="flex items-center gap-2"><i class="fas fa-phone-alt text-origem-gold"></i> (34) 3333-4444</span>
                        <span class="flex items-center gap-2"><i class="fas fa-envelope text-origem-gold"></i> contato@origemfono.com.br</span>
                        <span class="flex items-center gap-2"><i class="fas fa-map-marker-alt text-origem-gold"></i> Uberaba - MG</span>
                    </div>
                    <div class="flex items-center gap-4">
                        <span class="text-origem-gold font-semibold">Siga-nos:</span>
                        <a href="#" class="hover:text-white transition"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="hover:text-white transition"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="hover:text-white transition"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#" class="hover:text-white transition"><i class="fab fa-whatsapp"></i></a>
                    </div>
                </div>
            </div>

            <!-- Navbar Principal -->
            <nav class="navbar py-3 px-4 md:px-6">
                <div class="container mx-auto flex justify-between items-center">
                    <!-- Logo -->
                    <div class="flex items-center gap-3">
                        <svg class="logo-svg" viewBox="0 0 300 80" xmlns="http://www.w3.org/2000/svg">
                            <g transform="translate(10, 10)">
                                <path d="M20,10 C30,10 40,20 40,35 C40,50 30,60 20,60 C10,60 0,50 0,35 C0,20 10,10 20,10 Z" fill="none" stroke="#C0C0C0" stroke-width="2"/>
                                <path d="M20,15 Q30,25 25,40" fill="none" stroke="#C0C0C0" stroke-width="1.5"/>
                                <path d="M35,25 Q45,25 45,35 Q45,45 35,45" fill="none" stroke="#C0C0C0" stroke-width="2"/>
                                <circle cx="38" cy="32" r="1.5" fill="#C0C0C0"/>
                                <path d="M50,30 Q55,25 60,30" fill="none" stroke="#C0C0C0" stroke-width="2"/>
                                <path d="M52,35 Q58,28 64,35" fill="none" stroke="#C0C0C0" stroke-width="1.5"/>
                            </g>
                            <text x="90" y="45" font-family="'Playfair Display', serif" font-weight="700" font-size="28" fill="#F4F7F6" letter-spacing="4">ORIGEM</text>
                            <text x="92" y="60" font-family="'Montserrat', sans-serif" font-size="8" fill="#A0A0A0" letter-spacing="2">CENTRO DE FONOAUDIOLOGIA</text>
                        </svg>
                    </div>

                    <!-- Menu Desktop -->
                    <ul class="hidden lg:flex items-center gap-8 text-sm font-medium text-gray-300">
                        <li><a href="#" class="nav-link text-white">Início</a></li>
                        <li><a href="#sobre" class="nav-link hover:text-white">Especialista</a></li>
                        <li><a href="#servicos" class="nav-link hover:text-white">Serviços</a></li>
                        <li><a href="#" class="nav-link hover:text-white">Depoimentos</a></li>
                        <li><a href="#contato" class="nav-link hover:text-white">Contato</a></li>
                    </ul>

                    <!-- CTA Desktop -->
                    <div class="hidden lg:flex items-center gap-4">
                        <a href="#contato" class="bg-origem-gold text-origem-dark px-6 py-2.5 rounded-full font-bold text-sm hover:scale-105 transition shadow-lg shadow-origem-gold/20">
                            Agendar Consulta
                        </a>
                    </div>

                    <!-- Menu Mobile Button -->
                    <button onclick="toggleMobileMenu()" class="lg:hidden text-white text-2xl focus:outline-none">
                        <i class="fas fa-bars"></i>
                    </button>
                </div>

                <!-- Menu Mobile Dropdown -->
                <div id="mobileMenu" class="hidden lg:hidden mt-4 pb-4 border-t border-white/10 pt-4">
                    <ul class="flex flex-col gap-4 text-sm font-medium text-gray-300">
                        <li><a href="#" class="block hover:text-origem-gold transition">Início</a></li>
                        <li><a href="#sobre" class="block hover:text-origem-gold transition">Especialista</a></li>
                        <li><a href="#servicos" class="block hover:text-origem-gold transition">Serviços</a></li>
                        <li><a href="#" class="block hover:text-origem-gold transition">Depoimentos</a></li>
                        <li><a href="#contato" class="block hover:text-origem-gold transition">Contato</a></li>
                        <li class="pt-2">
                            <a href="#contato" class="block text-center bg-origem-gold text-origem-dark px-6 py-3 rounded-full font-bold text-sm">
                                Agendar Consulta
                            </a>
                        </li>
                    </ul>
                    <div class="flex gap-4 mt-6 justify-center text-origem-gold">
                        <a href="#"><i class="fab fa-instagram text-xl"></i></a>
                        <a href="#"><i class="fab fa-facebook-f text-xl"></i></a>
                        <a href="#"><i class="fab fa-whatsapp text-xl"></i></a>
                    </div>
                </div>
            </nav>
        </header>

        <!-- Espaçador para compensar o header fixo -->
        <div class="h-[140px] md:h-[120px]"></div>

        <!-- Hero Section -->
        <section class="min-h-[80vh] flex items-center pt-8 pb-12">
            <div class="container mx-auto px-4 md:px-6 flex flex-col md:flex-row items-center gap-12">
                <div class="md:w-3/5 fade-in-up delay-1">
                    <div class="inline-block bg-origem-gold/20 border border-origem-gold text-origem-gold px-4 py-1 rounded-full text-xs font-bold tracking-widest mb-6">
                        REFERÊNCIA EM COMUNICAÇÃO HUMANA
                    </div>
                    <h2 id="hero_title" class="font-serif text-4xl md:text-6xl lg:text-7xl text-white leading-tight mb-6">
                        Toda comunicação tem uma origem.
                    </h2>
                    <p id="hero_subtitle" class="text-base md:text-xl text-gray-300 mb-10 font-light max-w-2xl">
                        E compreender essa origem é o primeiro passo para desenvolver novas possibilidades.
                    </p>
                    <div class="flex flex-col sm:flex-row gap-4">
                        <a href="#contato" class="bg-origem-gold text-origem-dark px-8 py-4 rounded-full font-bold text-lg hover:scale-105 transition transform shadow-lg shadow-origem-gold/30 text-center">
                            Agendar Consulta
                        </a>
                        <a href="#sobre" class="glass-panel text-white px-8 py-4 rounded-full font-semibold text-lg hover:bg-white/10 transition text-center">
                            Conhecer o Especialista
                        </a>
                    </div>
                </div>
                
                <div class="md:w-2/5 fade-in-up delay-2">
                    <div class="glass-panel-dark p-6 rounded-3xl relative overflow-hidden group hover:scale-[1.02] transition duration-500 border border-origem-gold/30">
                        <div class="absolute -top-20 -right-20 w-40 h-40 bg-origem-gold rounded-full blur-[80px] opacity-20"></div>
                        <!-- FOTO DO DR. FERNANDO AQUI -->
                        <img src="https://images.unsplash.com/photo-1612349317150-e413f6a5b16d?q=80&w=800&auto=format&fit=crop" alt="Dr. Fernando Manoel Macedo" class="rounded-2xl w-full object-cover h-[300px] md:h-[400px] mb-4 border border-white/10 shadow-2xl">
                        <h3 class="font-serif text-2xl text-origem-gold mb-1">Dr. Fernando Manoel Macedo</h3>
                        <p class="text-gray-400 tracking-widest uppercase text-xs font-semibold mb-3">Fonoaudiólogo</p>
                        <p class="text-gray-300 text-sm italic border-l-2 border-origem-gold pl-3">"Ciência, escuta e propósito em cada fase da comunicação."</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seção de Qualificações Profissionais -->
        <section id="sobre" class="py-20 bg-black/40 relative">
            <div class="container mx-auto px-4 md:px-6">
                <div class="text-center mb-16">
                    <h3 class="font-serif text-3xl md:text-4xl text-white mb-4">Qualificações e Formação</h3>
                    <p class="text-gray-400 max-w-2xl mx-auto">A base científica e o aperfeiçoamento contínuo para oferecer o melhor tratamento.</p>
                </div>

                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6 max-w-6xl mx-auto">
                    <div class="glass-panel p-6 rounded-2xl flex flex-col items-center text-center gap-4 hover:-translate-y-2 transition border-t-2 border-t-origem-gold">
                        <div class="w-16 h-16 rounded-full bg-origem-gold/20 flex items-center justify-center text-origem-gold text-2xl">
                            <i class="fas fa-graduation-cap"></i>
                        </div>
                        <h4 class="font-bold text-white text-lg">Graduação</h4>
                        <p class="text-gray-400 text-sm">Graduado pela Universidade de Uberaba</p>
                    </div>

                    <div class="glass-panel p-6 rounded-2xl flex flex-col items-center text-center gap-4 hover:-translate-y-2 transition border-t-2 border-t-origem-gold">
                        <div class="w-16 h-16 rounded-full bg-origem-gold/20 flex items-center justify-center text-origem-gold text-2xl">
                            <i class="fas fa-book-open"></i>
                        </div>
                        <h4 class="font-bold text-white text-lg">Pós-Graduação</h4>
                        <p class="text-gray-400 text-sm">Especialista em Linguagem</p>
                    </div>

                    <div class="glass-panel p-6 rounded-2xl flex flex-col items-center text-center gap-4 hover:-translate-y-2 transition border-t-2 border-t-origem-gold">
                        <div class="w-16 h-16 rounded-full bg-origem-gold/20 flex items-center justify-center text-origem-gold text-2xl">
                            <i class="fas fa-ear-listen"></i>
                        </div>
                        <h4 class="font-bold text-white text-lg">Aperfeiçoamento</h4>
                        <p class="text-gray-400 text-sm">Audiologia pelo CEFAC</p>
                    </div>

                    <div class="glass-panel p-6 rounded-2xl flex flex-col items-center text-center gap-4 hover:-translate-y-2 transition border-t-2 border-t-origem-gold">
                        <div class="w-16 h-16 rounded-full bg-origem-gold/20 flex items-center justify-center text-origem-gold text-2xl">
                            <i class="fas fa-child"></i>
                        </div>
                        <h4 class="font-bold text-white text-lg">Teste da Linguinha</h4>
                        <p class="text-gray-400 text-sm">Curso para Realização do Teste da Linguinha</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seção Informativa: O que investigamos + Jornada do Paciente -->
        <section id="servicos" class="py-20 relative">
            <div class="container mx-auto px-4 md:px-6">
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 max-w-6xl mx-auto">
                    
                    <!-- Coluna Esquerda: O que investigamos -->
                    <div class="fade-in-up">
                        <h3 class="font-serif text-3xl md:text-4xl text-white mb-6">O que uma avaliação fonoaudiológica pode investigar?</h3>
                        <p class="text-gray-400 mb-8">A avaliação vai muito além de observar se a pessoa "fala certo ou errado".</p>
                        
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                            <div class="info-card glass-panel p-4 rounded-xl">
                                <i class="fas fa-brain text-origem-gold text-xl mb-2"></i>
                                <h4 class="font-bold text-white text-sm">Compreensão</h4>
                                <p class="text-xs text-gray-400 mt-1">Entender e processar informações</p>
                            </div>
                            <div class="info-card glass-panel p-4 rounded-xl">
                                <i class="fas fa-comment-dots text-origem-gold text-xl mb-2"></i>
                                <h4 class="font-bold text-white text-sm">Expressão Oral</h4>
                                <p class="text-xs text-gray-400 mt-1">Usar palavras e frases com clareza</p>
                            </div>
                            <div class="info-card glass-panel p-4 rounded-xl">
                                <i class="fas fa-wave-square text-origem-gold text-xl mb-2"></i>
                                <h4 class="font-bold text-white text-sm">Produção dos Sons</h4>
                                <p class="text-xs text-gray-400 mt-1">Articular os sons de forma adequada</p>
                            </div>
                            <div class="info-card glass-panel p-4 rounded-xl">
                                <i class="fas fa-puzzle-piece text-origem-gold text-xl mb-2"></i>
                                <h4 class="font-bold text-white text-sm">Organização</h4>
                                <p class="text-xs text-gray-400 mt-1">Estruturar ideias com sentido</p>
                            </div>
                            <div class="info-card glass-panel p-4 rounded-xl">
                                <i class="fas fa-water text-origem-gold text-xl mb-2"></i>
                                <h4 class="font-bold text-white text-sm">Fluência</h4>
                                <p class="text-xs text-gray-400 mt-1">Ritmo e continuidade na fala</p>
                            </div>
                            <div class="info-card glass-panel p-4 rounded-xl">
                                <i class="fas fa-microphone text-origem-gold text-xl mb-2"></i>
                                <h4 class="font-bold text-white text-sm">Voz</h4>
                                <p class="text-xs text-gray-400 mt-1">Qualidade vocal para cada contexto</p>
                            </div>
                            <div class="info-card glass-panel p-4 rounded-xl">
                                <i class="fas fa-face-smile text-origem-gold text-xl mb-2"></i>
                                <h4 class="font-bold text-white text-sm">Funções Orofaciais</h4>
                                <p class="text-xs text-gray-400 mt-1">Respiração, sucção e mastigação</p>
                            </div>
                            <div class="info-card glass-panel p-4 rounded-xl">
                                <i class="fas fa-users text-origem-gold text-xl mb-2"></i>
                                <h4 class="font-bold text-white text-sm">Impacto Social</h4>
                                <p class="text-xs text-gray-400 mt-1">Como afeta a vida diária</p>
                            </div>
                        </div>
                    </div>

                    <!-- Coluna Direita: Jornada do Paciente -->
                    <div class="fade-in-up delay-1">
                        <h3 class="font-serif text-3xl md:text-4xl text-white mb-6">Como funciona o nosso atendimento?</h3>
                        <p class="text-gray-400 mb-8">Na Origens, a conduta começa pela compreensão do caso, não pela escolha imediata de exercícios.</p>
                        
                        <div class="relative pl-8 space-y-8">
                            <div class="timeline-item active relative">
                                <div class="absolute -left-[31px] top-0 w-4 h-4 rounded-full bg-origem-gold border-4 border-origem-dark"></div>
                                <h4 class="font-bold text-white text-lg">1. Escuta e Anamnese</h4>
                                <p class="text-gray-400 text-sm mt-1">Ouvimos a história do paciente e entendemos o impacto da comunicação na vida diária.</p>
                            </div>
                            <div class="timeline-item active relative">
                                <div class="absolute -left-[31px] top-0 w-4 h-4 rounded-full bg-origem-gold border-4 border-origem-dark"></div>
                                <h4 class="font-bold text-white text-lg">2. Avaliação Detalhada</h4>
                                <p class="text-gray-400 text-sm mt-1">Analisamos todo o sistema de fala, voz e audição, e não apenas os sons isolados.</p>
                            </div>
                            <div class="timeline-item active relative">
                                <div class="absolute -left-[31px] top-0 w-4 h-4 rounded-full bg-origem-gold border-4 border-origem-dark"></div>
                                <h4 class="font-bold text-white text-lg">3. Devolutiva e Plano Terapêutico</h4>
                                <p class="text-gray-400 text-sm mt-1">Explicamos o diagnóstico e traçamos um plano personalizado, baseado em ciência.</p>
                            </div>
                            <div class="timeline-item relative">
                                <div class="absolute -left-[31px] top-0 w-4 h-4 rounded-full bg-gray-600 border-4 border-origem-dark"></div>
                                <h4 class="font-bold text-gray-500 text-lg">4. Terapia e Evolução</h4>
                                <p class="text-gray-500 text-sm mt-1">Acompanhamento contínuo com foco na evolução e autonomia do paciente.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seção de Cards Informativos (Baseado nas Imagens) -->
        <section class="py-24 bg-black/20">
            <div class="container mx-auto px-4 md:px-6">
                <div class="text-center mb-16">
                    <h3 class="font-serif text-3xl md:text-4xl text-white mb-4">Informação de Qualidade para Pais e Pacientes</h3>
                    <p class="text-gray-400 max-w-2xl mx-auto">Conteúdo baseado em ciência para você entender quando e como buscar ajuda especializada.</p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 max-w-6xl mx-auto">
                    <div class="glass-panel-dark rounded-2xl overflow-hidden info-card border-l-4 border-l-origem-gold">
                        <div class="h-40 overflow-hidden relative">
                            <img src="https://images.unsplash.com/photo-1519689680058-324335c77eba?q=80&w=800&auto=format&fit=crop" alt="Criança" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-gradient-to-t from-origem-dark to-transparent"></div>
                        </div>
                        <div class="p-6">
                            <h4 class="font-serif text-xl text-white mb-2">Meu filho fala pouco para a idade.</h4>
                            <p class="text-origem-gold text-xs font-semibold mb-3 uppercase tracking-wider">Isso é motivo de atenção?</p>
                            <p class="text-gray-400 text-sm leading-relaxed">Nem sempre falar pouco significa um atraso, mas alguns sinais ajudam a entender quando vale investigar.</p>
                        </div>
                    </div>

                    <div class="glass-panel-dark rounded-2xl overflow-hidden info-card border-l-4 border-l-origem-gold">
                        <div class="h-40 overflow-hidden relative">
                            <img src="https://images.unsplash.com/photo-1503454537195-1dcabb73ffb9?q=80&w=800&auto=format&fit=crop" alt="Mãe e filho" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-gradient-to-t from-origem-dark to-transparent"></div>
                        </div>
                        <div class="p-6">
                            <h4 class="font-serif text-xl text-white mb-2">Meninos realmente falam mais tarde?</h4>
                            <p class="text-origem-gold text-xs font-semibold mb-3 uppercase tracking-wider">Justificativa comum para adiar avaliação.</p>
                            <p class="text-gray-400 text-sm leading-relaxed">Existem diferenças individuais, mas os marcos comunicativos continuam sendo importantes. A evolução importa mais que a comparação.</p>
                        </div>
                    </div>

                    <div class="glass-panel-dark rounded-2xl overflow-hidden info-card border-l-4 border-l-origem-gold">
                        <div class="h-40 overflow-hidden relative">
                            <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?q=80&w=800&auto=format&fit=crop" alt="Mulher" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-gradient-to-t from-origem-dark to-transparent"></div>
                        </div>
                        <div class="p-6">
                            <h4 class="font-serif text-xl text-white mb-2">Sua voz cansa antes do fim do dia?</h4>
                            <p class="text-origem-gold text-xs font-semibold mb-3 uppercase tracking-wider">Ouça esse sinal.</p>
                            <p class="text-gray-400 text-sm leading-relaxed">A rouquidão persistente e o cansaço vocal não devem ser ignorados. A avaliação investiga a saúde da sua voz.</p>
                        </div>
                    </div>

                    <div class="glass-panel-dark rounded-2xl overflow-hidden info-card border-l-4 border-l-origem-gold">
                        <div class="p-6">
                            <div class="flex items-center gap-3 mb-3">
                                <i class="fas fa-exclamation-triangle text-origem-gold text-xl"></i>
                                <h4 class="font-serif text-lg text-white">Um erro comum</h4>
                            </div>
                            <p class="text-gray-400 text-sm leading-relaxed mb-3">Avaliar a fala observando apenas os sons que estão errados.</p>
                            <p class="text-gray-300 text-sm leading-relaxed border-t border-white/10 pt-3">Para compreender uma alteração, é importante analisar como ela acontece dentro de todo o sistema de fala.</p>
                        </div>
                    </div>

                    <div class="glass-panel-dark rounded-2xl overflow-hidden info-card border-l-4 border-l-origem-gold">
                        <div class="p-6">
                            <div class="flex items-center gap-3 mb-3">
                                <i class="fas fa-clipboard-check text-origem-gold text-xl"></i>
                                <h4 class="font-serif text-lg text-white">Antes do Plano Terapêutico</h4>
                            </div>
                            <p class="text-gray-400 text-sm leading-relaxed mb-3">O que acontece antes de definir um plano?</p>
                            <p class="text-gray-300 text-sm leading-relaxed border-t border-white/10 pt-3">Na Origens, a conduta começa pela compreensão do caso, não pela escolha imediata de exercícios.</p>
                        </div>
                    </div>

                    <div class="glass-panel-dark rounded-2xl overflow-hidden info-card border-l-4 border-l-origem-gold">
                        <div class="p-6">
                            <div class="flex items-center gap-3 mb-3">
                                <i class="fas fa-clock text-origem-gold text-xl"></i>
                                <h4 class="font-serif text-lg text-white">Respeitar o tempo da criança</h4>
                            </div>
                            <p class="text-gray-400 text-sm leading-relaxed mb-3">Não significa ignorar sinais de dificuldade.</p>
                            <p class="text-gray-300 text-sm leading-relaxed border-t border-white/10 pt-3">Cada criança tem seu ritmo, mas o acompanhamento profissional é fundamental para garantir um desenvolvimento saudável.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seção de Depoimentos -->
        <section class="py-20 relative">
            <div class="container mx-auto px-4 md:px-6 relative z-10">
                <div class="text-center mb-16">
                    <h3 class="font-serif text-3xl md:text-4xl text-white mb-4">O que nossos pacientes dizem</h3>
                    <div class="flex justify-center text-origem-gold gap-1 mb-4">
                        <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                    </div>
                    <p class="text-gray-400">Avaliações reais de quem confia no nosso trabalho.</p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 max-w-6xl mx-auto">
                    <div class="glass-panel p-8 rounded-3xl relative">
                        <i class="fas fa-quote-left text-origem-gold text-4xl opacity-20 absolute top-6 left-6"></i>
                        <p id="test1" class="text-gray-300 italic mb-6 relative z-10 mt-6">"O Dr. Fernando teve uma paciência incrível com meu filho. Em poucas sessões, já notamos uma diferença enorme na clareza da fala dele. Profissional excepcional!"</p>
                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 rounded-full bg-origem-gold/20 flex items-center justify-center text-origem-gold font-bold">M</div>
                            <div>
                                <h5 class="text-white font-bold text-sm">Mariana Silva</h5>
                                <p class="text-gray-500 text-xs">Mãe do Théo (4 anos)</p>
                            </div>
                        </div>
                    </div>

                    <div class="glass-panel p-8 rounded-3xl relative">
                        <i class="fas fa-quote-left text-origem-gold text-4xl opacity-20 absolute top-6 left-6"></i>
                        <p id="test2" class="text-gray-300 italic mb-6 relative z-10 mt-6">"Eu sofria com cansaço vocal todos os dias no trabalho. A avaliação foi super detalhada e o tratamento mudou minha qualidade de vida. Recomendo de olhos fechados."</p>
                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 rounded-full bg-origem-gold/20 flex items-center justify-center text-origem-gold font-bold">C</div>
                            <div>
                                <h5 class="text-white font-bold text-sm">Carlos Mendes</h5>
                                <p class="text-gray-500 text-xs">Professor</p>
                            </div>
                        </div>
                    </div>

                    <div class="glass-panel p-8 rounded-3xl relative lg:col-span-1 md:col-span-2 lg:col-span-1">
                        <i class="fas fa-quote-left text-origem-gold text-4xl opacity-20 absolute top-6 left-6"></i>
                        <p class="text-gray-300 italic mb-6 relative z-10 mt-6">"A abordagem da clínica é totalmente diferente. Eles não só tratam, mas explicam o porquê de cada exercício. Me senti acolhida e segura durante todo o processo."</p>
                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 rounded-full bg-origem-gold/20 flex items-center justify-center text-origem-gold font-bold">A</div>
                            <div>
                                <h5 class="text-white font-bold text-sm">Ana Paula Rocha</h5>
                                <p class="text-gray-500 text-xs">Paciente de Audição</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- RODAPÉ PROFISSIONAL -->
        <footer id="contato" class="pt-20 pb-10 relative overflow-hidden bg-black/60 border-t border-white/10">
            <div class="container mx-auto px-4 md:px-6 relative z-10 max-w-6xl mx-auto">
                
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-10 mb-16">
                    
                    <div class="col-span-1">
                        <div class="mb-6">
                            <svg class="logo-svg" viewBox="0 0 300 80" xmlns="http://www.w3.org/2000/svg">
                                <g transform="translate(10, 10)">
                                    <path d="M20,10 C30,10 40,20 40,35 C40,50 30,60 20,60 C10,60 0,50 0,35 C0,20 10,10 20,10 Z" fill="none" stroke="#C0C0C0" stroke-width="2"/>
                                    <path d="M20,15 Q30,25 25,40" fill="none" stroke="#C0C0C0" stroke-width="1.5"/>
                                    <path d="M35,25 Q45,25 45,35 Q45,45 35,45" fill="none" stroke="#C0C0C0" stroke-width="2"/>
                                    <circle cx="38" cy="32" r="1.5" fill="#C0C0C0"/>
                                    <path d="M50,30 Q55,25 60,30" fill="none" stroke="#C0C0C0" stroke-width="2"/>
                                    <path d="M52,35 Q58,28 64,35" fill="none" stroke="#C0C0C0" stroke-width="1.5"/>
                                </g>
                                <text x="90" y="45" font-family="'Playfair Display', serif" font-weight="700" font-size="28" fill="#F4F7F6" letter-spacing="4">ORIGEM</text>
                                <text x="92" y="60" font-family="'Montserrat', sans-serif" font-size="8" fill="#A0A0A0" letter-spacing="2">CENTRO DE FONOAUDIOLOGIA</text>
                            </svg>
                        </div>
                        <p class="text-gray-400 text-sm mb-6 leading-relaxed">Ciência, escuta e propósito em cada fase da comunicação.</p>
                        <div class="flex gap-3">
                            <a href="#" class="w-9 h-9 rounded-full glass-panel flex items-center justify-center text-origem-gold hover:bg-origem-gold hover:text-origem-dark transition text-sm"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="w-9 h-9 rounded-full glass-panel flex items-center justify-center text-origem-gold hover:bg-origem-gold hover:text-origem-dark transition text-sm"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="w-9 h-9 rounded-full glass-panel flex items-center justify-center text-origem-gold hover:bg-origem-gold hover:text-origem-dark transition text-sm"><i class="fab fa-linkedin-in"></i></a>
                            <a href="#" class="w-9 h-9 rounded-full glass-panel flex items-center justify-center text-origem-gold hover:bg-origem-gold hover:text-origem-dark transition text-sm"><i class="fab fa-whatsapp"></i></a>
                        </div>
                    </div>

                    <div>
                        <h4 class="text-white font-bold mb-6 uppercase tracking-wider text-sm border-b border-origem-gold/30 pb-2 inline-block">Navegação</h4>
                        <ul class="space-y-3 text-gray-400 text-sm">
                            <li><a href="#" class="hover:text-origem-gold transition flex items-center gap-2"><i class="fas fa-chevron-right text-xs text-origem-gold"></i> Início</a></li>
                            <li><a href="#sobre" class="hover:text-origem-gold transition flex items-center gap-2"><i class="fas fa-chevron-right text-xs text-origem-gold"></i> Sobre o Especialista</a></li>
                            <li><a href="#servicos" class="hover:text-origem-gold transition flex items-center gap-2"><i class="fas fa-chevron-right text-xs text-origem-gold"></i> Serviços</a></li>
                            <li><a href="#" class="hover:text-origem-gold transition flex items-center gap-2"><i class="fas fa-chevron-right text-xs text-origem-gold"></i> Depoimentos</a></li>
                            <li><a href="#" class="hover:text-origem-gold transition flex items-center gap-2"><i class="fas fa-chevron-right text-xs text-origem-gold"></i> Blog</a></li>
                        </ul>
                    </div>

                    <div>
                        <h4 class="text-white font-bold mb-6 uppercase tracking-wider text-sm border-b border-origem-gold/30 pb-2 inline-block">Contato</h4>
                        <ul class="space-y-4 text-gray-400 text-sm">
                            <li class="flex items-start gap-3">
                                <i class="fas fa-map-marker-alt text-origem-gold mt-1"></i>
                                <span id="footer_address">Av. Exemplo, 1234 - Sala 56<br>Centro, Uberaba - MG</span>
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fas fa-phone-alt text-origem-gold"></i>
                                <span id="footer_phone">(34) 3333-4444</span>
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fab fa-whatsapp text-origem-gold"></i>
                                <span>(34) 99999-8888</span>
                            </li>
                            <li class="flex items-center gap-3">
                                <i class="fas fa-envelope text-origem-gold"></i>
                                <span>contato@origemfono.com.br</span>
                            </li>
                        </ul>
                    </div>

                    <div>
                        <h4 class="text-white font-bold mb-6 uppercase tracking-wider text-sm border-b border-origem-gold/30 pb-2 inline-block">Horários</h4>
                        <ul class="space-y-3 text-gray-400 text-sm">
                            <li class="flex justify-between border-b border-white/5 pb-2">
                                <span>Segunda - Sexta</span>
                                <span class="text-white font-semibold">08:00 - 19:00</span>
                            </li>
                            <li class="flex justify-between border-b border-white/5 pb-2">
                                <span>Sábado</span>
                                <span class="text-white font-semibold">08:00 - 12:00</span>
                            </li>
                            <li class="flex justify-between">
                                <span>Domingo</span>
                                <span class="text-origem-gold">Fechado</span>
                            </li>
                        </ul>
                        <div class="mt-6">
                            <a href="#" class="block text-center bg-origem-gold text-origem-dark px-6 py-3 rounded-lg font-bold hover:bg-white transition text-sm">
                                Agendar Horário
                            </a>
                        </div>
                    </div>
                </div>

                <div class="border-t border-white/10 pt-8 flex flex-col md:flex-row justify-between items-center text-xs text-gray-500">
                    <p>&copy; 2024 Origens - Centro de Fonoaudiologia. Todos os direitos reservados.</p>
                    <div class="flex gap-6 mt-4 md:mt-0">
                        <a href="#" class="hover:text-origem-gold transition">Política de Privacidade</a>
                        <a href="#" class="hover:text-origem-gold transition">Termos de Uso</a>
                        <p>Desenvolvido com <i class="fas fa-heart text-red-500 mx-1"></i> para a saúde</p>
                    </div>
                </div>
            </div>
        </footer>
    </div>

    <!-- Scripts -->
    <script>
        // Menu Mobile
        function toggleMobileMenu() {
            const menu = document.getElementById('mobileMenu');
            menu.classList.toggle('hidden');
        }

        const defaultData = {
            hero_title: "Toda comunicação tem uma origem.",
            hero_subtitle: "E compreender essa origem é o primeiro passo para desenvolver novas possibilidades.",
            test1: "\"O Dr. Fernando teve uma paciência incrível com meu filho. Em poucas sessões, já notamos uma diferença enorme na clareza da fala dele. Profissional excepcional!\"",
            test2: "\"Eu sofria com cansaço vocal todos os dias no trabalho. A avaliação foi super detalhada e o tratamento mudou minha qualidade de vida. Recomendo de olhos fechados.\"",
            footer_address: "Av. Exemplo, 1234 - Sala 56<br>Centro, Uberaba - MG",
            footer_phone: "(34) 3333-4444"
        };

        function loadData() {
            const savedData = JSON.parse(localStorage.getItem('origemComercial')) || defaultData;
            document.getElementById('hero_title').innerText = savedData.hero_title;
            document.getElementById('hero_subtitle').innerText = savedData.hero_subtitle;
            document.getElementById('test1').innerText = savedData.test1;
            document.getElementById('test2').innerText = savedData.test2;
            document.getElementById('footer_address').innerHTML = savedData.footer_address;
            document.getElementById('footer_phone').innerText = savedData.footer_phone;

            document.getElementById('edit_hero_title').value = savedData.hero_title;
            document.getElementById('edit_hero_subtitle').value = savedData.hero_subtitle;
            document.getElementById('edit_test1').value = savedData.test1;
            document.getElementById('edit_test2').value = savedData.test2;
            document.getElementById('edit_footer_address').value = savedData.footer_address;
            document.getElementById('edit_footer_phone').value = savedData.footer_phone;
        }

        function saveData(event) {
            event.preventDefault();
            const newData = {
                hero_title: document.getElementById('edit_hero_title').value,
                hero_subtitle: document.getElementById('edit_hero_subtitle').value,
                test1: document.getElementById('edit_test1').value,
                test2: document.getElementById('edit_test2').value,
                footer_address: document.getElementById('edit_footer_address').value,
                footer_phone: document.getElementById('edit_footer_phone').value
            };
            localStorage.setItem('origemComercial', JSON.stringify(newData));
            loadData();
            toggleAdmin();
            
            const btn = event.target.querySelector('button');
            btn.innerHTML = '<i class="fas fa-check mr-2"></i> Salvo!';
            setTimeout(() => btn.innerHTML = 'Salvar Alterações', 2000);
        }

        function toggleAdmin() { document.getElementById('adminPanel').classList.toggle('active'); }
        window.onload = loadData;

        // ==========================================
        // FUNDO 3D TEMÁTICO: ONDAS SONORAS + REDE NEURAL
        // ==========================================
        const container = document.getElementById('canvas-container');
        const scene = new THREE.Scene();
        const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
        const renderer = new THREE.WebGLRenderer({ alpha: true, antialias: true });
        renderer.setSize(window.innerWidth, window.innerHeight);
        renderer.setPixelRatio(window.devicePixelRatio);
        container.appendChild(renderer.domElement);

        // 1. ONDAS SONORAS (Waveform 3D)
        const waveGroup = new THREE.Group();
        const waveCount = 5; // Quantidade de ondas
        const waveColors = [0xC0C0C0, 0x112240, 0x2A5A50]; // Prata, Azul escuro, Verde água

        for (let w = 0; w < waveCount; w++) {
            const points = [];
            const segments = 100;
            const width = 20;
            const amplitude = 0.5 + (w * 0.2); // Ondas diferentes
            const offset = (w - waveCount/2) * 1.5; // Espaçamento entre ondas
            const speed = 0.5 + (w * 0.1); // Velocidade diferente para cada onda

            for (let i = 0; i <= segments; i++) {
                const x = (i / segments - 0.5) * width;
                const y = Math.sin(i * 0.2 + w) * amplitude;
                points.push(new THREE.Vector3(x, y, offset));
            }

            const geometry = new THREE.BufferGeometry().setFromPoints(points);
            const material = new THREE.LineBasicMaterial({ 
                color: waveColors[w % waveColors.length], 
                transparent: true, 
                opacity: 0.3 - (w * 0.05) 
            });
            const line = new THREE.Line(geometry, material);
            line.userData = { basePoints: points, speed: speed, amplitude: amplitude, offset: offset };
            waveGroup.add(line);
        }
        scene.add(waveGroup);

        // 2. REDE NEURAL (Partículas conectadas)
        const particlesGeometry = new THREE.BufferGeometry();
        const particlesCount = 600;
        const posArray = new Float32Array(particlesCount * 3);
        for(let i = 0; i < particlesCount * 3; i++) { 
            posArray[i] = (Math.random() - 0.5) * 25; 
        }
        particlesGeometry.setAttribute('position', new THREE.BufferAttribute(posArray, 3));
        const particlesMaterial = new THREE.PointsMaterial({ 
            size: 0.02, 
            color: 0xC0C0C0, 
            transparent: true, 
            opacity: 0.8, 
            blending: THREE.AdditiveBlending 
        });
        const particlesMesh = new THREE.Points(particlesGeometry, particlesMaterial);
        scene.add(particlesMesh);

        // Linhas conectando partículas (Rede Neural)
        const linesMaterial = new THREE.LineBasicMaterial({ color: 0x112240, transparent: true, opacity: 0.15 });
        const linesGeometry = new THREE.BufferGeometry();
        const linesPositions = [];
        for(let i = 0; i < 200; i++) {
            const x1 = (Math.random() - 0.5) * 25; const y1 = (Math.random() - 0.5) * 25; const z1 = (Math.random() - 0.5) * 25;
            const x2 = x1 + (Math.random() - 0.5) * 4; const y2 = y1 + (Math.random() - 0.5) * 4; const z2 = z1 + (Math.random() - 0.5) * 4;
            linesPositions.push(x1, y1, z1); linesPositions.push(x2, y2, z2);
        }
        linesGeometry.setAttribute('position', new THREE.Float32BufferAttribute(linesPositions, 3));
        const linesMesh = new THREE.LineSegments(linesGeometry, linesMaterial);
        scene.add(linesMesh);

        camera.position.z = 8;
        camera.position.y = 1;

        let mouseX = 0; let mouseY = 0;
        document.addEventListener('mousemove', (event) => {
            mouseX = (event.clientX / window.innerWidth) - 0.5;
            mouseY = (event.clientY / window.innerHeight) - 0.5;
        });

        const clock = new THREE.Clock();

        function animate() {
            requestAnimationFrame(animate);
            const elapsedTime = clock.getElapsedTime();

            // Animar Ondas Sonoras
            waveGroup.children.forEach((wave, index) => {
                const positions = wave.geometry.attributes.position.array;
                const basePoints = wave.userData.basePoints;
                const speed = wave.userData.speed;
                const amplitude = wave.userData.amplitude;

                for (let i = 0; i < basePoints.length; i++) {
                    const base = basePoints[i];
                    const x = base.x;
                    // Modulação da onda (simula áudio)
                    const y = Math.sin(elapsedTime * speed + x * 0.5) * amplitude * Math.sin(elapsedTime * 0.5 + index);
                    positions[i * 3 + 1] = y; // Atualiza apenas o Y
                }
                wave.geometry.attributes.position.needsUpdate = true;
            });

            // Rotação suave da rede neural
            particlesMesh.rotation.y = elapsedTime * 0.02;
            linesMesh.rotation.y = elapsedTime * 0.02;

            // Interação com o mouse (Parallax)
            camera.position.x += (mouseX * 1.5 - camera.position.x) * 0.05;
            camera.position.y += (-mouseY * 1.5 - camera.position.y) * 0.05;
            camera.lookAt(scene.position);

            renderer.render(scene, camera);
        }
        animate();

        window.addEventListener('resize', () => {
            camera.aspect = window.innerWidth / window.innerHeight;
            camera.updateProjectionMatrix();
            renderer.setSize(window.innerWidth, window.innerHeight);
        });
    </script>
</body>
</html>
