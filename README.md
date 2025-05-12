import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Mountain, Leaf, Map } from "lucide-react";
import { motion } from "framer-motion";

export default function ArgentinaNature() {
  return (
    <div className="min-h-screen bg-green-50 text-green-900 p-4 md:p-10 font-sans">
      <header className="text-center mb-10">
        <h1 className="text-4xl md:text-6xl font-bold mb-2">Argentina Nature</h1>
        <p className="text-lg md:text-xl text-green-700">Descubra as maravilhas naturais da Argentina</p>
      </header>

      <section className="grid grid-cols-1 md:grid-cols-3 gap-6 mb-12">
        <motion.div whileHover={{ scale: 1.05 }}>
          <Card className="bg-white shadow-md rounded-2xl">
            <CardContent className="p-6 text-center">
              <Mountain className="w-12 h-12 mx-auto text-green-700 mb-4" />
              <h2 className="text-xl font-semibold mb-2">Cordilheira dos Andes</h2>
              <p>
                Explore as majestosas montanhas dos Andes, que atravessam o oeste da Argentina com paisagens de tirar o fôlego.
              </p>
            </CardContent>
          </Card>
        </motion.div>

        <motion.div whileHover={{ scale: 1.05 }}>
          <Card className="bg-white shadow-md rounded-2xl">
            <CardContent className="p-6 text-center">
              <Leaf className="w-12 h-12 mx-auto text-green-700 mb-4" />
              <h2 className="text-xl font-semibold mb-2">Florestas de Misiones</h2>
              <p>
                Lar das Cataratas do Iguaçu, Misiones abriga uma rica biodiversidade e vegetação exuberante da Mata Atlântica.
              </p>
            </CardContent>
          </Card>
        </motion.div>

        <motion.div whileHover={{ scale: 1.05 }}>
          <Card className="bg-white shadow-md rounded-2xl">
            <CardContent className="p-6 text-center">
              <Map className="w-12 h-12 mx-auto text-green-700 mb-4" />
              <h2 className="text-xl font-semibold mb-2">Patagônia Selvagem</h2>
              <p>
                Descubra a natureza intocada da Patagônia, com geleiras, lagos cristalinos e vastas planícies.
              </p>
            </CardContent>
          </Card>
        </motion.div>
      </section>

      <footer className="text-center text-green-600">
        <p>© 2025 Argentina Nature. Todos os direitos reservados.</p>
        <Button className="mt-4" variant="outline">Saiba mais</Button>
      </footer>
    </div>
  );
}
