import React from 'react';
import { Github, Linkedin, Instagram, Mail } from 'lucide-react';

function App() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-gray-900 to-gray-800 text-white">
      {/* Header Section */}
      <header className="container mx-auto px-4 py-16 text-center">
        <h1 className="text-4xl md:text-6xl font-bold mb-4">
          Hi <span className="inline-block animate-wave">👋</span>, I'm Yessin Khlif
        </h1>
        <p className="text-xl md:text-2xl text-gray-300 max-w-3xl mx-auto">
          A passionate and collaborative software engineer student learning DevOps practices.
        </p>
      </header>

      {/* Current Status Section */}
      <section className="container mx-auto px-4 py-8">
        <div className="bg-gray-800/50 rounded-lg p-6 max-w-3xl mx-auto space-y-4">
          <div className="flex items-center space-x-3">
            <span className="text-xl">🏃</span>
            <p className="text-lg">I'm currently working on <span className="text-blue-400">DevOps Project</span>.</p>
          </div>
          <div className="flex items-center space-x-3">
            <span className="text-xl">🌱</span>
            <p className="text-lg">I'm currently learning <span className="text-green-400">MicroServices</span>.</p>
          </div>
          <div className="flex items-center space-x-3">
            <span className="text-xl">💝</span>
            <p className="text-lg">I'm looking for an internship in <span className="text-purple-400">DevOps or Blockchain Technology</span>.</p>
          </div>
          <div className="flex items-center space-x-3">
            <span className="text-xl">📫</span>
            <p className="text-lg">How to reach me: <a href="mailto:khlifyessin@gmail.com" className="text-blue-400 hover:underline">khlifyessin@gmail.com</a></p>
          </div>
        </div>
      </section>

      {/* Technologies Section */}
      <section className="container mx-auto px-4 py-8">
        <h2 className="text-3xl font-bold text-center mb-8">Technologies & Tools</h2>
        <div className="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-4 max-w-4xl mx-auto">
          {technologies.map((tech) => (
            <div key={tech.name} className="flex flex-col items-center p-4 bg-gray-800/30 rounded-lg hover:bg-gray-700/30 transition-colors">
              <img src={tech.icon} alt={tech.name} className="w-12 h-12 object-contain" />
              <span className="mt-2 text-sm">{tech.name}</span>
            </div>
          ))}
        </div>
      </section>

      {/* Connect Section */}
      <section className="container mx-auto px-4 py-8">
        <h2 className="text-3xl font-bold text-center mb-8">Connect with me</h2>
        <div className="flex justify-center space-x-6">
          <a href="https://github.com/yessin007" className="text-gray-300 hover:text-white transition-colors">
            <Github size={32} />
          </a>
          <a href="https://www.linkedin.com/in/yessin-khlif" className="text-gray-300 hover:text-white transition-colors">
            <Linkedin size={32} />
          </a>
          <a href="https://www.instagram.com/yessinkhlif" className="text-gray-300 hover:text-white transition-colors">
            <Instagram size={32} />
          </a>
          <a href="mailto:khlifyessin@gmail.com" className="text-gray-300 hover:text-white transition-colors">
            <Mail size={32} />
          </a>
        </div>
      </section>
    </div>
  );
}

const technologies = [
  { name: 'Angular', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/angularjs/angularjs-original.svg' },
  { name: 'AWS', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original.svg' },
  { name: 'Azure', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/azure/azure-original.svg' },
  { name: 'Bootstrap', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-original.svg' },
  { name: 'C#', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg' },
  { name: 'CSS', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg' },
  { name: 'Docker', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg' },
  { name: '.NET', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/dot-net/dot-net-original.svg' },
  { name: 'GCP', icon: 'https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg' },
  { name: 'NestJS', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/nestjs/nestjs-plain.svg' },
  { name: 'HTML', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg' },
  { name: 'Java', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg' },
  { name: 'JavaScript', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg' },
  { name: 'Linux', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg' },
  { name: 'MongoDB', icon: 'https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original.svg' }
];

export default App;
