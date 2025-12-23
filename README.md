<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jubril Adams | Cloud & Systems Engineer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #00f5ff;
            --secondary: #7b2cbf;
            --dark: #0a0e27;
            --darker: #050816;
            --light: #e8f5ff;
            --gray: #a0a0a0;
            --card-bg: #151932;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: var(--darker);
            color: var(--light);
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Animated Background */
        .bg-animation {
            position: fixed;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            z-index: -1;
            background: linear-gradient(135deg, var(--darker) 0%, var(--dark) 100%);
        }

        .bg-animation::before {
            content: '';
            position: absolute;
            width: 500px;
            height: 500px;
            background: radial-gradient(circle, rgba(0, 245, 255, 0.1) 0%, transparent 70%);
            border-radius: 50%;
            top: -250px;
            right: -250px;
            animation: float 20s infinite alternate;
        }

        .bg-animation::after {
            content: '';
            position: absolute;
            width: 400px;
            height: 400px;
            background: radial-gradient(circle, rgba(123, 44, 191, 0.1) 0%, transparent 70%);
            border-radius: 50%;
            bottom: -200px;
            left: -200px;
            animation: float 15s infinite alternate-reverse;
        }

        @keyframes float {
            to {
                transform: translate(100px, 100px);
            }
        }

        /* Navigation */
        nav {
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            background: rgba(10, 14, 39, 0.8);
            backdrop-filter: blur(10px);
            padding: 1rem 0;
            transition: all 0.3s;
        }

        nav.scrolled {
            background: rgba(10, 14, 39, 0.95);
            box-shadow: 0 5px 30px rgba(0, 0, 0, 0.3);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            color: var(--light);
            text-decoration: none;
            transition: color 0.3s;
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary);
            transition: width 0.3s;
        }

        .nav-links a:hover::after,
        .nav-links a.active::after {
            width: 100%;
        }

        /* Container & Sections */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        section {
            padding: 100px 0;
            min-height: 60vh;
            display: flex;
            align-items: center;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding-top: 140px;
        }

        .hero h1 {
            font-size: 3.2rem;
            margin-bottom: 0.5rem;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: fadeInUp 1s;
        }

        .hero .role {
            font-size: 1.2rem;
            color: var(--gray);
            margin-bottom: 0.25rem;
        }

        .hero .availability {
            font-size: 0.95rem;
            color: var(--primary);
            margin-bottom: 1rem;
            text-transform: uppercase;
            letter-spacing: 0.08em;
        }

        .hero .subtitle {
            font-size: 1.3rem;
            color: var(--gray);
            margin-bottom: 1.5rem;
            animation: fadeInUp 1s 0.2s backwards;
        }

        .hero p {
            max-width: 650px;
            margin: 0 auto 2rem;
            color: var(--gray);
            animation: fadeInUp 1s 0.4s backwards;
        }

        .cta-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            justify-content: center;
            animation: fadeInUp 1s 0.6s backwards;
        }

        .btn {
            padding: 1rem 2rem;
            border: none;
            border-radius: 999px;
            font-size: 1rem;
            cursor: pointer;
            transition: all 0.3s;
            text-decoration: none;
            display: inline-block;
            font-weight: 500;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0, 245, 255, 0.3);
        }

        .btn-secondary {
            background: transparent;
            border: 2px solid var(--primary);
            color: var(--primary);
        }

        .btn-secondary:hover {
            background: var(--primary);
            color: var(--dark);
        }

        .btn
