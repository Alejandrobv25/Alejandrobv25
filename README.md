## Hi there 👋
// Portfolio Profesional en React + Tailwind CSS
// Archivo: src/App.jsx

import React from "react";
import { FaGithub, FaLinkedin, FaEnvelope } from "react-icons/fa";

const projects = [
  {
    title: "[Nombre del Proyecto]",
    description: "[Descripción del proyecto]",
    url: "https://github.com/tuusuario/repositorio"
  },
  // Agrega más proyectos aquí
];

const skills = [
  "JavaScript",
  "React",
  "Tailwind CSS",
  "Node.js",
  // Agrega más habilidades
];

export default function App() {
  return (
    <div className="min-h-screen bg-white text-gray-800 font-sans">
      {/* Hero */}
      <section className="text-center py-16 px-4 bg-gray-100">
        <h1 className="text-5xl font-bold mb-2">[Tu Nombre Aquí]</h1>
        <p className="text-xl text-gray-600">[Tu Profesión o especialidad]</p>
        <div className="flex justify-center gap-6 mt-4 text-2xl">
          <a href="mailto:tucorreo@example.com" className="hover:text-blue-600"><FaEnvelope /></a>
          <a href="https://github.com/tuusuario" className="hover:text-gray-800"><FaGithub /></a>
          <a href="https://linkedin.com/in/tuusuario" className="hover:text-blue-700"><FaLinkedin /></a>
        </div>
      </section>

     
      <section className="max-w-5xl mx-auto px-4 py-12">
        <h2 className="text-3xl font-semibold mb-8 text-center">Proyectos</h2>
        <div className="grid md:grid-cols-2 gap-6">
          {projects.map((project, index) => (
            <div key={index} className="border p-4 rounded-xl shadow hover:shadow-lg transition">
              <h3 className="text-xl font-bold">{project.title}</h3>
              <p className="text-gray-600 my-2">{project.description}</p>
              <a href={project.url} className="text-blue-500 hover:underline" target="_blank" rel="noopener noreferrer">
                Ver en GitHub
              </a>
            </div>
          ))}
        </div>
      </section>

      {/* Habilidades */}
      <section className="bg-gray-50 py-12 px-4">
        <h2 className="text-3xl font-semibold text-center mb-8">Habilidades</h2>
        <div className="flex flex-wrap justify-center gap-4">
          {skills.map((skill, index) => (
            <span key={index} className="bg-blue-100 text-blue-700 px-4 py-2 rounded-full text-sm">
              {skill}
            </span>
          ))}
        </div>
      </section>

      {/* Contacto */}
      <section className="text-center py-12 px-4">
        <h2 className="text-3xl font-semibold mb-4">Contacto</h2>
        <p className="mb-4">¿Te interesa colaborar o quieres contactarme?</p>
        <a
          href="mailto:tucorreo@example.com"
          className="inline-block bg-blue-600 text-white px-6 py-3 rounded-lg hover:bg-blue-700 transition"
        >
          Envíame un correo
        </a>
      </section>
    </div>
  );
}

<!--
**Alejandrobv25/Alejandrobv25** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
