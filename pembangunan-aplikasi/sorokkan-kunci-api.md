---
description: alur kerja untuk menyorokkan kunci API
---

# Sorokkan Kunci API

1. Simpan kunci API dalam satu fail, contoh: Constants/K
2. Isikan data dan maklumat yang sensitif dalam fail ini, seperti kunci API, rahsia OAuth dsb.
3. Di dalam kod, tulis kunci API sebagai pembolehubah \(variable\) yang dinyatakan di dalam fail Constants. 

   ```text
   let apiKey = Constant.ApiKey

   // instead of 
   // let apiKey = "987654321"
   ```

4. Cipta satu fail `.gitignore` di dalam direktori kerja
5. Buka fail `.gitignore`, dan isikan fail yang tidak perlu di commit/push oleh git. contoh: `Constants.swift`
6. Simpan dan tutup fail.
7. Di dalam terminal, taip `git status`. Fail `.gitignore` akan dipapar dan sedia untuk di kesan.
8. Taip `git add .` dan `git status` semula untuk melihat status fail tersebut. Jika semuanya ok, boleh teruskan dengan commit dan push ke repo rimot.
9. Di dalam repo rimot, tambahkan nota di dalam `README.md`, nyatakan bagaimana untuk cipta semula projek menggunakan kunci API sendiri.



sumber: [How to hide your API keys](https://ayunascode.medium.com/how-to-hide-your-api-keys-367ef6589949), [Hide API Keys](https://gist.github.com/derzorngottes/3b57edc1f996dddcab25)

