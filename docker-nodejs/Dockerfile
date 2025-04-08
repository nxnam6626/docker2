# Sử dụng node image từ Docker Hub
FROM node:18

# Thiết lập thư mục làm việc trong container
WORKDIR /usr/src/app

# Sao chép file package.json và cài đặt dependencies
COPY package*.json ./
RUN npm install

# Sao chép toàn bộ mã nguồn vào container
COPY . .

# Mở port 3000 để truy cập ứng dụng
EXPOSE 3000

# Chạy ứng dụng
CMD ["node", "index.js"]
