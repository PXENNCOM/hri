# Node.js resmi imajını kullan
FROM node:18

# Uygulama klasörü oluştur
WORKDIR /app

# package.json ve package-lock.json dosyalarını kopyala
COPY package*.json ./

# Bağımlılıkları yükle
RUN npm install

# Tüm kaynak kodları kopyala
COPY . .

# Uygulamanın çalışacağı portu belirt
EXPOSE 8082

# Uygulamayı başlat
CMD ["npm", "start"]