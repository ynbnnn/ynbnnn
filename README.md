- 👋 Hi, I’m @ynbnnn
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
ynbnnn/ynbnnn is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import pandas as pd

url = 'https://lonca.gov.tr'  # Verilerin olduğu URL
veriler = pd.read_html(url)  # HTML tablolarını oku

df = veriler[0]  # İlgili tabloyu seçin (gerekirse indeksi değiştirin)

df.to_excel('veriler.xlsx', index=False)  # Verileri Excel'e kaydet
