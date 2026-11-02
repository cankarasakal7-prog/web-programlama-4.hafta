# 🎨 CSS Seçicileri (Selectors) ve Kullanımı

Bu rehber, CSS'te kullanılan temel ve gelişmiş seçicileri ve ne işe yaradıklarını açıklamaktadır.

---

### 1. Etiket Seçici (Tag Selector) — `body`, `h1`
* **Tanım:** HTML etiketinin adıyla doğrudan seçim yapar.
* **Kullanım:** Sayfadaki tüm o etiket türlerini doğrudan etkiler.
```css
h1 {
  color: blue;
}
```

---

### 2. Kimlik (ID) Seçici — `#logo`
* **Tanım:** HTML'de `id="logo"` olan elemanı seçer.
* **Kullanım:** Başına **`#`** simgesi konur. Bir sayfada benzersizdir, sadece **1 kez** kullanılır.
```css
#logo {
  width: 150px;
}
```

---

### 3. Sınıf (Class) Seçici — `.gezegen-karti`
* **Tanım:** HTML'de `class="gezegen-karti"` olan elemanları seçer.
* **Kullanım:** Başına **`.` (nokta)** konur. Birden fazla farklı elemana aynı sınıf verilerek tekrar tekrar kullanılabilir.
```css
.gezegen-karti {
  background-color: #f4f4f4;
  padding: 15px;
}
```

---

### 4. Torun (Descendant) Seçici — `.gezegen-karti img`
* **Tanım:** Aralarında boşluk bırakılarak yazılır.
* **Kullanım:** Belirtilen bir kutunun veya kapsayıcının içindeki (ne kadar derinde olursa olsun) alt elemanları seçer.
```css
.gezegen-karti img {
  border-radius: 8px;
}
```

---

### 5. Sözde Sınıf (Pseudo-Class) — `:hover`
* **Tanım:** Elemanın özel bir durumunu hedef alır.
* **Kullanım:** Kullanıcı fare ile elemanın üzerine geldiği anki stilini belirlemek için sıklıkla kullanılır.
```css
button:hover {
  background-color: green;
}
```

---

### 6. Sözde Eleman (Pseudo-Element) — `::first-letter`, `::selection`
* **Tanım:** Elemanın tamamını değil, sadece belirli bir parçasını hedef alır.
* **Kullanım:** Çift iki nokta **`::`** ile yazılır (örn: metnin ilk harfi veya fareyle maviye boyanarak seçilen kısmı).
```css
p::first-letter {
  font-size: 200%;
  font-weight: bold;
}
```