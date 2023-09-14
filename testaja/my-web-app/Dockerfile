# Gunakan image base Python
FROM python:3.8-slim

# Set working directory
WORKDIR /app

# Salin file requirements.txt ke direktori kerja
COPY requirements.txt .

# Pasang dependensi Python
RUN pip install --no-cache-dir -r requirements.txt

# Salin file aplikasi Flask ke direktori kerja
COPY app.py .

# Expose port yang akan digunakan oleh aplikasi
EXPOSE 8080

# Menjalankan aplikasi Flask
CMD ["python", "app.py"]
