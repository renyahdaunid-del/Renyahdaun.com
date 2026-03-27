# Renyahdaun.com
renyah-daun/ ├── app/ │   ├── page.tsx │   ├── layout.tsx │   └── globals.css ├── public/ ├── package.json ├── tailwind.config.js ├── postcss.config.js ├── tsconfig.json └── next.config.js
import React from "react";

export default function RenyahDaunWebsite() { const featuredProducts = [ { name: "Nastar Premium", category: "Kue Kering", desc: "Lembut, buttery, dengan isian nanas legit khas rumahan. Cocok untuk hampers premium dan suguhan keluarga.", price: "Mulai Rp55.000", waText: "Halo Kak Renyah Daun, saya tertarik pesan Nastar Premium 🌿", }, { name: "Bolu Jadul Pandan", category: "Bolu", desc: "Aroma pandan harum, tekstur empuk, manis pas, menghadirkan rasa nostalgia dengan sentuhan premium.", price: "Mulai Rp48.000", waText: "Halo Kak Renyah Daun, saya tertarik pesan Bolu Jadul Pandan 🌿", }, { name: "Keripik Pisang Original", category: "Aneka Keripik", desc: "Renyah tipis, gurih manis, cocok untuk stok camilan harian maupun hantaran kecil yang berkesan.", price: "Mulai Rp22.000", waText: "Halo Kak Renyah Daun, saya tertarik pesan Keripik Pisang Original 🌿", }, { name: "Kembang Goyang Classic", category: "Kue Tradisional", desc: "Cita rasa tradisional Indonesia yang renyah, ringan, dan menghadirkan nuansa rumahan yang elegan.", price: "Mulai Rp35.000", waText: "Halo Kak Renyah Daun, saya tertarik pesan Kembang Goyang Classic 🌿", }, ];

const socials = [ { name: "Instagram", handle: "@renyahdaun.id", link: "https://instagram.com/renyahdaun.id", desc: "Lihat katalog, hampers, dan update produk terbaru", }, { name: "TikTok", handle: "@renyahdaun.id", link: "https://tiktok.com/@renyahdaun.id", desc: "Video produk, behind the scenes, dan promo", }, { name: "WhatsApp", handle: "+6282295840557", link: "https://wa.me/6282295840557", desc: "Fast response untuk order, custom hampers, dan reseller", }, { name: "Shopee", handle: "Renyah Daun Official", link: "https://shopee.co.id", desc: "Belanja praktis via marketplace official store", }, ];

const testimonials = [ { name: "Alya", text: "Nastarnya lembut banget dan kemasannya cantik, cocok banget buat hampers keluarga.", }, { name: "Rina", text: "Keripiknya renyah, rasanya nagih, dan kelihatan premium walau homemade.", }, { name: "Dewi", text: "Bolu pandan favorit anak-anak di rumah, wangi dan teksturnya empuk banget.", }, ];

const waNumber = "6282295840557"; const generalWa = https://wa.me/${waNumber}?text=${encodeURIComponent( "Halo Kak Renyah Daun, saya ingin tanya katalog dan pemesanan 🌿" )};

return ( <div className="min-h-screen bg-[#F7F3EB] text-[#4A3B2C] font-sans scroll-smooth"> <header className="sticky top-0 z-50 bg-white/90 backdrop-blur-md border-b border-[#E8E1D2]"> <div className="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between"> <div> <h1 className="text-2xl md:text-3xl font-bold tracking-wide text-[#355E3B]">Renyah Daun</h1> <p className="text-sm text-[#6C7A61] italic">Rasa rumahan, renyah berkesan</p> </div> <nav className="hidden md:flex items-center gap-6 text-sm font-medium text-[#5C4B3C]"> <a href="#tentang" className="hover:text-[#355E3B] transition">Tentang</a> <a href="#produk" className="hover:text-[#355E3B] transition">Produk</a> <a href="#hampers" className="hover:text-[#355E3B] transition">Hampers</a> <a href="#testimoni" className="hover:text-[#355E3B] transition">Testimoni</a> <a href="#kontak" className="hover:text-[#355E3B] transition">Kontak</a> <a
href={generalWa}
target="_blank"
rel="noreferrer"
className="bg-[#355E3B] text-white px-5 py-2.5 rounded-2xl shadow hover:opacity-90 transition"
> Order via WA </a> </nav> </div> </header>

<section className="max-w-7xl mx-auto px-6 py-16 md:py-24 grid md:grid-cols-2 gap-10 items-center">
    <div>
      <span className="inline-block bg-[#EDE7DA] text-[#7A5C3E] px-4 py-2 rounded-full text-sm font-semibold mb-5 shadow-sm">
        Homemade Artisan • Premium Giftable • Tradisional Modern
      </span>
      <h2 className="text-4xl md:text-6xl font-bold leading-tight text-[#355E3B]">
        Kue Tradisional, Kue Kering, Bolu & Keripik Premium untuk Momen Istimewa
      </h2>
      <p className="mt-6 text-lg text-[#6B5B4B] leading-relaxed">
        Renyah Daun menghadirkan aneka camilan homemade dengan cita rasa rumahan,
        sentuhan elegan, dan tampilan premium. Cocok untuk suguhan keluarga, hampers,
        acara spesial, hingga oleh-oleh yang berkesan.
      </p>
      <div className="mt-8 flex flex-wrap gap-4">
        <a
          href="#produk"
          className="bg-[#355E3B] text-white px-6 py-3 rounded-2xl shadow-md hover:opacity-90 transition"
        >
          Lihat Produk Andalan
        </a>
        <a
          href={generalWa}
          target="_blank"
          rel="noreferrer"
          className="border border-[#355E3B] text-[#355E3B] px-6 py-3 rounded-2xl hover:bg-[#355E3B] hover:text-white transition"
        >
          Tanya & Pesan Sekarang
        </a>
      </div>
    </div>

    <div className="grid grid-cols-2 gap-4">
      <div className="bg-white rounded-3xl p-6 shadow-lg border border-[#E8E1D2] h-52 flex flex-col justify-between">
        <p className="text-sm text-[#7A5C3E]">Best Seller</p>
        <h3 className="text-xl font-bold text-[#355E3B]">Nastar Premium</h3>
        <p className="text-sm text-[#6B5B4B]">Buttery, lembut, manis pas, favorit untuk hampers premium.</p>
      </div>
      <div className="bg-[#A8B89A] rounded-3xl p-6 shadow-lg h-60 text-white flex flex-col justify-between">
        <p className="text-sm opacity-90">Homemade Signature</p>
        <h3 className="text-2xl font-bold">Bolu Jadul Pandan</h3>
        <p className="text-sm opacity-95">Wangi pandan khas, empuk, klasik, dan disukai semua usia.</p>
      </div>
      <div className="bg-[#F2E8D8] rounded-3xl p-6 shadow-lg h-60 flex flex-col justify-between">
        <p className="text-sm text-[#7A5C3E]">Snack Favorite</p>
        <h3 className="text-xl font-bold text-[#8B5E3C]">Keripik Pisang</h3>
        <p className="text-sm text-[#6B5B4B]">Renyah tipis, gurih manis, cocok untuk stok camilan harian.</p>
      </div>
      <div className="bg-white rounded-3xl p-6 shadow-lg border border-[#E8E1D2] h-52 flex flex-col justify-between">
        <p className="text-sm text-[#7A5C3E]">Traditional Choice</p>
        <h3 className="text-xl font-bold text-[#355E3B]">Kembang Goyang</h3>
        <p className="text-sm text-[#6B5B4B]">Nostalgia tradisional dengan tampilan lebih premium.</p>
      </div>
    </div>
  </section>

  <section id="tentang" className="bg-white py-16 px-6">
    <div className="max-w-6xl mx-auto grid md:grid-cols-3 gap-6">
      <div className="md:col-span-2">
        <h3 className="text-3xl font-bold text-[#355E3B] mb-4">Tentang Renyah Daun</h3>
        <p className="text-[#6B5B4B] leading-relaxed text-lg">
          Renyah Daun adalah brand homemade artisan yang memadukan rasa tradisional Indonesia
          dengan kemasan modern premium. Setiap produk dibuat dengan bahan pilihan, cita rasa hangat,
          dan sentuhan elegan agar cocok untuk konsumsi pribadi, hadiah, maupun peluang reseller.
        </p>
      </div>
      <div className="bg-[#F7F3EB] rounded-3xl p-6 shadow-sm border border-[#E8E1D2]">
        <h4 className="font-bold text-[#355E3B] mb-3">Kategori Utama</h4>
        <ul className="space-y-2 text-[#6B5B4B]">
          <li>• Kue Tradisional</li>
          <li>• Kue Kering Premium</li>
          <li>• Bolu & Cake Rumahan</li>
          <li>• Aneka Keripik Renyah</li>
        </ul>
      </div>
    </div>
  </section>

  <section id="produk" className="py-16 px-6">
    <div className="max-w-7xl mx-auto">
      <div className="text-center mb-10">
        <h3 className="text-3xl md:text-4xl font-bold text-[#355E3B]">Produk Andalan</h3>
        <p className="mt-3 text-[#6B5B4B]">Pilihan favorit pelanggan untuk camilan, hampers, dan suguhan spesial.</p>
      </div>
      <div className="grid sm:grid-cols-2 lg:grid-cols-4 gap-6">
        {featuredProducts.map((product, idx) => (
          <div
            key={idx}
            className="bg-white rounded-3xl p-6 shadow-md border border-[#E8E1D2] hover:shadow-xl transition"
          >
            <div className="h-36 rounded-2xl bg-gradient-to-br from-[#E8E1D2] to-[#F7F3EB] mb-4 flex items-center justify-center text-center px-4">
              <span className="font-semibold text-[#7A5C3E]">Foto Produk {product.name}</span>
            </div>
            <p className="text-xs uppercase tracking-wide text-[#8B5E3C] font-semibold">{product.category}</p>
            <h4 className="text-xl font-bold text-[#355E3B] mt-2">{product.name}</h4>
            <p className="text-sm text-[#6B5B4B] mt-2">{product.desc}</p>
            <p className="mt-4 font-semibold text-[#7A5C3E]">{product.price}</p>
            <a
              href={`https://wa.me/${waNumber}?text=${encodeURIComponent(product.waText)}`}
              target="_blank"
              rel="noreferrer"
              className="mt-4 block w-full text-center bg-[#355E3B] text-white py-3 rounded-2xl hover:opacity-90 transition"
            >
              Pesan via WhatsApp
            </a>
          </div>
        ))}
      </div>
    </div>
  </section>

  <section id="hampers" className="bg-[#EEF2E7] py-16 px-6">
    <div className="max-w-6xl mx-auto grid md:grid-cols-2 gap-8 items-center">
      <div>
        <h3 className="text-3xl font-bold text-[#355E3B] mb-4">Paket Hampers & Custom Order</h3>
        <p className="text-[#6B5B4B] text-lg leading-relaxed">
          Tersedia paket hampers premium untuk hari raya, ulang tahun, acara keluarga, bingkisan kantor,
          dan hadiah spesial. Bisa custom isi, tema warna, kartu ucapan, dan jumlah pesanan.
        </p>
        <ul className="mt-5 space-y-3 text-[#5C4B3C]">
          <li>• Hampers premium siap kirim</li>
          <li>• Bisa custom isi produk</li>
          <li>• Cocok untuk gift & corporate order</li>
          <li>• Bisa request kemasan eksklusif</li>
        </ul>
        <a
          href={`https://wa.me/${waNumber}?text=${encodeURIComponent(
            "Halo Kak Renyah Daun, saya ingin tanya paket hampers dan custom order 🌿"
          )}`}
          target="_blank"
          rel="noreferrer"
          className="inline-block mt-6 bg-[#355E3B] text-white px-6 py-3 rounded-2xl shadow hover:opacity-90 transition"
        >
          Tanya Paket Hampers
        </a>
      </div>
      <div className="bg-white rounded-3xl p-8 shadow-lg border border-[#DDE5D1] min-h-[280px] flex items-center justify-center text-center">
        <p className="text-[#7A5C3E] font-semibold">Area Foto Hampers / Packaging Premium Renyah Daun</p>
      </div>
    </div>
  </section>

  <section id="testimoni" className="py-16 px-6 bg-white">
    <div className="max-w-6xl mx-auto">
      <div className="text-center mb-10">
        <h3 className="text-3xl font-bold text-[#355E3B]">Testimoni Pelanggan</h3>
        <p className="mt-3 text-[#6B5B4B]">Kesan hangat dari pelanggan yang sudah mencoba produk Renyah Daun.</p>
      </div>
      <div className="grid md:grid-cols-3 gap-6">
        {testimonials.map((item, idx) => (
          <div key={idx} className="bg-[#F7F3EB] rounded-3xl p-6 border border-[#E8E1D2] shadow-sm">
            <p className="text-[#5C4B3C] leading-relaxed">“{item.text}”</p>
            <p className="mt-4 font-semibold text-[#355E3B]">— {item.name}</p>
          </div>
        ))}
      </div>
    </div>
  </section>

  <section className="bg-[#355E3B] text-white py-12 px-6">
    <div className="max-w-6xl mx-auto text-center">
      <h3 className="text-3xl md:text-4xl font-bold">Siap Pesan untuk Keluarga, Hampers, atau Reseller?</h3>
      <p className="mt-4 text-white/90 max-w-3xl mx-auto">
        Hubungi Renyah Daun sekarang untuk pemesanan produk homemade premium dengan rasa rumahan yang berkesan.
      </p>
      <a
        href={generalWa}
        target="_blank"
        rel="noreferrer"
        className="inline-block mt-6 bg-white text-[#355E3B] px-8 py-3 rounded-2xl font-semibold shadow hover:opacity-90 transition"
      >
        Order Sekarang via WhatsApp
      </a>
    </div>
  </section>

  <section id="kontak" className="py-16 px-6">
    <div className="max-w-6xl mx-auto grid md:grid-cols-2 gap-8">
      <div>
        <h3 className="text-3xl font-bold text-[#355E3B] mb-4">Hubungi & Ikuti Kami</h3>
        <p className="text-[#6B5B4B] mb-6">
          Siap menerima pesanan untuk konsumsi pribadi, hampers, acara keluarga, hingga reseller dan custom order.
        </p>
        <div className="space-y-4">
          {socials.map((social, idx) => (
            <a
              key={idx}
              href={social.link}
              target="_blank"
              rel="noreferrer"
              className="block bg-white rounded-2xl p-4 shadow-sm border border-[#E8E1D2] hover:shadow-md transition"
            >
              <p className="font-semibold text-[#355E3B]">{social.name}</p>
              <p className="text-[#6B5B4B] text-sm">{social.handle}</p>
              <p className="text-xs text-[#8B7A67] mt-1">{social.desc}</p>
            </a>
          ))}
        </div>
      </div>

      <div className="bg-white rounded-3xl p-8 shadow-lg border border-[#E8E1D2]">
        <h4 className="text-2xl font-bold text-[#355E3B] mb-4">Info Pemesanan</h4>
        <div className="space-y-4 text-[#5C4B3C]">
          <div className="bg-[#F7F3EB] rounded-2xl p-4 border border-[#E8E1D2]">
            <p className="font-semibold text-[#355E3B]">WhatsApp</p>
            <p>+62 812-3456-7890</p>
          </div>
          <div className="bg-[#F7F3EB] rounded-2xl p-4 border border-[#E8E1D2]">
            <p className="font-semibold text-[#355E3B]">Jam Layanan</p>
            <p>Senin - Sabtu • 08.00 - 20.00</p>
          </div>
          <div className="bg-[#F7F3EB] rounded-2xl p-4 border border-[#E8E1D2]">
            <p className="font-semibold text-[#355E3B]">Layanan</p>
            <p>Pre-order • Hampers • Custom Order • Reseller</p>
          </div>
        </div>
        <a
          href={generalWa}
          target="_blank"
          rel="noreferrer"
          className="block mt-6 w-full text-center bg-[#355E3B] text-white py-3 rounded-2xl font-semibold hover:opacity-90 transition"
        >
          Chat WhatsApp Sekarang
        </a>
      </div>
    </div>
  </section>

  <footer className="bg-[#2F4E34] text-white py-8 px-6">
    <div className="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between gap-4">
      <div>
        <h4 className="text-xl font-bold">Renyah Daun</h4>
        <p className="text-sm opacity-90">Rasa rumahan, renyah berkesan</p>
      </div>
      <p className="text-sm opacity-90">© 2026 Renyah Daun • Homemade Artisan Bakery & Snack</p>
    </div>
  </footer>
</div>

); }
