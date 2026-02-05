import { motion } from "framer-motion";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";


export default function SteelWeldingFabricationWebsite() {
return (


{/* Hero */}


<motion.div initial={{ opacity: 0, y: 30 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 0.8 }}>

Precision Steel Welding & Fabrication



Custom metal solutions built to last — residential, commercial, and industrial fabrication.


Request a Quote
</motion.div>




  {/* Services */}
  <section className="py-20 px-6 bg-gray-900">
    <h2 className="text-3xl font-semibold text-center mb-12">Our Services</h2>
    <div className="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-6xl mx-auto">
      {["Structural Steel Welding", "Custom Fabrication", "Repairs & Modifications"].map((service) => (
        <Card key={service} className="bg-gray-800 border-gray-700">
          <CardContent className="p-6">
            <h3 className="text-xl font-semibold mb-2">{service}</h3>
            <p className="text-gray-300">High-quality workmanship with strict safety and durability standards.</p>
          </CardContent>
        </Card>
      ))}
    </div>
  </section>

  {/* About */}
  <section className="py-20 px-6">
    <div className="max-w-4xl mx-auto text-center">
      <h2 className="text-3xl font-semibold mb-6">About Us</h2>
      <p className="text-gray-300 text-lg">
        We are a professional steel welding and fabrication company committed to precision, strength, and reliability.
        With years of hands-on experience, we deliver custom solutions tailored to your project requirements.
      </p>
    </div>
  </section>

  {/* Contact */}
  <section className="py-20 px-6 bg-gray-900">
    <div className="max-w-3xl mx-auto text-center">
      <h2 className="text-3xl font-semibold mb-6">Get in Touch</h2>
      <p className="text-gray-300 mb-8">Ready to start your project? Contact us today for a free quote.</p>
      <div className="flex flex-col md:flex-row gap-4 justify-center">
        <Button className="px-6 py-5">Call Us</Button>
        <Button variant="outline" className="px-6 py-5">Email Us</Button>
      </div>
    </div>
  </section>

  {/* Footer */}
  <footer className="py-6 text-center text-gray-400 text-sm">
    © {new Date().getFullYear()} Steel Welding & Fabrication. All rights reserved.
  </footer>
</div>



);
}

