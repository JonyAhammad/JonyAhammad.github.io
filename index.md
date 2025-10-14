<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jony Ahammad - Digital Portfolio</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Configure Tailwind with the soft dark mode palette -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        'primary-bg': '#1a202c', // Dark Slate/Charcoal - Soft Background
                        'secondary-bg': '#2d3748', // Lighter Slate - Card Background
                        'accent': '#4dc0b5', // Soft Teal/Cyan - Soothing Accent Color
                        'text-light': '#f7fafc', // Off-white
                        'text-muted': '#a0aec0', // Soft Gray
                    }
                }
            }
        }
    </script>
    <style>
        /* Base styles */
        html {
            scroll-behavior: smooth;
        }
        body {
            background-color: theme('colors.primary-bg');
            color: theme('colors.text-light');
            font-family: theme('fontFamily.sans');
            min-height: 100vh;
        }
        /* Navigation Hover Effect */
        .nav-link {
            transition: color 0.3s, background-color 0.3s;
        }
        .nav-link:hover {
            color: theme('colors.accent');
            background-color: theme('colors.secondary-bg');
        }
        /* General Card Styling with Soft Shadow */
        .content-card {
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.3), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            transition: all 0.3s ease;
        }
        .content-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 20px -5px rgba(77, 192, 181, 0.2), 0 6px 8px -3px rgba(0, 0, 0, 0.1);
        }
        /* Profile Image Placeholder Styling */
        .profile-pic-placeholder {
            width: 120px;
            height: 120px;
            background-color: theme('colors.secondary-bg');
            border: 4px solid theme('colors.accent');
        }
    </style>
    <!-- Lucide Icons for aesthetic enhancement -->
    <script type="module" src="https://unpkg.com/lucide@latest"></script>
</head>
<body class="antialiased">

    <!-- Header & Navigation -->
    <header class="bg-secondary-bg/90 backdrop-blur-sm shadow-2xl sticky top-0 z-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <!-- Site Title / Logo -->
            <div class="text-2xl font-extrabold text-text-light tracking-wide">
                <span class="text-accent">Jony</span>Ahammad
            </div>

            <!-- Navigation Links -->
            <nav class="hidden md:flex space-x-6">
                <!-- Links now point to sections within this single file -->
                <a href="#about" class="nav-link px-3 py-2 rounded-lg font-semibold text-text-light">About Me</a>
                <a href="#skills" class="nav-link px-3 py-2 rounded-lg font-semibold text-text-light">Skills</a>
                <a href="#projects" class="nav-link px-3 py-2 rounded-lg font-semibold text-text-light">Projects</a>
                <a href="#interests" class="nav-link px-3 py-2 rounded-lg font-semibold text-text-light">Interests</a>
            </nav>

            <!-- Mobile Menu Placeholder -->
            <button class="md:hidden text-text-light focus:outline-none">
                 <i data-lucide="menu" class="w-6 h-6"></i>
            </button>
        </div>
    </header>

    <!-- Main Content Area -->
    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">

        <!-- 1. About Me Section (Content Integrated from About Me.md) -->
        <section id="about" class="text-center mb-20 pt-8 flex flex-col items-center">
            <div class="profile-pic-placeholder rounded-full flex items-center justify-center mb-6 text-2xl font-bold text-accent">J.A.</div>
            <h1 class="text-5xl md:text-6xl font-extrabold mb-4 leading-tight text-accent">
                Jony Ahammad: Digital Architect
            </h1>
            <p class="text-xl md:text-2xl text-text-muted max-w-4xl mx-auto mb-10">
                Welcome to my digital workshop. I am a dedicated developer focused on the intersection of **clean code, robust security, and user-centric web design**.
            </p>
            
            <div class="content-card bg-secondary-bg p-8 rounded-xl max-w-5xl text-left">
                <h2 class="text-3xl font-bold mb-4 flex items-center"><i data-lucide="user-square" class="w-6 h-6 mr-3 text-accent"></i> My Core Philosophy: Continuous Mastery</h2>
                <p class="text-text-light leading-relaxed mb-4">
                    My professional journey is centered on **continu
