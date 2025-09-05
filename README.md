import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { Instagram, Phone } from "lucide-react"; import { motion } from "framer-motion";

export default function SMWebsite() { return ( <div className="bg-pink-50 min-h-screen text-gray-800 font-poppins"> {/* Header */} <header className="flex justify-between items-center p-6 shadow-md bg-white"> <div className="flex items-center gap-2"> <img
src="/logo-sm.png"
alt="Logo SM Personalizados"
className="h-12 w-12 rounded-full"
/> <h1 className="text-xl font-bold text-pink-500">SM Personalizados</h1> </div> <nav className="flex gap-6 text-pink-600 font-medium"> <a href="#sobre">Sobre</a> <a href="#produtos">Produtos</a> <a href="#contato">Contato</a> </nav> </header>

{/* Hero Section */}
  <section className="text-center py-16 bg-gradient-to-r from-pink-100 to-pink-200">
    <motion.h2
      initial={{ opacity: 0, y: 20 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.8 }}
      className="text-3xl font-bold text-pink-600"
    >
      Transforme suas ideias em canecas exclusivas
    </motion.h2>
    <p className="mt-4 text-gray-600 max-w-xl mx-auto">
      Canecas de porcelana personalizadas para presentear, divulgar sua marca
      ou deixar seu dia mais especial.
    </p>
    <Button className="mt-6 bg-pink-500 hover:bg-pink-600 text-white px-6 py-2 rounded-2xl shadow-lg">
      Ver Produtos
    </Button>
  </section>

  {/* Sobre */}
  <section id="sobre" className="py-16 px-6 max-w-4xl mx-auto text-center">
    <h3 className="text-2xl font-bold text-pink-600 mb-4">Sobre Nós</h3>
    <p className="text-gray-700 leading-relaxed">
      Na SM Personalizados, transformamos suas ideias em canecas exclusivas e únicas.
      Trabalhamos com personalização de canecas de porcelana para presentear ou divulgar
      sua marca, ou simplesmente deixar o seu dia mais especial.
    </p>
  </section>

  {/* Produtos */}
  <section id="produtos" className="py-16 px-6 bg-white">
    <h3 className="text-2xl font-bold text-center text-pink-600 mb-8">Nossos Produtos</h3>
    <div className="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-6xl mx-auto">
      {[1, 2, 3].map((item) => (
        <Card key={item} className="rounded-2xl shadow-md hover:shadow-lg">
          <CardContent className="p-4 flex flex-col items-center">
            <img
              src={`/caneca${item}.jpg`}
              alt={`Caneca ${item}`}
              className="rounded-xl w-full h-48 object-cover"
            />
            <h4 className="mt-4 font-semibold text-gray-700">Caneca {item}</h4>
            <Button className="mt-3 bg-pink-500 hover:bg-pink-600 text-white w-full rounded-xl">
              Pedir pelo WhatsApp
            </Button>
          </CardContent>
        </Card>
      ))}
    </div>
  </section>

  {/* Contato */}
  <section id="contato" className="py-16 px-6 bg-pink-50">
    <h3 className="text-2xl font-bold text-center text-pink-600 mb-6">Entre em Contato</h3>
    <div className="flex flex-col items-center gap-4">
      <a
        href="https://www.instagram.com/sm_personalizadosltda"
        target="_blank"
        className="flex items-center gap-2 text-pink-600 hover:underline"
      >
        <Instagram /> @sm_personalizadosltda
      </a>
      <a
        href="https://wa.me/5551991400100"
        target="_blank"
        className="flex items-center gap-2 text-pink-600 hover:underline"
      >
        <Phone /> (51) 99140-0100
      </a>
    </div>
  </section>

  {/* Footer */}
  <footer className="py-6 text-center text-gray-600 text-sm bg-white border-t">
    © {new Date().getFullYear()} SM Personalizados. Todos os direitos reservados.
  </footer>
</div>

); }
