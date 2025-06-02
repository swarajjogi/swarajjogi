<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Swaraj Jogi | UI/UX Designer</title>

  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>

  <!-- Animate.css -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css" />

  <style>
    /* Creative Hover Animation for Projects */
    .project-card {
      transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
      position: relative;
      overflow: hidden;
      border-radius: 0.375rem;
    }

    .project-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      border-radius: 0.375rem;
      background: linear-gradient(45deg, rgba(59, 130, 246, 0.3), rgba(147, 51, 234, 0.3));
      opacity: 0;
      transition: opacity 0.4s ease;
      z-index: 1;
    }

    .project-card:hover {
      transform: scale(1.05) rotate(1deg);
      box-shadow: 0 20px 40px rgba(59, 130, 246, 0.3), 0 0 20px rgba(147, 51, 234, 0.2);
    }

    .project-card:hover::before {
      opacity: 1;
    }

    .project-card .project-content {
      position: relative;
      z-index: 2;
    }

    .project-card:hover .project-title {
      color: rgb(140, 158, 148);
      text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
    }

    /* Smooth image scaling */
    .project-card img {
      transition: transform 0.4s ease;
    }

    .project-card:hover img {
      transform: scale(1.1);
    }

    /* Additional sparkle effect */
    .project-card::after {
      content: '✦';
      position: absolute;
      top: 10px;
      right: 10px;
      color: white;
      font-size: 1.2rem;
      opacity: 0;
      transform: scale(0) rotate(0deg);
      transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
      z-index: 3;
    }

    .project-card:hover::after {
      opacity: 1;
      transform: scale(1) rotate(180deg);
    }
  </style>
</head>

<body class="bg-white text-gray-800 font-sans">

  <!-- Navbar -->
  <header class="bg-white shadow-md sticky top-0 z-50 animate__animated animate__fadeInDown">
    <div
      class="max-w-7xl mx-auto px-4 py-4 flex flex-col sm:flex-row justify-between items-center space-y-2 sm:space-y-0">
      <h1 class="text-2xl font-bold">Swaraj Jogi</h1>
      <nav class="flex flex-wrap justify-center gap-4 text-base">
        <a href="#home" class="hover:text-blue-500 transition duration-300">Home</a>
        <a href="#projects" class="hover:text-blue-500 transition duration-300">Projects</a>
        <a href="#about" class="hover:text-blue-500 transition duration-300">About</a>
        <a href="#contact" class="hover:text-blue-500 transition duration-300">Contact</a>
      </nav>
    </div>
  </header>
</html>
