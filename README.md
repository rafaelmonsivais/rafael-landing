# rafael-landing
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { ArrowRight } from "lucide-react";
import { motion } from "framer-motion";

export default function LandingPage() {
  return (
    <div className="min-h-screen bg-white text-gray-900 px-6 py-12 md:px-20">
      <section className="text-center mb-20">
        <motion.h1
          className="text-4xl md:text-6xl font-bold mb-4"
          initial={{ opacity: 0, y: -30 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.6 }}
        >
          Rafael Monsivais Salazar
        </motion.h1>
        <p className="text-lg md:text-xl text-gray-600 max-w-2xl mx-auto">
          Emprendedor, consultor y educador en inteligencia artificial. Transformo negocios con procesos digitales, flores y tecnología.
        </p>
      </section>

      <section className="grid md:grid-cols-3 gap-8 mb-24">
        <Card>
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-2">Florería Suspiros</h2>
            <p className="text-gray-600 mb-4">
              Plataforma que conecta pedidos de flores con talleres florales locales en toda Latinoamérica. Calidad, puntualidad y diseño.
            </p>
            <Button variant="outline">
              Visitar sitio
              <ArrowRight className="ml-2 w-4 h-4" />
            </Button>
          </CardContent>
        </Card>

        <Card>
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-2">Consultoría</h2>
            <p className="text-gray-600 mb-4">
              Transformación digital para empresas. Migramos sistemas a Notion e integramos inteligencia artificial con automatización total.
            </p>
            <Button variant="outline">
              Solicitar auditoría
              <ArrowRight className="ml-2 w-4 h-4" />
            </Button>
          </CardContent>
        </Card>

        <Card>
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-2">IA para Profesionales</h2>
            <p className="text-gray-600 mb-4">
              Cursos para dominar la IA aplicada al trabajo. Desde mejorar tu productividad hasta lanzar una florería en línea.
            </p>
            <Button variant="outline">
              Ver cursos
              <ArrowRight className="ml-2 w-4 h-4" />
            </Button>
          </CardContent>
        </Card>
      </section>

      <section className="text-center">
        <h3 className="text-3xl font-bold mb-4">Conecta conmigo</h3>
        <p className="text-gray-600 mb-6 max-w-xl mx-auto">
          ¿Quieres digitalizar tu empresa, aprender IA o enviar flores? Estoy aquí para ayudarte.
        </p>
        <div className="flex justify-center gap-4 flex-wrap">
          <Button variant="secondary">TikTok</Button>
          <Button variant="secondary">Instagram</Button>
          <Button variant="secondary">LinkedIn</Button>
          <Button variant="secondary">WhatsApp</Button>
        </div>
      </section>
    </div>
  );
}
