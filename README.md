# HTML content updated with Malay translation, contact info, WhatsApp button, and logo
html_content = """
<!DOCTYPE html>
<html lang="ms">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Khidmat SSM Mudah & Pantas | SG Solution</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
</head>
<body class="bg-gray-100 text-gray-800">

  <!-- Header with Logo -->
  <header class="bg-blue-900 text-white py-6">
    <div class="container mx-auto flex flex-col items-center">
      <img src="logo.jpeg" alt="SG Solution Logo" class="w-24 h-24 mb-4 rounded-full border-4 border-white shadow-lg">
      <h1 class="text-3xl font-bold">Khidmat SSM Mudah & Pantas</h1>
      <p class="text-lg mt-2">Bersama SG Solution</p>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="py-10 text-center bg-white">
    <div class="container mx-auto">
      <h2 class="text-2xl font-semibold mb-4">Urus Perniagaan Anda Dengan Mudah & Cepat</h2>
      <p class="text-gray-600 max-w-xl mx-auto">
        Kami menyediakan perkhidmatan SSM yang cepat, dipercayai dan sepenuhnya digital menggunakan Google Workspace (Docs & Drive) untuk pengurusan dokumen yang selamat dan cekap.
      </p>
    </div>
  </section>

  <!-- Services Section -->
  <section class="py-10 bg-gray-100">
    <div class="container mx-auto">
      <h3 class="text-xl font-bold text-center mb-6">Perkhidmatan Kami</h3>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <div class="bg-white p-5 rounded shadow text-center">✅ Pendaftaran SSM Baharu</div>
        <div class="bg-white p-5 rounded shadow text-center">✅ Pembaharuan SSM</div>
        <div class="bg-white p-5 rounded shadow text-center">✅ Kemaskini Maklumat Perniagaan</div>
        <div class="bg-white p-5 rounded shadow text-center">✅ Permintaan Dokumen Rasmi</div>
        <div class="bg-white p-5 rounded shadow text-center">✅ Penutupan Perniagaan</div>
      </div>
    </div>
  </section>

  <!-- Contact & WhatsApp -->
  <section class="py-10 bg-blue-900 text-white text-center">
    <div class="container mx-auto">
      <h3 class="text-xl font-bold mb-4">Hubungi Kami Hari Ini</h3>
      <p class="text-lg mb-4">Untuk bantuan pakar & proses yang lancar</p>
      <a href="mailto:sgsolution73@gmail.com" class="block text-lg underline mb-2">📧 sgsolution73@gmail.com</a>
      <a href="https://wa.me/60173239181" class="inline-block bg-green-500 text-white px-6 py-2 rounded font-semibold shadow hover:bg-green-600">
        💬 WhatsApp Kami
      </a>
    </div>
  </section>

  <!-- Footer -->
  <footer class="py-4 bg-gray-800 text-center text-white text-sm">
    &copy; 2025 SG Solution. Semua hak cipta terpelihara.
  </footer>
</body>
</html>
"""

# Save updated HTML file
html_path = os.path.join(site_dir, "index.html")
with open(html_path, "w") as file:
    file.write(html_content.strip())

# Zip the folder
zip_path = "/mnt/data/ssm_website_updated.zip"
shutil.make_archive("/mnt/data/ssm_website_updated", 'zip', site_dir)

zip_path
