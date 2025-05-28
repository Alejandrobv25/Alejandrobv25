## Hi there 👋

import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Mail, Github, Linkedin } from "lucide-react";

export default function App() {
  return (
    <main className="min-h-screen bg-gray-50 p-6 font-sans">
      <section className="max-w-4xl mx-auto text-center py-12">
        <h1 className="text-4xl font-bold mb-4">[Tu Nombre Aquí]</h1>
        <p className="text-lg text-gray-700 mb-6">[Tu Profesión o Título profesional]</p>
        <div className="flex justify-center gap-4 mb-10">
          <a href="mailto:tucorreo@example.com"><Mail /></a>
          <a href="https://github.com/tuusuario"><Github /></a>
          <a href="https://linkedin.com/in/tuusuario"><Linkedin /></a>
        </div>
      </section>

      <section className="max-w-4xl mx-auto py-8">
        <h2 className="text-2xl font-semibold mb-6">Proyectos Destacados</h2>
        <div className="grid gap-6 md:grid-cols-2">
          {/* Copia este bloque para cada proyecto */}
          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-bold">[Nombre del Proyecto]</h3>
              <p className="text-gray-600 mt-2">[Descripción corta del proyecto]</p>
              <a
                href="https://github.com/tuusuario/repositorio"
                className="text-blue-500 mt-2 inline-block"
              >
                Ver en GitHub
              </a>
            </CardContent>
          </Card>
        </div>
      </section>

      <section className="max-w-4xl mx-auto py-8">
        <h2 className="text-2xl font-semibold mb-6">Habilidades</h2>
        <ul className="grid grid-cols-2 md:grid-cols-4 gap-4 text-center text-gray-800">
          <li>JavaScript</li>
          <li>React</li>
          <li>Node.js</li>
          <li>Git</li>
          {/* Agrega más habilidades aquí */}
        </ul>
      </section>

      <section className="max-w-4xl mx-auto py-8">
        <h2 className="text-2xl font-semibold mb-6">Contacto</h2>
        <p className="text-center text-gray-700">¿Te interesa colaborar o contratarme? ¡Hablemos!</p>
        <div className="text-center mt-4">
          <Button asChild>
            <a href="mailto:tucorreo@example.com">Envíame un correo</a>
          </Button>
        </div>
      </section>
    </main>
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
