<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>القافلة الطبية - كلية الصيدلة جامعة عين شمس</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/@fontsource/cairo@4.5.0/index.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/@fontsource/poppins@4.5.0/index.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #1e40af;
            --primary-light: #3b82f6;
            --primary-dark: #1e3a8a;
            --secondary: #059669;
            --secondary-light: #10b981;
            --accent: #f59e0b;
            --accent-light: #fbbf24;
            --bg-light: #f8fafc;
            --text-dark: #1e293b;
            --text-light: #64748b;
            --card-shadow: 0 10px 40px rgba(0, 0, 0, 0.1);
            --card-hover: 0 20px 60px rgba(0, 0, 0, 0.15);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
            font-size: 16px;
        }

        @media (max-width: 768px) {
            html {
                font-size: 14px;
            }
        }

        body {
            font-family: 'Cairo', 'Poppins', sans-serif;
            background: var(--bg-light);
            color: var(--text-dark);
            overflow-x: hidden;
        }

        body.en {
            font-family: 'Poppins', 'Cairo', sans-serif;
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }

        ::-webkit-scrollbar-thumb {
            background: var(--primary);
            border-radius: 5px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: var(--primary-light);
        }

        /* Gradient Backgrounds */
        .gradient-primary {
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
        }

        .gradient-secondary {
            background: linear-gradient(135deg, var(--secondary) 0%, var(--secondary-light) 100%);
        }

        .gradient-accent {
            background: linear-gradient(135deg, var(--accent) 0%, var(--accent-light) 100%);
        }

        .gradient-sponsor {
            background: linear-gradient(135deg, #ec4899 0%, #f472b6 100%);
        }

        /* Cards */
        .card {
            background: white;
            border-radius: 16px;
            box-shadow: var(--card-shadow);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            overflow: hidden;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: var(--card-hover);
        }

        /* Buttons */
        .btn {
            padding: 12px 24px;
            border-radius: 50px;
            font-weight: 700;
            transition: all 0.3s ease;
            cursor: pointer;
            border: none;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            text-decoration: none;
            font-size: 0.95rem;
        }

        @media (max-width: 768px) {
            .btn {
                padding: 10px 20px;
                font-size: 0.85rem;
            }
        }

        .btn-primary {
            background: var(--primary);
            color: white;
            box-shadow: 0 4px 15px rgba(30, 64, 175, 0.4);
        }

        .btn-primary:hover {
            background: var(--primary-light);
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(30, 64, 175, 0.5);
        }

        .btn-secondary {
            background: white;
            color: var(--primary);
            border: 2px solid var(--primary);
        }

        .btn-secondary:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-3px);
        }

        .btn-gold {
            background: linear-gradient(135deg, var(--accent) 0%, var(--accent-light) 100%);
            color: white;
            box-shadow: 0 4px 15px rgba(245, 158, 11, 0.4);
        }

        .btn-gold:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(245, 158, 11, 0.5);
        }

        /* Sections */
        .section {
            padding: 60px 16px;
        }

        @media (min-width: 768px) {
            .section {
                padding: 80px 20px;
            }
        }

        @media (min-width: 1024px) {
            .section {
                padding: 100px 20px;
            }
        }

        .section-title {
            font-size: 2rem;
            font-weight: 800;
            text-align: center;
            margin-bottom: 16px;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            position: relative;
            display: inline-block;
            width: 100%;
        }

        @media (min-width: 768px) {
            .section-title {
                font-size: 2.5rem;
            }
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -12px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            border-radius: 2px;
        }

        .section-subtitle {
            text-align: center;
            color: var(--text-light);
            font-size: 1rem;
            max-width: 600px;
            margin: 0 auto 40px;
            line-height: 1.8;
        }

        @media (min-width: 768px) {
            .section-subtitle {
                font-size: 1.2rem;
                margin-bottom: 60px;
            }
        }

        /* Committee Grid */
        .committee-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            max-width: 1400px;
            margin: 0 auto;
        }

        @media (min-width: 640px) {
            .committee-grid {
                grid-template-columns: repeat(2, 1fr);
                gap: 25px;
            }
        }

        @media (min-width: 1024px) {
            .committee-grid {
                grid-template-columns: repeat(3, 1fr);
                gap: 35px;
            }
        }

        @media (min-width: 1280px) {
            .committee-grid {
                grid-template-columns: repeat(4, 1fr);
            }
        }

        .committee-card {
            background: white;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: var(--card-shadow);
            transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
            cursor: pointer;
            position: relative;
        }

        .committee-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--secondary), var(--accent));
            transform: scaleX(0);
            transition: transform 0.5s ease;
        }

        .committee-card:hover::before {
            transform: scaleX(1);
        }

        .committee-card:hover {
            transform: translateY(-8px) scale(1.02);
            box-shadow: var(--card-hover);
        }

        .committee-card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        @media (min-width: 768px) {
            .committee-card img {
                height: 220px;
            }
        }

        .committee-card:hover img {
            transform: scale(1.05);
        }

        .committee-card-content {
            padding: 20px;
        }

        @media (min-width: 768px) {
            .committee-card-content {
                padding: 30px;
            }
        }

        .committee-card-icon {
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            border-radius: 14px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 16px;
            font-size: 1.3rem;
            color: white;
            box-shadow: 0 4px 15px rgba(30, 64, 175, 0.3);
        }

        @media (min-width: 768px) {
            .committee-card-icon {
                width: 60px;
                height: 60px;
                font-size: 1.5rem;
            }
        }

        .committee-card h3 {
            font-size: 1.2rem;
            color: var(--primary);
            margin-bottom: 10px;
            font-weight: 700;
        }

        @media (min-width: 768px) {
            .committee-card h3 {
                font-size: 1.5rem;
            }
        }

        .committee-card p {
            color: var(--text-light);
            line-height: 1.6;
            font-size: 0.85rem;
        }

        @media (min-width: 768px) {
            .committee-card p {
                font-size: 0.95rem;
            }
        }

        .committee-card-badge {
            display: inline-block;
            background: linear-gradient(135deg, var(--secondary) 0%, var(--secondary-light) 100%);
            color: white;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.7rem;
            font-weight: 600;
            margin-top: 12px;
        }

        /* Timeline */
        .timeline-container {
            max-width: 100%;
            margin: 0 auto;
            position: relative;
            padding: 20px 0;
        }

        @media (min-width: 768px) {
            .timeline-container {
                max-width: 1200px;
                padding: 40px 0;
            }
        }

        .timeline-container::before {
            content: '';
            position: absolute;
            left: 24px;
            transform: translateX(-50%);
            width: 4px;
            height: 100%;
            background: linear-gradient(to bottom, var(--primary), var(--secondary), var(--accent));
            border-radius: 3px;
            box-shadow: 0 0 20px rgba(30, 64, 175, 0.3);
        }

        @media (min-width: 768px) {
            .timeline-container::before {
                left: 50%;
                width: 6px;
            }
        }

        .timeline-item {
            display: flex;
            justify-content: flex-start;
            padding: 20px 20px 20px 60px;
            position: relative;
            width: 100%;
            opacity: 0;
            transform: translateX(-30px);
            transition: all 0.6s ease;
        }

        @media (min-width: 768px) {
            .timeline-item {
                width: 50%;
                padding: 30px 50px;
                transform: translateX(-50px);
            }

            .timeline-item:nth-child(even) {
                justify-content: flex-start;
                margin-left: 50%;
                transform: translateX(50px);
            }

            .timeline-item:nth-child(even).visible {
                transform: translateX(0);
            }
        }

        .timeline-item.visible {
            opacity: 1;
            transform: translateX(0);
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            width: 20px;
            height: 20px;
            background: white;
            border: 4px solid var(--primary);
            border-radius: 50%;
            top: 30px;
            left: 14px;
            box-shadow: 0 0 0 6px rgba(30, 64, 175, 0.2), 0 4px 10px rgba(0, 0, 0, 0.2);
            z-index: 2;
            transition: all 0.3s ease;
        }

        @media (min-width: 768px) {
            .timeline-item::before {
                width: 24px;
                height: 24px;
                top: 40px;
                left: auto;
                right: -12px;
            }

            .timeline-item:nth-child(even)::before {
                left: -12px;
                right: auto;
            }
        }

        .timeline-item:hover::before {
            background: var(--primary);
            box-shadow: 0 0 0 8px rgba(30, 64, 175, 0.4), 0 4px 15px rgba(0, 0, 0, 0.3);
        }

        .timeline-content {
            background: white;
            padding: 20px;
            border-radius: 16px;
            box-shadow: var(--card-shadow);
            width: 100%;
            position: relative;
            transition: all 0.3s ease;
            border: 1px solid rgba(30, 64, 175, 0.1);
        }

        @media (min-width: 768px) {
            .timeline-content {
                padding: 35px;
                max-width: 500px;
            }
        }

        .timeline-content:hover {
            transform: scale(1.01);
            box-shadow: var(--card-hover);
        }

        .timeline-year-badge {
            display: inline-block;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            color: white;
            padding: 6px 16px;
            border-radius: 30px;
            font-size: 0.95rem;
            font-weight: 700;
            margin-bottom: 12px;
            box-shadow: 0 4px 15px rgba(30, 64, 175, 0.3);
        }

        @media (min-width: 768px) {
            .timeline-year-badge {
                font-size: 1.1rem;
                padding: 8px 20px;
            }
        }

        .timeline-title {
            font-size: 1.1rem;
            font-weight: 700;
            color: var(--text-dark);
            margin-bottom: 12px;
            line-height: 1.4;
        }

        @media (min-width: 768px) {
            .timeline-title {
                font-size: 1.4rem;
            }
        }

        .timeline-location {
            display: flex;
            align-items: center;
            gap: 6px;
            color: var(--secondary);
            font-weight: 600;
            margin-bottom: 12px;
            font-size: 0.85rem;
        }

        @media (min-width: 768px) {
            .timeline-location {
                font-size: 0.95rem;
            }
        }

        .timeline-location i {
            font-size: 0.9rem;
        }

        .timeline-text {
            color: var(--text-light);
            line-height: 1.8;
            font-size: 0.85rem;
            margin-bottom: 16px;
        }

        @media (min-width: 768px) {
            .timeline-text {
                font-size: 0.95rem;
            }
        }

        .timeline-stats {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
            margin-top: 16px;
            padding-top: 16px;
            border-top: 2px dashed rgba(30, 64, 175, 0.1);
        }

        @media (min-width: 768px) {
            .timeline-stats {
                grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
                gap: 12px;
            }
        }

        .timeline-stat {
            background: linear-gradient(135deg, rgba(30, 64, 175, 0.05) 0%, rgba(59, 130, 246, 0.05) 100%);
            padding: 12px 10px;
            border-radius: 10px;
            text-align: center;
            border: 1px solid rgba(30, 64, 175, 0.1);
        }

        .timeline-stat-number {
            font-size: 1.2rem;
            font-weight: 800;
            color: var(--primary);
            display: block;
            margin-bottom: 4px;
        }

        @media (min-width: 768px) {
            .timeline-stat-number {
                font-size: 1.4rem;
            }
        }

        .timeline-stat-label {
            font-size: 0.7rem;
            color: var(--text-light);
            font-weight: 500;
        }

        @media (min-width: 768px) {
            .timeline-stat-label {
                font-size: 0.8rem;
            }
        }

        .timeline-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
            margin-top: 12px;
        }

        .timeline-tag {
            background: linear-gradient(135deg, var(--secondary) 0%, var(--secondary-light) 100%);
            color: white;
            padding: 4px 10px;
            border-radius: 15px;
            font-size: 0.7rem;
            font-weight: 600;
        }

        .timeline-tag.accent {
            background: linear-gradient(135deg, var(--accent) 0%, var(--accent-light) 100%);
        }

        .timeline-tag.purple {
            background: linear-gradient(135deg, #8b5cf6 0%, #a78bfa 100%);
        }

        .timeline-tag.sponsor {
            background: linear-gradient(135deg, #ec4899 0%, #f472b6 100%);
        }

        /* Sponsor Badge */
        .sponsor-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: linear-gradient(135deg, #ec4899 0%, #f472b6 100%);
            color: white;
            padding: 6px 16px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 700;
            margin-top: 12px;
            box-shadow: 0 4px 15px rgba(236, 72, 153, 0.4);
        }

        .sponsor-badge i {
            font-size: 0.9rem;
        }

        /* Stats Section */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            max-width: 100%;
            margin: 0 auto;
        }

        @media (min-width: 640px) {
            .stats-grid {
                grid-template-columns: repeat(4, 1fr);
                gap: 25px;
            }
        }

        .stat-card {
            background: white;
            padding: 20px 15px;
            border-radius: 16px;
            text-align: center;
            box-shadow: var(--card-shadow);
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
        }

        @media (min-width: 768px) {
            .stat-card {
                padding: 35px 25px;
            }
        }

        .stat-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--secondary), var(--accent));
        }

        .stat-card:hover {
            transform: translateY(-5px);
            box-shadow: var(--card-hover);
        }

        .stat-icon {
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 15px;
            font-size: 1.3rem;
            color: white;
            box-shadow: 0 4px 20px rgba(30, 64, 175, 0.3);
        }

        @media (min-width: 768px) {
            .stat-icon {
                width: 70px;
                height: 70px;
                font-size: 1.8rem;
            }
        }

        .stat-number {
            font-size: 1.8rem;
            font-weight: 800;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            display: block;
            margin-bottom: 6px;
        }

        @media (min-width: 768px) {
            .stat-number {
                font-size: 2.5rem;
            }
        }

        .stat-label {
            font-size: 0.8rem;
            color: var(--text-light);
            font-weight: 600;
        }

        @media (min-width: 768px) {
            .stat-label {
                font-size: 1rem;
            }
        }

        /* Vision Cards */
        .vision-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 25px;
            max-width: 100%;
            margin: 0 auto;
        }

        @media (min-width: 768px) {
            .vision-grid {
                grid-template-columns: repeat(3, 1fr);
                gap: 40px;
            }
        }

        .vision-card {
            text-align: center;
            padding: 30px 20px;
            background: white;
            border-radius: 20px;
            box-shadow: var(--card-shadow);
            transition: all 0.4s ease;
            position: relative;
        }

        @media (min-width: 768px) {
            .vision-card {
                padding: 45px 35px;
            }
        }

        .vision-card:hover {
            transform: translateY(-8px);
            box-shadow: var(--card-hover);
        }

        .vision-icon {
            width: 70px;
            height: 70px;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            font-size: 1.8rem;
            color: white;
            box-shadow: 0 8px 30px rgba(30, 64, 175, 0.3);
            position: relative;
        }

        @media (min-width: 768px) {
            .vision-icon {
                width: 90px;
                height: 90px;
                font-size: 2.2rem;
            }
        }

        .vision-icon::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            border-radius: 50%;
            background: inherit;
            opacity: 0.3;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 0.3; }
            50% { transform: scale(1.1); opacity: 0.1; }
        }

        .vision-card h3 {
            font-size: 1.3rem;
            color: var(--primary);
            margin-bottom: 15px;
            font-weight: 700;
        }

        @media (min-width: 768px) {
            .vision-card h3 {
                font-size: 1.6rem;
            }
        }

        .vision-card p {
            color: var(--text-light);
            line-height: 1.8;
            font-size: 0.9rem;
        }

        @media (min-width: 768px) {
            .vision-card p {
                font-size: 1rem;
                line-height: 2;
            }
        }

        /* Full Page Modal */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            backdrop-filter: blur(5px);
            z-index: 1000;
            overflow-y: auto;
            padding: 20px 12px;
        }

        .modal.active {
            display: flex;
            justify-content: center;
            align-items: flex-start;
        }

        .modal-content {
            background: white;
            border-radius: 20px;
            max-width: 100%;
            width: 100%;
            max-height: 95vh;
            overflow-y: auto;
            position: relative;
            animation: modalSlide 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: 0 25px 80px rgba(0, 0, 0, 0.3);
        }

        @media (min-width: 768px) {
            .modal-content {
                max-width: 1100px;
            }
        }

        @keyframes modalSlide {
            from {
                opacity: 0;
                transform: translateY(-60px) scale(0.9);
            }
            to {
                opacity: 1;
                transform: translateY(0) scale(1);
            }
        }

        .modal-close {
            position: absolute;
            top: 15px;
            left: 15px;
            width: 45px;
            height: 45px;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 50%;
            cursor: pointer;
            font-size: 1.2rem;
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 10;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(30, 64, 175, 0.4);
        }

        @media (min-width: 768px) {
            .modal-close {
                top: 20px;
                left: 20px;
                width: 50px;
                height: 50px;
                font-size: 1.4rem;
            }
        }

        .modal-close:hover {
            background: var(--primary-light);
            transform: rotate(90deg) scale(1.1);
        }

        .modal-header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            color: white;
            padding: 40px 25px;
            border-radius: 20px 20px 0 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        @media (min-width: 768px) {
            .modal-header {
                padding: 60px 40px;
            }
        }

        .modal-header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            animation: rotate 20s linear infinite;
        }

        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .modal-header img {
            width: 100%;
            max-height: 300px;
            object-fit: cover;
            border-radius: 12px;
            margin-bottom: 25px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
            position: relative;
            z-index: 1;
        }

        @media (min-width: 768px) {
            .modal-header img {
                max-height: 400px;
            }
        }

        .modal-header h2 {
            font-size: 1.8rem;
            margin-bottom: 10px;
            position: relative;
            z-index: 1;
        }

        @media (min-width: 768px) {
            .modal-header h2 {
                font-size: 2.5rem;
            }
        }

        .modal-header p {
            opacity: 0.9;
            font-size: 1rem;
            position: relative;
            z-index: 1;
        }

        @media (min-width: 768px) {
            .modal-header p {
                font-size: 1.2rem;
            }
        }

        .modal-body {
            padding: 30px 20px;
        }

        @media (min-width: 768px) {
            .modal-body {
                padding: 50px;
            }
        }

        .modal-section {
            margin-bottom: 35px;
            padding-bottom: 25px;
            border-bottom: 2px dashed rgba(30, 64, 175, 0.1);
        }

        .modal-section:last-child {
            border-bottom: none;
        }

        .modal-section h3 {
            font-size: 1.4rem;
            color: var(--primary);
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 12px;
            font-weight: 700;
        }

        @media (min-width: 768px) {
            .modal-section h3 {
                font-size: 1.6rem;
            }
        }

        .modal-section h3 i {
            width: 40px;
            height: 40px;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1rem;
            color: white;
        }

        .modal-section p, .modal-section li {
            color: var(--text-light);
            line-height: 2;
            margin-bottom: 12px;
            font-size: 0.95rem;
        }

        @media (min-width: 768px) {
            .modal-section p, .modal-section li {
                font-size: 1.05rem;
            }
        }

        .modal-section ul {
            padding-right: 25px;
        }

        body.en .modal-section ul {
            padding-right: 0;
            padding-left: 25px;
        }

        .detail-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            margin: 20px 0;
        }

        @media (min-width: 768px) {
            .detail-grid {
                grid-template-columns: repeat(3, 1fr);
                gap: 20px;
            }
        }

        .detail-card {
            background: linear-gradient(135deg, rgba(30, 64, 175, 0.05) 0%, rgba(59, 130, 246, 0.05) 100%);
            padding: 20px;
            border-radius: 16px;
            border-right: 4px solid var(--primary);
            transition: all 0.3s ease;
        }

        body.en .detail-card {
            border-right: none;
            border-left: 4px solid var(--primary);
        }

        .detail-card:hover {
            background: linear-gradient(135deg, rgba(30, 64, 175, 0.1) 0%, rgba(59, 130, 246, 0.1) 100%);
            transform: translateY(-3px);
        }

        .detail-card i {
            font-size: 1.5rem;
            color: var(--primary);
            margin-bottom: 12px;
            display: block;
        }

        .detail-card h5 {
            color: var(--text-dark);
            font-size: 0.95rem;
            font-weight: 600;
        }

        @media (min-width: 768px) {
            .detail-card h5 {
                font-size: 1rem;
            }
        }

        .impact-badges {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin: 20px 0;
        }

        .impact-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: linear-gradient(135deg, var(--secondary) 0%, var(--secondary-light) 100%);
            color: white;
            padding: 8px 18px;
            border-radius: 25px;
            font-size: 0.85rem;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(5, 150, 105, 0.3);
        }

        @media (min-width: 768px) {
            .impact-badge {
                font-size: 0.95rem;
                padding: 10px 22px;
            }
        }

        .impact-badge i {
            font-size: 0.9rem;
        }

        .impact-badge.accent {
            background: linear-gradient(135deg, var(--accent) 0%, var(--accent-light) 100%);
            box-shadow: 0 4px 15px rgba(245, 158, 11, 0.3);
        }

        .impact-badge.purple {
            background: linear-gradient(135deg, #8b5cf6 0%, #a78bfa 100%);
            box-shadow: 0 4px 15px rgba(139, 92, 246, 0.3);
        }

        .timeline-evolution {
            background: linear-gradient(135deg, rgba(30, 64, 175, 0.05) 0%, rgba(59, 130, 246, 0.05) 100%);
            padding: 25px;
            border-radius: 16px;
            margin: 25px 0;
        }

        .timeline-evolution h4 {
            color: var(--primary);
            font-size: 1.2rem;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .timeline-evolution ul {
            padding-right: 20px;
        }

        body.en .timeline-evolution ul {
            padding-right: 0;
            padding-left: 20px;
        }

        /* Language Switcher */
        .lang-switch {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            z-index: 999;
            width: 90%;
            max-width: 200px;
        }

        @media (min-width: 768px) {
            .lang-switch {
                bottom: auto;
                top: 20px;
                left: auto;
                right: 20px;
                transform: none;
                width: auto;
            }
        }

        .lang-btn {
            background: white;
            border: 2px solid var(--primary);
            color: var(--primary);
            padding: 10px 20px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 700;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            box-shadow: 0 4px 15px rgba(30, 64, 175, 0.2);
            width: 100%;
            font-size: 0.9rem;
        }

        @media (min-width: 768px) {
            .lang-btn {
                padding: 12px 24px;
            }
        }

        .lang-btn:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(30, 64, 175, 0.3);
        }

        .lang-btn i {
            animation: rotateGlobe 3s linear infinite;
        }

        @keyframes rotateGlobe {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        /* Navigation */
        .nav {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(10px);
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
            z-index: 998;
            padding: 14px 0;
            transition: all 0.3s ease;
        }

        @media (min-width: 768px) {
            .nav {
                padding: 18px 0;
            }
        }

        .nav.scrolled {
            padding: 10px 0;
            background: rgba(255, 255, 255, 0.99);
        }

        .nav-content {
            max-width: 1400px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 16px;
        }

        @media (min-width: 768px) {
            .nav-content {
                padding: 0 25px;
            }
        }

        .nav-logo {
            font-size: 1.3rem;
            font-weight: 800;
            color: var(--primary);
            display: flex;
            align-items: center;
            gap: 8px;
            text-decoration: none;
        }

        @media (min-width: 768px) {
            .nav-logo {
                font-size: 1.6rem;
                gap: 12px;
            }
        }

        .nav-logo i {
            font-size: 1.5rem;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        @media (min-width: 768px) {
            .nav-logo i {
                font-size: 1.8rem;
            }
        }

        .nav-links {
            display: none;
            gap: 25px;
            list-style: none;
        }

        @media (min-width: 768px) {
            .nav-links {
                display: flex;
                gap: 35px;
            }
        }

        .nav-links a {
            color: var(--text-dark);
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            position: relative;
            padding: 8px 0;
            font-size: 0.9rem;
        }

        @media (min-width: 768px) {
            .nav-links a {
                font-size: 1rem;
            }
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 3px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            border-radius: 2px;
            transition: width 0.3s ease;
        }

        .nav-links a:hover {
            color: var(--primary);
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        /* Hero */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, rgba(30, 64, 175, 0.92) 0%, rgba(59, 130, 246, 0.85) 100%),
                        url('https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/1e3936c0a-a22a-4175-93a1-7ecb57e66ea6.png');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            padding: 100px 16px 60px;
            position: relative;
            overflow: hidden;
        }

        @media (min-width: 768px) {
            .hero {
                padding: 120px 20px 80px;
            }
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: radial-gradient(circle at 50% 50%, transparent 0%, rgba(0,0,0,0.3) 100%);
        }

        .hero-content {
            text-align: center;
            color: white;
            max-width: 100%;
            position: relative;
            z-index: 1;
        }

        @media (min-width: 768px) {
            .hero-content {
                max-width: 1000px;
            }
        }

        .charity-badge {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: linear-gradient(135deg, var(--accent) 0%, var(--accent-light) 100%);
            padding: 12px 30px;
            border-radius: 50px;
            font-size: 0.95rem;
            font-weight: 700;
            margin-bottom: 20px;
            border: 2px solid rgba(255, 255, 255, 0.4);
            color: white;
            box-shadow: 0 4px 20px rgba(245, 158, 11, 0.4);
        }

        @media (min-width: 768px) {
            .charity-badge {
                padding: 14px 35px;
                font-size: 1.05rem;
            }
        }

        .charity-badge i {
            color: white;
            animation: heartbeat 1.5s ease-in-out infinite;
        }

        @keyframes heartbeat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.2); }
        }

        .hero-title {
            font-size: 2rem;
            font-weight: 800;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
            line-height: 1.3;
        }

        @media (min-width: 640px) {
            .hero-title {
                font-size: 2.8rem;
            }
        }

        @media (min-width: 1024px) {
            .hero-title {
                font-size: 3.8rem;
            }
        }

        .hero-subtitle {
            font-size: 1rem;
            margin-bottom: 30px;
            line-height: 1.8;
            opacity: 0.95;
            max-width: 100%;
            margin-left: auto;
            margin-right: auto;
        }

        @media (min-width: 640px) {
            .hero-subtitle {
                font-size: 1.2rem;
                max-width: 800px;
            }
        }

        @media (min-width: 1024px) {
            .hero-subtitle {
                font-size: 1.35rem;
            }
        }

        .hero-buttons {
            display: flex;
            gap: 12px;
            justify-content: center;
            flex-wrap: wrap;
        }

        @media (min-width: 640px) {
            .hero-buttons {
                gap: 20px;
            }
        }

        .hero-stats {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
            margin-top: 40px;
        }

        @media (min-width: 640px) {
            .hero-stats {
                display: flex;
                justify-content: center;
                gap: 40px;
            }
        }

        .hero-stat {
            text-align: center;
        }

        .hero-stat-number {
            font-size: 1.8rem;
            font-weight: 800;
            display: block;
            margin-bottom: 4px;
        }

        @media (min-width: 640px) {
            .hero-stat-number {
                font-size: 2.5rem;
            }
        }

        .hero-stat-label {
            font-size: 0.8rem;
            opacity: 0.9;
        }

        @media (min-width: 640px) {
            .hero-stat-label {
                font-size: 0.95rem;
            }
        }

        /* Footer */
        .footer {
            background: linear-gradient(135deg, var(--text-dark) 0%, #0f172a 100%);
            color: white;
            padding: 50px 16px 25px;
            position: relative;
        }

        @media (min-width: 768px) {
            .footer {
                padding: 80px 20px 30px;
            }
        }

        .footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--secondary), var(--accent));
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
        }

        @media (min-width: 768px) {
            .footer-content {
                grid-template-columns: repeat(3, 1fr);
                gap: 50px;
            }
        }

        .footer-section h4 {
            font-size: 1.2rem;
            margin-bottom: 20px;
            color: var(--primary-light);
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        @media (min-width: 768px) {
            .footer-section h4 {
                font-size: 1.4rem;
            }
        }

        .footer-section h4 i {
            width: 32px;
            height: 32px;
            background: rgba(59, 130, 246, 0.2);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        @media (min-width: 768px) {
            .footer-section h4 i {
                width: 35px;
                height: 35px;
            }
        }

        .footer-section p, .footer-section a {
            color: rgba(255, 255, 255, 0.8);
            line-height: 1.8;
            text-decoration: none;
            display: block;
            margin-bottom: 10px;
            transition: all 0.3s ease;
            font-size: 0.9rem;
        }

        @media (min-width: 768px) {
            .footer-section p, .footer-section a {
                font-size: 1rem;
            }
        }

        .footer-section a:hover {
            color: var(--primary-light);
            padding-right: 5px;
        }

        body.en .footer-section a:hover {
            padding-right: 0;
            padding-left: 5px;
        }

        .footer-social {
            display: flex;
            gap: 15px;
            margin-top: 20px;
            flex-wrap: wrap;
        }

        .footer-social a {
            width: 50px;
            height: 50px;
            background: rgba(59, 130, 246, 0.2);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.3rem;
            transition: all 0.3s ease;
            text-decoration: none;
        }

        @media (min-width: 768px) {
            .footer-social a {
                width: 55px;
                height: 55px;
                font-size: 1.4rem;
            }
        }

        .footer-social a:hover {
            transform: translateY(-5px) scale(1.1);
        }

        .footer-social a.linkedin:hover {
            background: linear-gradient(135deg, #0077b5 0%, #00a0dc 100%);
        }

        .footer-social a.facebook:hover {
            background: linear-gradient(135deg, #1877f2 0%, #4267b2 100%);
        }

        .footer-social a.instagram:hover {
            background: linear-gradient(135deg, #f09433 0%, #e6683c 25%, #dc2743 50%, #cc2366 75%, #bc1888 100%);
        }

        .footer-social a.email:hover {
            background: linear-gradient(135deg, #ea4335 0%, #fbbc05 100%);
        }

        .footer-bottom {
            text-align: center;
            padding-top: 30px;
            margin-top: 40px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: rgba(255, 255, 255, 0.6);
            font-size: 0.85rem;
        }

        @media (min-width: 768px) {
            .footer-bottom {
                font-size: 1rem;
            }
        }

        /* Mobile Menu */
        .mobile-menu {
            display: block;
            font-size: 1.3rem;
            color: var(--primary);
            cursor: pointer;
            padding: 8px;
        }

        @media (min-width: 768px) {
            .mobile-menu {
                display: none;
            }
        }

        /* Mobile Navigation */
        .mobile-nav {
            display: none;
            position: fixed;
            top: 60px;
            left: 0;
            right: 0;
            background: white;
            padding: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            z-index: 997;
        }

        .mobile-nav.active {
            display: block;
            animation: slideDown 0.3s ease;
        }

        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .mobile-nav a {
            display: block;
            padding: 12px 16px;
            color: var(--text-dark);
            text-decoration: none;
            font-weight: 600;
            border-radius: 10px;
            transition: all 0.3s ease;
            font-size: 0.95rem;
        }

        .mobile-nav a:hover {
            background: var(--bg-light);
            color: var(--primary);
        }

        /* Animations */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Scroll to Top */
        .scroll-top {
            position: fixed;
            bottom: 80px;
            right: 20px;
            width: 50px;
            height: 50px;
            background: var(--primary);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
            z-index: 996;
            box-shadow: 0 4px 20px rgba(30, 64, 175, 0.4);
        }

        @media (min-width: 768px) {
            .scroll-top {
                bottom: 100px;
            }
        }

        .scroll-top.visible {
            opacity: 1;
            visibility: visible;
        }

        .scroll-top:hover {
            background: var(--primary-light);
            transform: translateY(-5px);
        }

        /* Sponsors Section */
        .sponsors-section {
            background: linear-gradient(135deg, rgba(236, 72, 153, 0.05) 0%, rgba(244, 114, 182, 0.05) 100%);
            padding: 60px 20px;
            text-align: center;
        }

        .sponsors-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 40px auto 0;
        }

        @media (min-width: 640px) {
            .sponsors-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (min-width: 1024px) {
            .sponsors-grid {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        .sponsor-card {
            background: white;
            padding: 35px 25px;
            border-radius: 20px;
            box-shadow: var(--card-shadow);
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
        }

        .sponsor-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 5px;
            background: linear-gradient(135deg, #ec4899 0%, #f472b6 100%);
        }

        .sponsor-card:hover {
            transform: translateY(-8px);
            box-shadow: var(--card-hover);
        }

        .sponsor-card-icon {
            width: 80px;
            height: 80px;
            background: linear-gradient(135deg, #ec4899 0%, #f472b6 100%);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 25px;
            font-size: 2rem;
            color: white;
            box-shadow: 0 8px 30px rgba(236, 72, 153, 0.4);
        }

        .sponsor-card h4 {
            color: var(--primary);
            font-size: 1.3rem;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .sponsor-card p {
            color: var(--text-light);
            font-size: 0.95rem;
            line-height: 1.8;
        }

        .sponsor-year {
            display: inline-block;
            background: linear-gradient(135deg, #ec4899 0%, #f472b6 100%);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-top: 15px;
        }

        .sponsors-title {
            text-align: center;
            margin-bottom: 20px;
        }

        .sponsors-title i {
            color: #ec4899;
            margin-left: 10px;
        }

        body.en .sponsors-title i {
            margin-left: 0;
            margin-right: 10px;
        }

        /* Contact Links */
        .contact-link {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 12px 25px;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            color: white;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            margin: 10px 5px;
            box-shadow: 0 4px 15px rgba(30, 64, 175, 0.3);
        }

        .contact-link:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(30, 64, 175, 0.4);
        }

        .contact-link.linkedin {
            background: linear-gradient(135deg, #0077b5 0%, #00a0dc 100%);
        }

        .contact-link.facebook {
            background: linear-gradient(135deg, #1877f2 0%, #4267b2 100%);
        }

        .contact-link.instagram {
            background: linear-gradient(135deg, #f09433 0%, #e6683c 25%, #dc2743 50%, #cc2366 75%, #bc1888 100%);
        }

        .contact-link.email {
            background: linear-gradient(135deg, #ea4335 0%, #fbbc05 100%);
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="nav" id="navbar">
        <div class="nav-content">
            <a href="#" class="nav-logo">
                <i class="fas fa-heartbeat"></i>
                <span data-ar="القافلة الطبية" data-en="Medical Caravan">القافلة الطبية</span>
            </a>
            <ul class="nav-links">
                <li><a href="#home" data-ar="الرئيسية" data-en="Home">الرئيسية</a></li>
                <li><a href="#about" data-ar="عن القافلة" data-en="About">عن القافلة</a></li>
                <li><a href="#sponsors" data-ar="الرعاة" data-en="Sponsors">الرعاة</a></li>
                <li><a href="#committees" data-ar="اللجان" data-en="Committees">اللجان</a></li>
                <li><a href="#history" data-en="History">التاريخ</a></li>
                <li><a href="#contact" data-ar="تواصل معنا" data-en="Contact">تواصل معنا</a></li>
            </ul>
            <div class="mobile-menu" onclick="toggleMobileNav()">
                <i class="fas fa-bars"></i>
            </div>
        </div>
    </nav>

    <!-- Mobile Navigation -->
    <div class="mobile-nav" id="mobileNav">
        <a href="#home" onclick="toggleMobileNav()" data-ar="الرئيسية" data-en="Home">الرئيسية</a>
        <a href="#about" onclick="toggleMobileNav()" data-ar="عن القافلة" data-en="About">عن القافلة</a>
        <a href="#sponsors" onclick="toggleMobileNav()" data-ar="الرعاة" data-en="Sponsors">الرعاة</a>
        <a href="#committees" onclick="toggleMobileNav()" data-ar="اللجان" data-en="Committees">اللجان</a>
        <a href="#history" onclick="toggleMobileNav()" data-ar="التاريخ" data-en="History">التاريخ</a>
        <a href="#contact" onclick="toggleMobileNav()" data-ar="تواصل معنا" data-en="Contact">تواصل معنا</a>
    </div>

    <!-- Language Switcher -->
    <div class="lang-switch">
        <button class="lang-btn" onclick="toggleLanguage()">
            <i class="fas fa-globe"></i>
            <span id="lang-text">English</span>
        </button>
    </div>

    <!-- Scroll to Top Button -->
    <div class="scroll-top" id="scrollTop" onclick="scrollToTop()">
        <i class="fas fa-arrow-up"></i>
    </div>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <div class="charity-badge">
                <i class="fas fa-heart"></i>
                <span data-ar="عمل خيري تطوعي" data-en="Volunteer Charity Work">عمل خيري تطوعي</span>
            </div>
            <h1 class="hero-title" data-ar="القافلة الطبية - كلية الصيدلة جامعة عين شمس" data-en="Medical Caravan - Ain Shams Faculty of Pharmacy">القافلة الطبية - كلية الصيدلة جامعة عين شمس</h1>
            <p class="hero-subtitle" data-ar="منذ عام 2005، نقدم خدمات صحية مجانية للمجتمعات المحرومة، نبني جيلاً من الصيادلة المتميزين القادرين على خدمة المجتمع" data-en="Since 2005, we provide free healthcare services to underserved communities, building a generation of outstanding pharmacists">منذ عام 2005، نقدم خدمات صحية مجانية للمجتمعات المحرومة، نبني جيلاً من الصيادلة المتميزين القادرين على خدمة المجتمع</p>
            <div class="hero-buttons">
                <a href="#committees" class="btn btn-primary">
                    <i class="fas fa-users"></i>
                    <span data-ar="استكشف اللجان" data-en="Explore Committees">استكشف اللجان</span>
                </a>
                <a href="#history" class="btn btn-gold">
                    <i class="fas fa-history"></i>
                    <span data-ar="تاريخ القافلة" data-en="Caravan History">تاريخ القافلة</span>
                </a>
            </div>
            <div class="hero-stats">
                <div class="hero-stat">
                    <span class="hero-stat-number" data-counter="20">0</span>
                    <span class="hero-stat-label" data-ar="سنة من العطاء" data-en="Years of Service">سنة من العطاء</span>
                </div>
                <div class="hero-stat">
                    <span class="hero-stat-number" data-counter="50000">0</span>
                    <span class="hero-stat-label" data-ar="مريض" data-en="Patients">مريض</span>
                </div>
                <div class="hero-stat">
                    <span class="hero-stat-number" data-counter="100000">0</span>
                    <span class="hero-stat-label" data-ar="تفاعل توعوي" data-en="Awareness">تفاعل توعوي</span>
                </div>
                <div class="hero-stat">
                    <span class="hero-stat-number" data-counter="6000">0</span>
                    <span class="hero-stat-label" data-ar="متطوع تدرب" data-en="Volunteers Trained">متطوع تدرب</span>
                </div>
            </div>
        </div>
    </section>

    <!-- About/Vision Section -->
    <section class="section vision-section" id="about" style="background: white;">
        <h2 class="section-title" data-ar="رؤيتنا ورسالتنا" data-en="Our Vision & Mission">رؤيتنا ورسالتنا</h2>
        <p class="section-subtitle" data-ar="نسعى لتحقيق التميز في خدمة المجتمع من خلال تقديم رعاية صحية متكاملة وتطوير مهارات طلابنا" data-en="We strive for excellence in community service through integrated healthcare and student development">نسعى لتحقيق التميز في خدمة المجتمع من خلال تقديم رعاية صحية متكاملة وتطوير مهارات طلابنا</p>
        
        <div class="vision-grid">
            <div class="vision-card fade-in">
                <div class="vision-icon">
                    <i class="fas fa-eye"></i>
                </div>
                <h3 data-ar="الرؤية" data-en="Vision">الرؤية</h3>
                <p data-ar="أن نكون النموذج الرائد في العمل الصحي التطوعي الطلابي، نقدم خدمات صحية مستدامة ومؤثرة للمجتمعات الأكثر احتياجاً" data-en="To be the leading model in student volunteer health work, providing sustainable and impactful healthcare services">أن نكون النموذج الرائد في العمل الصحي التطوعي الطلابي، نقدم خدمات صحية مستدامة ومؤثرة للمجتمعات الأكثر احتياجاً</p>
            </div>
            <div class="vision-card fade-in">
                <div class="vision-icon">
                    <i class="fas fa-bullseye"></i>
                </div>
                <h3 data-ar="الرسالة" data-en="Mission">الرسالة</h3>
                <p data-ar="تقديم خدمات صحية مجانية عالية الجودة، تطوير المهارات العملية للطلاب، ونشر الوعي الصحي في المجتمع" data-en="Provide high-quality free healthcare services, develop students' practical skills, and spread health awareness">تقديم خدمات صحية مجانية عالية الجودة، تطوير المهارات العملية للطلاب، ونشر الوعي الصحي في المجتمع</p>
            </div>
            <div class="vision-card fade-in">
                <div class="vision-icon">
                    <i class="fas fa-gem"></i>
                </div>
                <h3 data-ar="القيم" data-en="Values">القيم</h3>
                <p data-ar="التطوع، التميز، الاستدامة، العمل الجماعي، المسؤولية المجتمعية، والابتكار في خدمة الصحة العامة" data-en="Volunteering, Excellence, Sustainability, Teamwork, Social Responsibility, and Innovation">التطوع، التميز، الاستدامة، العمل الجماعي، المسؤولية المجتمعية، والابتكار في خدمة الصحة العامة</p>
            </div>
        </div>

        <!-- Stats -->
        <div class="stats-grid" style="margin-top: 60px;">
            <div class="stat-card fade-in">
                <div class="stat-icon">
                    <i class="fas fa-file-prescription"></i>
                </div>
                <span class="stat-number">50,000+</span>
                <span class="stat-label" data-ar="روشتة صرفت" data-en="Prescriptions Dispensed">روشتة صرفت</span>
            </div>
            <div class="stat-card fade-in">
                <div class="stat-icon">
                    <i class="fas fa-flask"></i>
                </div>
                <span class="stat-number">15,000+</span>
                <span class="stat-label" data-ar="تحليل معملي" data-en="Lab Tests">تحليل معملي</span>
            </div>
            <div class="stat-card fade-in">
                <div class="stat-icon">
                    <i class="fas fa-bullhorn"></i>
                </div>
                <span class="stat-number">100,000+</span>
                <span class="stat-label" data-ar="تفاعل توعوي" data-en="Awareness Interactions">تفاعل توعوي</span>
            </div>
            <div class="stat-card fade-in">
                <div class="stat-icon">
                    <i class="fas fa-users"></i>
                </div>
                <span class="stat-number">6,000+</span>
                <span class="stat-label" data-ar="متطوع تدرب" data-en="Volunteers Trained">متطوع تدرب</span>
            </div>
        </div>
    </section>

    <!-- Sponsors Section -->
    <section class="sponsors-section" id="sponsors">
        <h2 class="section-title sponsors-title">
            <i class="fas fa-handshake"></i>
            <span data-ar="شركاء النجاح" data-en="Our Sponsors & Partners">شركاء النجاح</span>
        </h2>
        <p class="section-subtitle" data-ar="نتقدم بخالص الشكر لجميع الرعاة والشركاء الذين ساهموا في نجاح القافلة الطبية عبر السنين" data-en="We extend our sincere gratitude to all sponsors and partners who contributed to the success of the Medical Caravan over the years">نتقدم بخالص الشكر لجميع الرعاة والشركاء الذين ساهموا في نجاح القافلة الطبية عبر السنين</p>
        
        <div class="sponsors-grid">
            <div class="sponsor-card fade-in">
                <div class="sponsor-card-icon">
                    <i class="fas fa-star"></i>
                </div>
                <h4 data-ar="أول رعاية رسمية" data-en="First Official Sponsorship">أول رعاية رسمية</h4>
                <p data-ar="2019 - النهضة - السلام" data-en="2019 - El-Nahda - El Salam">2019 - النهضة - السلام</p>
                <span class="sponsor-year" data-ar="MC15" data-en="MC15">MC15</span>
            </div>
            <div class="sponsor-card fade-in">
                <div class="sponsor-card-icon">
                    <i class="fas fa-pills"></i>
                </div>
                <h4>Supremo Pharmaceuticals</h4>
                <p data-ar="2020 - التحول الرقمي" data-en="2020 - Digital Transformation">2020 - التحول الرقمي</p>
                <span class="sponsor-year" data-ar="MC16" data-en="MC16">MC16</span>
            </div>
            <div class="sponsor-card fade-in">
                <div class="sponsor-card-icon">
                    <i class="fas fa-capsules"></i>
                </div>
                <h4>Sato Pharma</h4>
                <p data-ar="2025 - النمو المؤسسي" data-en="2025 - Institutional Growth">2025 - النمو المؤسسي</p>
                <span class="sponsor-year" data-ar="MC20" data-en="MC20">MC20</span>
            </div>
        </div>
    </section>

    <!-- Committees Section -->
    <section class="section" id="committees" style="background: var(--bg-light);">
        <h2 class="section-title" data-ar="لجان القافلة الطبية" data-en="Medical Caravan Committees">لجان القافلة الطبية</h2>
        <p class="section-subtitle" data-ar="ثماني لجان متخصصة تعمل معاً لتحقيق أقصى تأثير في خدمة المجتمع" data-en="Eight specialized committees working together to achieve maximum impact">ثماني لجان متخصصة تعمل معاً لتحقيق أقصى تأثير في خدمة المجتمع</p>

        <div class="committee-grid">
            <!-- Pharmacy Committee -->
            <div class="committee-card fade-in" onclick="openCommitteeModal('pharmacy')">
                <img src="https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/16ac6f2e3-249d-433c-bd39-5d0597f897b6.png" alt="Pharmacy Committee">
                <div class="committee-card-content">
                    <div class="committee-card-icon">
                        <i class="fas fa-pills"></i>
                    </div>
                    <h3 data-ar="لجنة الصيدلة" data-en="Pharmacy Committee">لجنة الصيدلة</h3>
                    <p data-ar="العمود الفقري للقافلة، مسؤولة عن صرف الأدوية والاستشارات الدوائية" data-en="The backbone of the Caravan, responsible for dispensing medications">العمود الفقري للقافلة، مسؤولة عن صرف الأدوية والاستشارات الدوائية</p>
                    <span class="committee-card-badge" data-ar="تأسست 2005" data-en="Founded 2005">تأسست 2005</span>
                </div>
            </div>

            <!-- Lab Committee -->
            <div class="committee-card fade-in" onclick="openCommitteeModal('lab')">
                <img src="https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/137cb0553-c4d5-4aa6-86cf-2b279d266c92.png" alt="Lab Committee">
                <div class="committee-card-content">
                    <div class="committee-card-icon">
                        <i class="fas fa-microscope"></i>
                    </div>
                    <h3 data-ar="لجنة المعمل" data-en="Laboratory Committee">لجنة المعمل</h3>
                    <p data-ar="تقوم بإجراء الفحوصات والتحاليل الطبية بدقة" data-en="Conducts medical tests and laboratory analyses with precision">تقوم بإجراء الفحوصات والتحاليل الطبية بدقة</p>
                    <span class="committee-card-badge" data-ar="تأسست 2005" data-en="Founded 2005">تأسست 2005</span>
                </div>
            </div>

            <!-- Preclinic Committee -->
            <div class="committee-card fade-in" onclick="openCommitteeModal('preclinic')">
                <img src="https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/1a5f181e0-8387-406f-bf1d-67f22e42374c.png" alt="Preclinic Committee">
                <div class="committee-card-content">
                    <div class="committee-card-icon">
                        <i class="fas fa-clipboard-check"></i>
                    </div>
                    <h3 data-ar="لجنة ما قبل العيادة" data-en="Pre-Clinic Committee">لجنة ما قبل العيادة</h3>
                    <p data-ar="نظام الفرز والتقييم الأولي للمرضى، تطوير 2024" data-en="Triage and initial assessment system, 2024 upgrade">نظام الفرز والتقييم الأولي للمرضى، تطوير 2024</p>
                    <span class="committee-card-badge gradient-accent" data-ar="جديد 2024" data-en="New 2024">جديد 2024</span>
                </div>
            </div>

            <!-- Awareness Committee -->
            <div class="committee-card fade-in" onclick="openCommitteeModal('awareness')">
                <img src="https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/1a82b30ee-4dd4-43eb-b3d3-e29636402520.png" alt="Awareness Committee">
                <div class="committee-card-content">
                    <div class="committee-card-icon">
                        <i class="fas fa-bullhorn"></i>
                    </div>
                    <h3 data-ar="لجنة التوعية" data-en="Awareness Committee">لجنة التوعية</h3>
                    <p data-ar="نشر الوعي الصحي وتثقيف المجتمع" data-en="Spreading health awareness and educating the community">نشر الوعي الصحي وتثقيف المجتمع</p>
                    <span class="committee-card-badge" data-ar="تأسست 2005" data-en="Founded 2005">تأسست 2005</span>
                </div>
            </div>

            <!-- HR Committee -->
            <div class="committee-card fade-in" onclick="openCommitteeModal('hr')">
                <img src="https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/14ee3168e-b576-4807-9763-6110549c2112.png" alt="HR Committee">
                <div class="committee-card-content">
                    <div class="committee-card-icon">
                        <i class="fas fa-users-cog"></i>
                    </div>
                    <h3 data-ar="لجنة الموارد البشرية" data-en="Human Resources Committee">لجنة الموارد البشرية</h3>
                    <p data-ar="إدارة الأعضاء وتنظيم الفرق وتطوير الكوادر" data-en="Managing members, organizing teams, and developing personnel">إدارة الأعضاء وتنظيم الفرق وتطوير الكوادر</p>
                    <span class="committee-card-badge" data-ar="تأسست 2016" data-en="Founded 2016">تأسست 2016</span>
                </div>
            </div>

            <!-- FR Committee -->
            <div class="committee-card fade-in" onclick="openCommitteeModal('fr')">
                <img src="https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/14873365c-9a6f-4815-b37d-82b09e3db942.png" alt="FR Committee">
                <div class="committee-card-content">
                    <div class="committee-card-icon">
                        <i class="fas fa-hand-holding-heart"></i>
                    </div>
                    <h3 data-ar="لجنة العلاقات الخارجية" data-en="Fundraising Committee">لجنة العلاقات الخارجية</h3>
                    <p data-ar="تأمين الدعم المالي وبناء الشراكات" data-en="Securing financial support and building partnerships">تأمين الدعم المالي وبناء الشراكات</p>
                    <span class="committee-card-badge" data-ar="تأسست 2017" data-en="Founded 2017">تأسست 2017</span>
                </div>
            </div>

            <!-- Operations Committee -->
            <div class="committee-card fade-in" onclick="openCommitteeModal('operations')">
                <img src="https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/1d33c1670-18f0-4b62-80d9-45c7d21b886a.png" alt="Operations Committee">
                <div class="committee-card-content">
                    <div class="committee-card-icon">
                        <i class="fas fa-truck-medical"></i>
                    </div>
                    <h3 data-ar="لجنة العمليات واللوجستيات" data-en="Operations & Logistics">لجنة العمليات واللوجستيات</h3>
                    <p data-ar="تنظيم الإمدادات الطبية وإدارة المعدات" data-en="Organizing medical supplies and equipment management">تنظيم الإمدادات الطبية وإدارة المعدات</p>
                    <span class="committee-card-badge" data-ar="تأسست 2005" data-en="Founded 2005">تأسست 2005</span>
                </div>
            </div>

            <!-- Media Committee -->
            <div class="committee-card fade-in" onclick="openCommitteeModal('media')">
                <img src="https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/13b0aac78-05dc-40e1-81e4-f9e710ffffda.png" alt="Media Committee">
                <div class="committee-card-content">
                    <div class="committee-card-icon">
                        <i class="fas fa-camera"></i>
                    </div>
                    <h3 data-ar="لجنة الإعلام والتسويق" data-en="Media & Marketing">لجنة الإعلام والتسويق</h3>
                    <p data-ar="إدارة المحتوى الرقمي والتصوير والحملات" data-en="Managing digital content, photography, and campaigns">إدارة المحتوى الرقمي والتصوير والحملات</p>
                    <span class="committee-card-badge" data-ar="تأسست 2015" data-en="Founded 2015">تأسست 2015</span>
                </div>
            </div>
        </div>
    </section>

    <!-- History/Timeline Section -->
    <section class="section" id="history" style="background: white;">
        <h2 class="section-title" data-ar="تاريخ القافلة الطبية" data-en="Medical Caravan History">تاريخ القافلة الطبية</h2>
        <p class="section-subtitle" data-ar="رحلة عشرين عاماً من العطاء والتطور المستمر" data-en="A twenty-year journey of giving and continuous development">رحلة عشرين عاماً من العطاء والتطور المستمر</p>

        <div class="timeline-container">
            <!-- Timeline items remain the same as before -->
            <!-- 2005-2010 -->
            <div class="timeline-item fade-in">
                <div class="timeline-content">
                    <span class="timeline-year-badge">2005 - 2010</span>
                    <h3 class="timeline-title" data-ar="التأسيس والهوية الميدانية" data-en="Foundation & Field Identity">التأسيس والهوية الميدانية</h3>
                    <div class="timeline-location">
                        <i class="fas fa-map-marker-alt"></i>
                        <span data-ar="القرى النائية - إسماعيلية، الفيوم" data-en="Remote Villages - Ismailia, Fayoum">القرى النائية - إسماعيلية، الفيوم</span>
                    </div>
                    <p class="timeline-text" data-ar="تأسست القافلة الطبية عام 2005 (MC1) كمبادرة طلابية مبنية على أربع لجان أساسية: الصيدلة، المعمل، التوعية، وإدارة المشاريع." data-en="Medical Caravan was founded in 2005 (MC1) as a student-led initiative built on four core committees.">تأسست القافلة الطبية عام 2005 (MC1) كمبادرة طلابية مبنية على أربع لجان أساسية: الصيدلة، المعمل، التوعية، وإدارة المشاريع.</p>
                    <div class="timeline-stats">
                        <div class="timeline-stat">
                            <span class="timeline-stat-number">800-1,200</span>
                            <span class="timeline-stat-label" data-ar="روشتة سنوياً" data-en="Prescriptions/Year">روشتة سنوياً</span>
                        </div>
                        <div class="timeline-stat">
                            <span class="timeline-stat-number">200-400</span>
                            <span class="timeline-stat-label" data-ar="تحليل معملي" data-en="Lab Tests">تحليل معملي</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 2025 MC20 -->
            <div class="timeline-item fade-in">
                <div class="timeline-content">
                    <span class="timeline-year-badge">2025 (MC20)</span>
                    <h3 class="timeline-title" data-ar="النمو المؤسسي والتوسع" data-en="Institutional Growth & Expansion">النمو المؤسسي والتوسع</h3>
                    <div class="timeline-location">
                        <i class="fas fa-building"></i>
                        <span data-ar="عام التوسع المؤسسي" data-en="Institutional Expansion Year">عام التوسع المؤسسي</span>
                    </div>
                    <p class="timeline-text" data-ar="استمرت القافلة في التطور كمنظمة أكثر نضجاً وهيكلة." data-en="The Caravan continued evolving as a more mature organization.">استمرت القافلة في التطور كمنظمة أكثر نضجاً وهيكلة.</p>
                    <div class="timeline-tags">
                        <span class="timeline-tag sponsor" data-ar="ساتو فارما" data-en="Sato Pharma">ساتو فارما</span>
                        <span class="timeline-tag purple" data-ar="لينكد إن" data-en="LinkedIn">لينكد إن</span>
                    </div>
                    <div class="sponsor-badge">
                        <i class="fas fa-handshake"></i>
                        <span data-ar="الراعي: ساتو فارما" data-en="Sponsor: Sato Pharma">الراعي: ساتو فارما</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="section" id="contact" style="background: var(--bg-light);">
        <h2 class="section-title" data-ar="تواصل معنا" data-en="Contact Us">تواصل معنا</h2>
        <p class="section-subtitle" data-ar="نسعد بتواصلكم معنا للانضمام أو الاستفسار" data-en="We are happy to hear from you for joining or inquiries">نسعد بتواصلكم معنا للانضمام أو الاستفسار</p>

        <div class="vision-grid">
            <div class="card fade-in" style="padding: 35px 25px; text-align: center;">
                <div class="vision-icon">
                    <i class="fas fa-envelope"></i>
                </div>
                <h3 data-ar="البريد الإلكتروني" data-en="Email">البريد الإلكتروني</h3>
                <a href="mailto:medicalcaravaneasu14@gmail.com" class="contact-link email" style="margin-top: 15px;">
                    <i class="fas fa-envelope"></i>
                    <span>medicalcaravaneasu14@gmail.com</span>
                </a>
            </div>
            <div class="card fade-in" style="padding: 35px 25px; text-align: center;">
                <div class="vision-icon">
                    <i class="fas fa-map-marker-alt"></i>
                </div>
                <h3 data-ar="العنوان" data-en="Address">العنوان</h3>
                <p data-ar="كلية الصيدلة، جامعة عين شمس، القاهرة، مصر" data-en="Faculty of Pharmacy, Ain Shams University, Cairo, Egypt">كلية الصيدلة، جامعة عين شمس، القاهرة، مصر</p>
            </div>
            <div class="card fade-in" style="padding: 35px 25px; text-align: center;">
                <div class="vision-icon">
                    <i class="fas fa-share-alt"></i>
                </div>
                <h3 data-ar="وسائل التواصل" data-en="Social Media">وسائل التواصل</h3>
                <div class="footer-social" style="justify-content: center; margin-top: 20px;">
                    <a href="https://eg.linkedin.com/company/medical-caravan?trk=public_post_feed-actor-name" target="_blank" class="linkedin" title="LinkedIn">
                        <i class="fab fa-linkedin-in"></i>
                    </a>
                    <a href="https://www.facebook.com/share/1FqKn8A188/?mibextid=wwXIfr" target="_blank" class="facebook" title="Facebook">
                        <i class="fab fa-facebook-f"></i>
                    </a>
                    <a href="https://www.instagram.com/medical_caravan?igsh=MTd3a2JvcGcyYXNoeA%3D%3D&utm_source=qr" target="_blank" class="instagram" title="Instagram">
                        <i class="fab fa-instagram"></i>
                    </a>
                    <a href="mailto:medicalcaravaneasu14@gmail.com" class="email" title="Email">
                        <i class="fas fa-envelope"></i>
                    </a>
                </div>
                <div style="margin-top: 20px;">
                    <a href="https://eg.linkedin.com/company/medical-caravan?trk=public_post_feed-actor-name" target="_blank" class="contact-link linkedin">
                        <i class="fab fa-linkedin-in"></i>
                        <span data-ar="لينكد إن" data-en="LinkedIn">لينكد إن</span>
                    </a>
                    <a href="https://www.facebook.com/share/1FqKn8A188/?mibextid=wwXIfr" target="_blank" class="contact-link facebook">
                        <i class="fab fa-facebook-f"></i>
                        <span data-ar="فيسبوك" data-en="Facebook">فيسبوك</span>
                    </a>
                    <a href="https://www.instagram.com/medical_caravan?igsh=MTd3a2JvcGcyYXNoeA%3D%3D&utm_source=qr" target="_blank" class="contact-link instagram">
                        <i class="fab fa-instagram"></i>
                        <span data-ar="إنستجرام" data-en="Instagram">إنستجرام</span>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer-content">
            <div class="footer-section">
                <h4><i class="fas fa-heartbeat"></i> <span data-ar="عن القافلة" data-en="About Caravan">عن القافلة</span></h4>
                <p data-ar="القافلة الطبية بكلية الصيدلة جامعة عين شمس هي مبادرة طلابية تطوعية تهدف إلى تقديم خدمات صحية مجانية للمجتمعات المحرومة." data-en="Medical Caravan at Ain Shams Faculty of Pharmacy is a student volunteer initiative aimed at providing free healthcare services.">القافلة الطبية بكلية الصيدلة جامعة عين شمس هي مبادرة طلابية تطوعية تهدف إلى تقديم خدمات صحية مجانية للمجتمعات المحرومة.</p>
            </div>
            <div class="footer-section">
                <h4><i class="fas fa-link"></i> <span data-ar="روابط سريعة" data-en="Quick Links">روابط سريعة</span></h4>
                <a href="#home" data-ar="الرئيسية" data-en="Home">الرئيسية</a>
                <a href="#about" data-ar="عن القافلة" data-en="About">عن القافلة</a>
                <a href="#sponsors" data-ar="الرعاة" data-en="Sponsors">الرعاة</a>
                <a href="#committees" data-ar="اللجان" data-en="Committees">اللجان</a>
                <a href="#history" data-ar="التاريخ" data-en="History">التاريخ</a>
            </div>
            <div class="footer-section">
                <h4><i class="fas fa-users"></i> <span data-ar="تواصل معنا" data-en="Contact Us">تواصل معنا</span></h4>
                <div class="footer-social">
                    <a href="https://eg.linkedin.com/company/medical-caravan?trk=public_post_feed-actor-name" target="_blank" class="linkedin" title="LinkedIn">
                        <i class="fab fa-linkedin-in"></i>
                    </a>
                    <a href="https://www.facebook.com/share/1FqKn8A188/?mibextid=wwXIfr" target="_blank" class="facebook" title="Facebook">
                        <i class="fab fa-facebook-f"></i>
                    </a>
                    <a href="https://www.instagram.com/medical_caravan?igsh=MTd3a2JvcGcyYXNoeA%3D%3D&utm_source=qr" target="_blank" class="instagram" title="Instagram">
                        <i class="fab fa-instagram"></i>
                    </a>
                    <a href="mailto:medicalcaravaneasu14@gmail.com" class="email" title="Email">
                        <i class="fas fa-envelope"></i>
                    </a>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <p data-ar="© 2025 القافلة الطبية - كلية الصيدلة جامعة عين شمس. جميع الحقوق محفوظة." data-en="© 2025 Medical Caravan - Ain Shams Faculty of Pharmacy. All rights reserved.">© 2025 القافلة الطبية - كلية الصيدلة جامعة عين شمس. جميع الحقوق محفوظة.</p>
        </div>
    </footer>

    <!-- Committee Full Page Modal -->
    <div class="modal" id="committeeModal">
        <div class="modal-content">
            <button class="modal-close" onclick="closeCommitteeModal()">
                <i class="fas fa-times"></i>
            </button>
            <div class="modal-header">
                <img id="modalImage" src="" alt="">
                <h2 id="modalTitle"></h2>
                <p id="modalSubtitle"></p>
            </div>
            <div class="modal-body" id="modalBody">
            </div>
        </div>
    </div>

    <script>
        let currentLang = 'ar';
        let countersAnimated = false;

        const committeeData = {
            pharmacy: {
                ar: {
                    title: 'لجنة الصيدلة',
                    subtitle: 'Pharmacy Committee - تأسست عام 2005',
                    description: 'لجنة الصيدلة هي العمود الفقري للقافلة الطبية منذ تأسيسها عام 2005.',
                    overview: 'تعتبر لجنة الصيدلة من الركائز الأساسية التي بنيت عليها القافلة الطبية منذ بدايتها.',
                    responsibilities: ['صرف الأدوية الموصوفة من الأطباء بدقة وسرعة', 'تقديم استشارات دوائية متخصصة للمرضى', 'شرح طريقة استخدام الأدوية والجرعات الصحيحة'],
                    impact: ['800-1,200 روشتة سنوياً في السنوات الأولى', '2,000+ روشتة في الحملات الكبيرة', 'تثقيف دوائي شامل لكل مريض'],
                    skills: ['المعرفة الدوائية العميقة', 'مهارات التواصل الفعال', 'إدارة المخزون'],
                    evolution: ['2005: التأسيس', '2012: التوسع في القاهرة', '2024: دمج نظام ما قبل العيادة']
                },
                en: {
                    title: 'Pharmacy Committee',
                    subtitle: 'Founded 2005',
                    description: 'The Pharmacy Committee is the backbone of the Medical Caravan since 2005.',
                    overview: 'The Pharmacy Committee is one of the fundamental pillars on which the Medical Caravan was built.',
                    responsibilities: ['Dispensing prescribed medications accurately', 'Providing pharmaceutical consultations', 'Explaining medication usage'],
                    impact: ['800-1,200 prescriptions annually in early years', '2,000+ prescriptions in large campaigns', 'Comprehensive pharmaceutical education'],
                    skills: ['Deep pharmaceutical knowledge', 'Effective communication', 'Inventory management'],
                    evolution: ['2005: Founded', '2012: Cairo expansion', '2024: Pre-Clinic integration']
                },
                image: 'https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/16ac6f2e3-249d-433c-bd39-5d0597f897b6.png'
            },
            lab: {
                ar: {
                    title: 'لجنة المعمل',
                    subtitle: 'Laboratory Committee - تأسست عام 2005',
                    description: 'لجنة المعمل تقوم بإجراء الفحوصات والتحاليل الطبية للمرضى باستخدام أحدث الأجهزة.',
                    overview: 'تعتبر لجنة المعمل من اللجان الأساسية التي تأسست مع القافلة عام 2005.',
                    responsibilities: ['إجراء تحاليل الدم الأساسية', 'تحليل السكر والكوليسترول', 'فحوصات وظائف الكبد والكلى'],
                    impact: ['200-400 تحليل في السنوات الأولى', '1,000+ تحليل في الحملات الكبيرة', 'تشخيص دقيق'],
                    skills: ['المهارات المعملية', 'الدقة في النتائج', 'التعامل مع الأجهزة'],
                    evolution: ['2005: التأسيس', '2016: تحاليل متقدمة', '2025: توسيع نطاق التحاليل']
                },
                en: {
                    title: 'Laboratory Committee',
                    subtitle: 'Founded 2005',
                    description: 'The Laboratory Committee conducts medical tests using modern equipment.',
                    overview: 'The Laboratory Committee is one of the fundamental committees founded in 2005.',
                    responsibilities: ['Performing basic blood tests', 'Sugar and cholesterol analysis', 'Liver and kidney function tests'],
                    impact: ['200-400 tests in early years', '1,000+ tests in large campaigns', 'Accurate diagnosis'],
                    skills: ['Technical laboratory skills', 'Accuracy in results', 'Equipment handling'],
                    evolution: ['2005: Founded', '2016: Advanced tests', '2025: Expanded test range']
                },
                image: 'https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/137cb0553-c4d5-4aa6-86cf-2b279d266c92.png'
            },
            preclinic: {
                ar: {
                    title: 'لجنة ما قبل العيادة',
                    subtitle: 'Pre-Clinic Committee - تطوير 2024',
                    description: 'نظام ما قبل العيادة هو طبقة الفرز والتقييم الأولى للمرضى قبل الوصول للطبيب.',
                    overview: 'تعتبر لجنة ما قبل العيادة أحدث إضافة لهيكل القافلة الطبية.',
                    responsibilities: ['تقييم المرضى الأولي', 'تسجيل البيانات الطبية', 'توجيه الحالات للعيادة المناسبة'],
                    impact: ['تحسين الكفاءة 40%', 'تقليل وقت الانتظار 50%', 'تجربة مريض أفضل'],
                    skills: ['التقييم السريع', 'التصنيف الطبي', 'إدارة التدفق'],
                    evolution: ['2024: الإطلاق', '2025: التطوير المستمر']
                },
                en: {
                    title: 'Pre-Clinic Committee',
                    subtitle: '2024 Upgrade',
                    description: 'The Pre-Clinic System is the first triage layer for patients.',
                    overview: 'The Pre-Clinic Committee is the latest addition to the Caravan structure.',
                    responsibilities: ['Initial patient assessment', 'Recording medical data', 'Directing cases efficiently'],
                    impact: ['40% efficiency improvement', '50% waiting time reduction', 'Better patient experience'],
                    skills: ['Quick assessment', 'Medical triage', 'Flow management'],
                    evolution: ['2024: Launch', '2025: Continuous development']
                },
                image: 'https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/1a5f181e0-8387-406f-bf1d-67f22e42374c.png'
            },
            awareness: {
                ar: {
                    title: 'لجنة التوعية',
                    subtitle: 'Awareness Committee - تأسست عام 2005',
                    description: 'لجنة التوعية مسؤولة عن نشر الوعي الصحي وتثقيف المجتمع.',
                    overview: 'تعتبر لجنة التوعية من اللجان الأساسية التي تأسست مع القافلة عام 2005.',
                    responsibilities: ['تنظيم جلسات توعية', 'توزيع مواد تثقيفية', 'حملات الكشف المبكر'],
                    impact: ['6,742 تفاعل في 2018', '6,245 تفاعل في 2023', 'حملة وجه وأمل'],
                    skills: ['مهارات العرض', 'التواصل المجتمعي', 'التصميم الإبداعي'],
                    evolution: ['2005: التأسيس', '2018: ذروة التفاعل', '2023: حملة وجه وأمل']
                },
                en: {
                    title: 'Awareness Committee',
                    subtitle: 'Founded 2005',
                    description: 'The Awareness Committee spreads health awareness in the community.',
                    overview: 'The Awareness Committee is one of the fundamental committees founded in 2005.',
                    responsibilities: ['Organizing awareness sessions', 'Distributing educational materials', 'Early detection campaigns'],
                    impact: ['6,742 interactions in 2018', '6,245 interactions in 2023', 'Face & Hope Campaign'],
                    skills: ['Presentation skills', 'Community communication', 'Creative design'],
                    evolution: ['2005: Founded', '2018: Peak engagement', '2023: Face & Hope Campaign']
                },
                image: 'https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/1a82b30ee-4dd4-43eb-b3d3-e29636402520.png'
            },
            hr: {
                ar: {
                    title: 'لجنة الموارد البشرية',
                    subtitle: 'Human Resources Committee - تأسست عام 2016',
                    description: 'تم إدخال لجنة الموارد البشرية عام 2016، مما حول القافلة إلى منظمة أكثر هيكلة.',
                    overview: 'تعتبر لجنة الموارد البشرية إضافة استراتيجية لهيكل القافلة.',
                    responsibilities: ['تنظيم الأعضاء في فرق', 'إدارة التواصل الداخلي', 'تطوير الأعضاء'],
                    impact: ['100+ عضو سنوياً', 'تحسين الإنتاجية 35%', '6,000+ متطوع'],
                    skills: ['إدارة الموارد البشرية', 'حل النزاعات', 'القيادة'],
                    evolution: ['2016: التأسيس', '2020: التحول الرقمي', '2025: 6,000+ متطوع']
                },
                en: {
                    title: 'Human Resources Committee',
                    subtitle: 'Founded 2016',
                    description: 'HR Committee introduced in 2016, transforming Caravan into structured organization.',
                    overview: 'The HR Committee is a strategic addition to the Caravan structure.',
                    responsibilities: ['Organizing members into teams', 'Managing internal communication', 'Member development'],
                    impact: ['100+ members annually', '35% productivity improvement', '6,000+ volunteers'],
                    skills: ['HR management', 'Conflict resolution', 'Leadership'],
                    evolution: ['2016: Founded', '2020: Digital transformation', '2025: 6,000+ volunteers']
                },
                image: 'https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/14ee3168e-b576-4807-9763-6110549c2112.png'
            },
            fr: {
                ar: {
                    title: 'لجنة العلاقات الخارجية',
                    subtitle: 'Fundraising Committee - تأسست عام 2017',
                    description: 'بدأت جهود جمع التمويل عام 2017، مما أدخل الاستدامة المالية للقافلة.',
                    overview: 'تعتبر لجنة العلاقات الخارجية إضافة استراتيجية لضمان استدامة القافلة.',
                    responsibilities: ['تأمين الدعم المالي', 'بناء الشراكات', 'التواصل مع الرعاة'],
                    impact: ['أول رعاية 2019', 'سوبريمو 2020', 'ساتو 2025'],
                    skills: ['التفاوض', 'بناء العلاقات', 'إدارة الشراكات'],
                    evolution: ['2017: البداية', '2019: أول رعاية', '2025: ساتو فارما']
                },
                en: {
                    title: 'Fundraising Committee',
                    subtitle: 'Founded 2017',
                    description: 'Fundraising began in 2017, introducing financial sustainability.',
                    overview: 'The Fundraising Committee ensures the Caravan\'s financial sustainability.',
                    responsibilities: ['Securing financial support', 'Building partnerships', 'Communicating with sponsors'],
                    impact: ['First sponsorship 2019', 'Supremo 2020', 'Sato 2025'],
                    skills: ['Negotiation', 'Relationship building', 'Partnership management'],
                    evolution: ['2017: Beginning', '2019: First sponsorship', '2025: Sato Pharma']
                },
                image: 'https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/14873365c-9a6f-4815-b37d-82b09e3db942.png'
            },
            operations: {
                ar: {
                    title: 'لجنة العمليات واللوجستيات',
                    subtitle: 'Operations & Logistics - تأسست عام 2005',
                    description: 'مسؤولة عن تنظيم الإمدادات الطبية وإدارة المعدات والتنسيق الميداني.',
                    overview: 'تعتبر لجنة العمليات من اللجان الأساسية التي تأسست مع القافلة عام 2005.',
                    responsibilities: ['تنظيم الإمدادات', 'إدارة المعدات', 'التنسيق الشامل'],
                    impact: ['20+ حملة سنوياً', '100,000+ جنيه معدات', '100+ متطوع'],
                    skills: ['التخطيط اللوجستي', 'إدارة الإمداد', 'القيادة الميدانية'],
                    evolution: ['2005: التأسيس', '2022: عودة العمليات', '2024: نظام ما قبل العيادة']
                },
                en: {
                    title: 'Operations & Logistics',
                    subtitle: 'Founded 2005',
                    description: 'Responsible for medical supplies, equipment, and field coordination.',
                    overview: 'The Operations Committee is one of the fundamental committees founded in 2005.',
                    responsibilities: ['Organizing medical supplies', 'Equipment management', 'Comprehensive coordination'],
                    impact: ['20+ campaigns annually', '100,000+ EGP equipment', '100+ volunteers'],
                    skills: ['Logistical planning', 'Supply management', 'Field leadership'],
                    evolution: ['2005: Founded', '2022: Multi-day operations', '2024: Pre-Clinic system']
                },
                image: 'https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/1d33c1670-18f0-4b62-80d9-45c7d21b886a.png'
            },
            media: {
                ar: {
                    title: 'لجنة الإعلام والتسويق',
                    subtitle: 'Media & Marketing - تأسست عام 2015',
                    description: 'تم إدخال لجنة التسويق عام 2015، عززت الهوية البصرية للقافلة.',
                    overview: 'تعتبر لجنة الإعلام والتسويق إضافة حديثة لهيكل القافلة.',
                    responsibilities: ['محتوى السوشيال ميديا', 'التصوير', 'تصميم الهوية'],
                    impact: ['زيادة الوضوح', 'جذب متطوعين', 'لينكد إن 2025'],
                    skills: ['التصميم', 'التصوير', 'إدارة السوشيال ميديا'],
                    evolution: ['2015: التأسيس', '2020: التحول الرقمي', '2025: لينكد إن']
                },
                en: {
                    title: 'Media & Marketing',
                    subtitle: 'Founded 2015',
                    description: 'Marketing Committee introduced in 2015, strengthened visual identity.',
                    overview: 'The Media & Marketing Committee is a recent addition to the Caravan.',
                    responsibilities: ['Social media content', 'Photography', 'Identity design'],
                    impact: ['Increased visibility', 'Attracting volunteers', 'LinkedIn 2025'],
                    skills: ['Design', 'Photography', 'Social media management'],
                    evolution: ['2015: Founded', '2020: Digital transformation', '2025: LinkedIn']
                },
                image: 'https://image.qwenlm.ai/public_source/125bdda8-7b09-4539-bc81-787fba55e8b1/13b0aac78-05dc-40e1-81e4-f9e710ffffda.png'
            }
        };

        function toggleLanguage() {
            currentLang = currentLang === 'ar' ? 'en' : 'ar';
            document.documentElement.lang = currentLang;
            document.documentElement.dir = currentLang === 'ar' ? 'rtl' : 'ltr';
            document.body.classList.toggle('en');
            document.getElementById('lang-text').textContent = currentLang === 'ar' ? 'English' : 'عربي';
            
            document.querySelectorAll('[data-ar]').forEach(el => {
                el.textContent = el.getAttribute(`data-${currentLang}`);
            });
        }

        function toggleMobileNav() {
            const mobileNav = document.getElementById('mobileNav');
            mobileNav.classList.toggle('active');
        }

        function openCommitteeModal(committee) {
            const data = committeeData[committee][currentLang];
            const modal = document.getElementById('committeeModal');
            
            document.getElementById('modalImage').src = committeeData[committee].image;
            document.getElementById('modalTitle').textContent = data.title;
            document.getElementById('modalSubtitle').textContent = data.subtitle;
            
            let content = `
                <div class="modal-section">
                    <h3><i class="fas fa-info-circle"></i> ${currentLang === 'ar' ? 'نظرة عامة' : 'Overview'}</h3>
                    <p style="font-size: 1.05rem; line-height: 2;">${data.overview}</p>
                </div>
                
                <div class="modal-section">
                    <h3><i class="fas fa-book-open"></i> ${currentLang === 'ar' ? 'وصف اللجنة' : 'Description'}</h3>
                    <p style="font-size: 1.05rem; line-height: 2;">${data.description}</p>
                </div>
                
                <div class="modal-section">
                    <h3><i class="fas fa-tasks"></i> ${currentLang === 'ar' ? 'المسؤوليات' : 'Responsibilities'}</h3>
                    <ul>${data.responsibilities.map(item => `<li>${item}</li>`).join('')}</ul>
                </div>
                
                <div class="modal-section">
                    <h3><i class="fas fa-chart-line"></i> ${currentLang === 'ar' ? 'الأثر' : 'Impact'}</h3>
                    <div class="impact-badges">${data.impact.map(item => `<span class="impact-badge">${item}</span>`).join('')}</div>
                </div>
                
                <div class="modal-section">
                    <h3><i class="fas fa-graduation-cap"></i> ${currentLang === 'ar' ? 'المهارات' : 'Skills'}</h3>
                    <div class="detail-grid">${data.skills.map(skill => `<div class="detail-card"><i class="fas fa-check-circle"></i><h5>${skill}</h5></div>`).join('')}</div>
                </div>
                
                <div class="modal-section">
                    <h3><i class="fas fa-history"></i> ${currentLang === 'ar' ? 'التطور' : 'Evolution'}</h3>
                    <div class="timeline-evolution"><ul>${data.evolution.map(item => `<li>${item}</li>`).join('')}</ul></div>
                </div>
            `;
            
            document.getElementById('modalBody').innerHTML = content;
            modal.classList.add('active');
            document.body.style.overflow = 'hidden';
        }

        function closeCommitteeModal() {
            document.getElementById('committeeModal').classList.remove('active');
            document.body.style.overflow = 'auto';
        }

        document.getElementById('committeeModal').addEventListener('click', function(e) {
            if (e.target === this) {
                closeCommitteeModal();
            }
        });

        document.addEventListener('keydown', function(e) {
            if (e.key === 'Escape') {
                closeCommitteeModal();
            }
        });

        function animateCounters() {
            const counters = document.querySelectorAll('[data-counter]');
            counters.forEach(counter => {
                const target = parseInt(counter.getAttribute('data-counter'));
                const duration = 2000;
                const step = target / (duration / 16);
                let current = 0;
                
                const updateCounter = () => {
                    current += step;
                    if (current < target) {
                        counter.textContent = Math.floor(current).toLocaleString();
                        requestAnimationFrame(updateCounter);
                    } else {
                        counter.textContent = target >= 1000 ? (target / 1000).toFixed(0) + 'K+' : target;
                    }
                };
                
                updateCounter();
            });
        }

        function scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        window.addEventListener('scroll', function() {
            const navbar = document.getElementById('navbar');
            const scrollTop = document.getElementById('scrollTop');
            
            if (window.scrollY > 100) {
                navbar.classList.add('scrolled');
                scrollTop.classList.add('visible');
            } else {
                navbar.classList.remove('scrolled');
                scrollTop.classList.remove('visible');
            }

            if (window.scrollY < 500 && !countersAnimated) {
                countersAnimated = true;
                animateCounters();
            }
        });

        const observerOptions = { threshold: 0.1, rootMargin: '0px 0px -50px 0px' };
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in, .timeline-item').forEach(el => {
            observer.observe(el);
        });

        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });
    </script>
</body>
</html>

